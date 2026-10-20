# VideoExpress Pixar-Style 3D Hindi Bhakti-Katha Agent

A system prompt for producing 8-minute-and-up Hindi devotional story videos in VideoExpress.ai in the format of a popular 3D "Bhakti Katha" channel: Pixar-style 3D characters, golden-light forests and ghats, a warm storyteller narrator, short comic lip-synced dialogue, Hindi subtitles, soft background music, and a funny repeating visit-pattern in which a hungry, innocent child devotee lovingly scolds the gods and finally leads his doubting guru to see them.

Format direction comes from a start-to-end study of https://www.youtube.com/watch?v=0gatfAoic-0 (see STYLE_BIBLE.md for what was observed and what could not be, such as audio). The story, characters, setting, numbers and lines in this repo are original.

## What changed from the earlier agents

| Topic | 2D devotional kids' agent | This agent |
| --- | --- | --- |
| Look | 2D flat-cel chibi, pastel paint | Pixar-style 3D, soft global illumination, golden-light forests, blurred backgrounds |
| Image Type | 2D | 3D |
| Voice | No narrator, only on-screen speakers | Narrator voice-over plus one on-screen lip-synced speaker per dialogue clip |
| Story | Short moral story | Repeating visit pattern with escalation, doubting guru, final reveal, deity-spoken moral |
| Deities | Only when asked, solo clips | Speaking guests with short reverent lines; never the butt of a joke |
| Hook | None | 30–40 s teaser re-using finished clips, then a narrator intro |
| Length | about 6 min | about 8 min default; longer videos split into Parts |
| Subtitles | Editor text layer | Same; Hindi, white with dark outline, bottom centre |

## Use

1. Open SYSTEM_PROMPT.md and paste the whole prompt into Claude or another browser-capable agent.
2. Enable its supported browser control and keep production visible. Sign in to VideoExpress yourself.
3. Send a topic, deity or moral, or point at the sample script, as shown in examples/example-request.md.
4. The agent builds characters, references, clips, voice-over, the timeline, then saves and exports.

## Contents

- SYSTEM_PROMPT.md — the production agent prompt
- STYLE_BIBLE.md — what the reference video looks like and how the format is reproduced
- examples/example-request.md — paste-ready requests
- examples/story-adhaiya-ki-chaturthi.md — an original 96-clip Hindi script "अढ़ैया की चतुर्थी" with story line, cast, set layouts, narration, hook plan, full ledger, sample prompts and a YouTube title and description
- evals/acceptance-checklist.md — production acceptance checklist

## Known limits

- Audio could not be heard during the study; voice guidance is inferred from captions and frames.
- VideoExpress clips sometimes carry burned-in garbled captions; the prompt never mentions text and every clip is checked.
- Only two Reference Photo slots exist, so crowded scenes use group reference images.
- The account may cap AI clips per day (about 150); long videos are split into Parts.
- The narrator can be made by editor voice-over (Route A) or inside the clip (Route B); Route B can drift in voice.

## Security

Never put passwords, tokens, API keys, payment data or browser session data in this repository.
