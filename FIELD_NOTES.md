# Field notes from the first full run (Sote Bhagwan Ko Jagane Wala Balak)

These notes override older text in the other files where they disagree.

## Prompts
- Keep scene prompts SHORT. Format: shot, "calm camera", who speaks (Hindi line in quotes), "Only <speaker>'s mouth moves", others "keep their mouths closed", "Exactly N characters, each appearing once", "Ends on a held calm pose".
- NEVER write "No subtitles" or mention on-screen text in a video prompt. The model burns captions into the video when it sees those words. Clips 35-40, 45-50, 52-58, 60 had to be redone for this reason.
- Duplicates (two Garud, two Vishnu): regenerate the image with "only ONE ... no other bird/creature" and repeat it in the video prompt.
- Narrator clips: tick "Video Only" so they stay silent; narration comes from clonevoice.

## Shesh Naag
- Saved sheet is a BLACK serpent with cobra faces; the model gives 3 hoods (a large crowned centre hood), not 5 or 7. Do not say "seven hoods" in any spoken line; the Guru's "seven hoods" lines and narrator clip 19 were changed accordingly. Record the real hood count in the report.

## VideoExpress mechanics
- Server errors "Please try again later": wait 60-90 s or use the other image variant.
- Library list shows 20 items; press "More" to load the rest. Drag-and-drop onto the timeline places a clip at the drop time (zoom 0.02 = 20 px/s; `left` is start in ms).
- A whole project can be built in the browser console: `app.getProjectData()` -> edit `data[track].bricks` (type video/audio, `left`, `duration`, `media_id`, fileName, path) -> `app.loadProjectData(project, project.data)`.
- Narration audio: download URL from clonevoice is `cdn.clonevoice.ai/uploads/production/...mp3` (CORS open); upload to VideoExpress with POST `/library/upload/4` (fields `file`, `categoryId`).
- With 60+ clips the in-app preview may report "Unable to update timeline videos" (browser decoder limit); the server render still works. Verify the exported MP4 instead.

## Length
- The 61-clip ledger adds up to about 8 minutes, not 6. Trim clips or lines if 6 minutes is a hard limit.

## Bhai Dooj run: duplicate characters and the fix

- First clip test: with the 3-view sheets of Jamuni and Bholu as Reference Photo 1 and 2, all four variants (two attempts) showed **two Jamunis plus Bholu**, even with "exactly 2 characters" and "exactly one girl" in the prompt. The model copies the repeated figure on the sheet.
- Fix: make a **single-pose image** of each character (text-only Create Image with Consistent Character OFF, "exactly one figure", one front view) and use those as the references. With Jamuni-Single + Bholu-Single the same clip gave exactly two characters in both variants.
- Image prompts for 2+ characters also carry: "Each named character appears exactly once (...); there is no second copy, no twin and no look-alike of any character, no character sheet and no multiple views of the same person."
- VideoExpress does not ask for a name when saving an image; recognise images by thumbnail and by order (newest first). In the reference picker, open the My AI Images folder with a single click, then scroll; selecting an image and pressing Choose fills the slot.
- Narrator clips: tick Advanced Mode, **Video Only (No Sound)** and **Manual Video Length**, and keep Automatically enhance my video prompt OFF.
- Image variants can take 60 to 90 s to appear; wait, do not resubmit.

## Bhai Dooj run — production learnings (added 2026-10-27)
- Group reference images: for 3+ characters including Jamuni+Bholu, upload a DUO (Jamuni+Bholu) reference plus the third character's single; for 5 characters use [DUO, TRIO]. This keeps outfits correct and avoids duplicate look-alikes.
- Video queue: keep at most 5 videos in progress; "Error. Please try again later" is a rate/queue error — wait ~25 s and resubmit.
- Review every image before making its video; reject extra tiny people, duplicated characters and prop leakage, then regenerate that clip's image.
- Narration Video (Choose my Audio) is 9:16 only, and clonevoice Voice Changer has no Hindi voices. So dialogue clips are generated with native speech, muted on the timeline, and the character's clonevoice audio is placed on the audio track.
- Importing clonevoice audio: payload is an array of {id,uuid,src,title} with actionPath `voice_clone/generated_audio_import`; items land in "My CloneVoice.ai Audio".
- Timeline: hooks first, then clips 1..N in order; video track volume 0, audio track starts at the clip's start.

## Bhai Dooj run — lipsync fix: single-speaker audio-driven clips (added 2026-10-27)
- With several characters in a shot, native speech / audio-driven video animates only the leftmost character (the wrong mouth moves, e.g. Acharya's line spoken by Jamuni). Fix: every dialogue clip is a separate single-character shot, so the speaker is the only face on screen.
- Audio-driven method that works at 16:9: `image2video` with `audioMediaId` = the character's clonevoice audio (library id from "My CloneVoice.ai Audio"), `isNarrationVideo:'1'`, `videoLength` = ceil(audio seconds), `aspect:'16:9'`. The supplied audio is embedded in the video, so no separate audio brick is needed; keep the brick volume at 100. Narrator clips stay silent video (volume 0) plus the Narrator audio brick.
- Per-clip workflow: character image alone (rotate village settings) -> `save_generated_image` -> `image2video`. Speaker comes from the clip's heading ("— N — Narrator" = narrator clip).
- "Multiple videos in progress" means 5 are rendering. A submit that was accepted is not finished: poll `ai/api/status/<uuid>` for every uuid, not just the ones you track. Wait for slots and retry.
- Do not write "no text / no subtitles / no captions" in audio-driven prompts: the model sometimes prints that wording as a burned-in garbled caption. Omit it; if captions still appear, regenerate the clip (the fix-subtitles endpoint does not support "Create Video From Prompt" clips). Check each clip at ~2 s and ~3.5 s for captions.
- Magic/sparkle/"divine guests" wording makes the video model add extra people mid-clip (clip 46 got extra girls). Use a static, calm prompt: "exactly three characters stand in place, fold hands, no one enters the frame".
- A new CDN file can return 404 for 1-2 minutes after status SUCCEEDED; overlays with many `<video>` tags slow the editor page, so remove them before bulk timeline edits.
- Timeline rebuild: `brickItemsCollection.remove(models)` clears, then `onMediaTimelineDropped` with track model `trackItemsCollection.get('30')` for video and `get('32')` for audio, left = ms*0.005. After Save, a "Unable to update timeline videos" confirm may show if a clip is not on the CDN yet; click Yes and Save again.
- Export: Export Video -> FullHD / mp4 / High -> Create; it is queued and appears under My Videos.
