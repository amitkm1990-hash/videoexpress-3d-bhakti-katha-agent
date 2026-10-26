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
