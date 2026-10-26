# VideoExpress 3D Bhakti-Katha Agent v2 — "सोते भगवान को जगाने वाला बालक"

A system prompt, character kit and ready-to-paste clip prompts for producing a 6-minute, 16:9, Pixar-style 3D Hindi bhakti-katha in VideoExpress.ai about Dev Uthani Ekadashi: hungry little Tunnu scolds the Lord who has slept four months, his guru insists "Vishnu ji toh Ekadashi par hi uthenge", then Maa Lakshmi, Shesh Naag and Garud come in turn, and finally Shri Hari wakes.

Built on `videoexpress-3d-bhakti-katha-agent`, with fixes for the problems seen in earlier videos.

## What is new in v2

| Problem before | Fix here |
|---|---|
| Characters changed from clip to clip | Characters come only from images you create once (CHARACTER_SHEETS.md); identity locks are pasted word for word into every prompt |
| Several copies of one character in one scene | Exact headcount in every prompt, a census check on the start, middle and end frame of every clip, no idols or reflections, no crowds, designed look-alike separation |
| Gods looked simplified | DEITY_ICONOGRAPHY.md: real traditional forms (Vishnu with four arms, chakra, conch, lotus, mace; Lakshmi with lotus; Shesh Naag (see FIELD_NOTES.md for the real hood count); eagle-faced Garud) |
| Wrong character speaking or listeners moving lips | One owner per line; every non-speaker's mouth closed; every mouth closed during narration |

## Use

1. Create the 9 images in CHARACTER_SHEETS.md yourself in VideoExpress and save them in My AI Images under the exact names.
2. Paste SYSTEM_PROMPT.md into Claude or another browser-capable agent; keep production visible and sign in to VideoExpress yourself.
3. Send: "Start production of the bundled story, 16:9, 6 minutes" (examples/example-request.md).
4. Narration audio is made in app.clonevoice.ai (sign in there yourself): language Hindi, voice Neha Verma, the same voice for every narrator line.
5. The agent builds the 61 clips from examples/clip-prompts.md, adds the narration, hook, music and export.

## Files

- SYSTEM_PROMPT.md — the production agent prompt
- CHARACTER_BIBLE.md — identity locks, look-alike rules, dialogue and mouth rules
- DEITY_ICONOGRAPHY.md — how each god must look
- CHARACTER_SHEETS.md — prompts for the 7 sheets and 3 group images
- STYLE_BIBLE.md — look, sound, limits
- examples/example-request.md — paste-ready requests
- examples/story-sote-bhagwan-ko-jagane-wala-balak.md — the original 61-clip Hindi ledger, hook plan, YouTube title and description
- examples/clip-prompts.md — an image prompt and a video prompt for every clip
- evals/acceptance-checklist.md — acceptance checklist

## Known limits

- Audio cannot be heard by the agent; speech is checked by line length against clip seconds.
- VideoExpress clips can carry burned-in garbled captions; prompts never mention text and every clip is checked.
- Only two Reference Photo slots exist; scenes with more characters use the speaker and main listener, or a saved group image.
- Four-armed Vishnu and Shesh Naag (see FIELD_NOTES.md for the real hood count) can glitch; every clip is checked.
- The account may cap AI clips per day (about 150).

## Security

Never put passwords, tokens, API keys or payment data in this repository.
