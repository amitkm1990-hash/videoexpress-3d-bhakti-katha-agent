# Style bible — what the reference video looks like and how to reproduce the format

Reference studied: https://www.youtube.com/watch?v=0gatfAoic-0 (a 40 min 45 s Hindi 3D devotional "Bhakti Katha", published 16 Oct 2026). This file records what was observed and what was not. Nothing from the video (characters, names, lines, logo, music) is reused in this repo.

## How it was studied

- The full Hindi caption transcript (about 300 timed segments) was read from start to end in the browser, giving the script structure, language, pacing and the narrator/dialogue mix.
- Frames were captured at about 2:20, 12:05, 27:45, 36:15 and 37:15 in the player, and the player's own subtitle rendering was checked. Two other seeks landed on ads and were discarded, so the frame study is a sample, not every scene.
- Audio could not be heard, so voices, accents and music are inferred from the captions ([संगीत], [हंसी], [चीखने की आवाज़] markers) and from mouth shapes in the frames. Do not treat voice guidance as measured.
- The player ran at 854×480; export at Full HD anyway.

## Visual style (observed)

- Pixar-style 3D animation: smooth sculpted faces, soft global illumination, saturated colour, golden daylight, creamy depth-of-field blur behind the characters.
- Children have oversized heads and huge glossy eyes (toddler-like proportions); the hero is a small round-faced boy with a tuft, tilak and bead necklaces. The old guru is a slim elder with a long white beard and saffron robe. Deities (Krishna, Shiva) are drawn youthful and soft with large eyes, traditional crowns, garlands, peacock feather, trident, damaru and snake, in the same 3D look.
- Settings: a lush green forest with sunlight through the leaves and wildflowers in the foreground, a river bank at sunrise, an ashram, a forest clearing with a clay chulha and cows in the background.
- Camera: medium and medium close-up shots of the speaker; over-the-shoulder shots with the listener's back of head blurred in the foreground; wide shots for arrivals; calm, mostly static or slow push-in.
- On-screen text: Hindi subtitles in white bold Devanagari with a dark outline, two short lines, near the bottom; a small round channel emblem in the bottom-right corner.

## Script and language (observed)

- Language: Hindi, simple and conversational, with village words (ठाकुर, बाबा जी, बालक, पुत्र). The hero is blunt and funny; the elders and deities answer calmly.
- Structure: a teaser of three or four later lines → a friendly narrator intro to the audience ("दोस्तों ... चलो बिना देरी किए शुरू करते हैं") → setup at a river and an ashram → the hero's nickname joke (a unit of food) → the ashram's fasting rule and a negotiation → five repeats of the same visit (the hero cooks alone, calls the deity, a guest arrives, eats everything, leaves; the hero tells the guru; the guru does not believe) → the quantity of food and the number of guests grow each repeat → on the last repeat the hero makes the guests work → a new deity arrives with an entourage → the hero drags the guru to see → the guru weeps and thanks him.
- Narrator: a storyteller voice describes scenes and transitions between dialogue ("कुछ दिन बाद ... एकादशी आ गई"). Dialogue clips carry the comedy; narrator clips carry time, place and action.
- Pace: about 2 narrator lines for every 4–5 dialogue lines, many short lines of 3–8 seconds, a [संगीत] bed under almost every scene.
- Lip-sync: only the speaker's mouth moves; the listener stays in frame or at the frame edge.

## Rules this repo adds on top

- The story is original; only the format is borrowed.
- Deities are shown reverently; humour comes from the child hero's loving grumbling, not from the deities. (The reference lets the hero scold the gods; this repo keeps that spirit but makes sure the gods are never the target of a joke.)
- Subtitles and the emblem are added in the editor, never drawn by the video model.
- One speaker per clip, with silent listeners in frame, and a narrator track that is a single consistent voice.

## Known limits

- VideoExpress clips sometimes carry burned-in garbled captions. The prompt never mentions text and every clip is checked.
- Only two Reference Photo slots exist, so scenes with three or more characters use group reference images.
- The video model may move non-speakers' mouths, add extra characters or turn a speaker's back to the camera; every clip is checked.
- Deities with four or more arms may glitch; this repo uses the simplified two-armed cartoon form and checks each face.
