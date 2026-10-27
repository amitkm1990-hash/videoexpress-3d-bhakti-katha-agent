# Character bible — identity locks

These locks are the single source of truth. Paste the lock text for every character in the frame **word for word** into every image prompt. Never paraphrase, shorten or improve a lock. The locks describe the exact images the user saved in VideoExpress "My AI Images" (see CHARACTER_SHEETS.md); if a lock and a saved image ever disagree, the saved image wins and the lock is corrected before use.

| Code | Character | Role | Voice |
|---|---|---|---|
| N | Narrator (never seen) | storyteller | app.clonevoice.ai, language Hindi, voice Neha Verma, calm storytelling cadence |
| T | Tunnu (टुन्नू) | 7-year-old child hero | bright, cheeky, high child voice |
| G | Guru Harisharan (गुरुजी) | the guru | calm, slightly raspy elder voice |
| R | Garud (गरुड़ जी) | divine eagle | strong, proud, clear heroic voice |
| L | Maa Lakshmi (माँ लक्ष्मी) | goddess | soft, warm, motherly female voice |
| S | Shesh Naag (शेषनाग जी) | divine serpent | very deep, slow, soothing voice |
| V | Lord Vishnu (Shri Hari) (श्रीहरि) | deity | deep, calm, resonant, kind voice |

## Identity locks

### T — Tunnu

Saved image name: `TUNNU - Sheet`

```
Tunnu: a 7-year-old Indian boy in chibi proportions (head about 40% of body height), huge round glossy brown eyes with highlights, round cheeks, small nose, shaved head with one small black tuft (shikha) on top, white U-shaped Vaishnav tilak with a red centre line, bright grass-green short kurta with a thin gold border, white dhoti-style shorts, a single tulsi-bead necklace, bare feet, exactly two arms and two hands
```

### G — Guru Harisharan

Saved image name: `GURU HARISHARAN - Sheet`

```
Guru Harisharan: a slim elderly Indian sage, normal adult proportions, bald head with a small white tilak, long straight white beard down to the chest, kind wrinkled eyes, saffron dhoti and a saffron shoulder-cloth, one tulsi mala around the neck, wooden sandals, exactly two arms and two hands
```

### R — Garud

Saved image name: `GARUD - Sheet`

```
Garud: a divine eagle-man, human torso and legs with a golden eagle face and curved golden beak, kind bright eyes, a small gold crown, two huge red-and-gold feathered wings, red-orange body with gold armlets and a necklace, yellow dhoti, exactly two arms and two hands plus two wings
```

### L — Maa Lakshmi

Saved image name: `MAA LAKSHMI - Sheet`

```
Maa Lakshmi: goddess in traditional devotional-poster form, adult proportions, golden-fair glowing complexion, serene smiling face with lotus-shaped eyes, deep red silk saree with a wide golden border, jewelled golden crown, gold necklace, earrings, bangles and waist belt, a pink lotus in her right hand, left hand in blessing pose or pressing the Lord's feet, exactly two arms and two hands, no elephants, no coins
```

### S — Shesh Naag

Saved image name: `SHESH NAAG - Sheet`

```
Shesh Naag: a giant silver-white divine serpent with EXACTLY SEVEN fanned cobra hoods; the large central hood has one kind, wise face with gentle ruby-red eyes and a small golden crown, the six other hoods are smooth plain cobra hoods without faces, gold jewellery on the hoods, a pearly white body in thick coils; only the central face ever speaks
```

### V — Lord Vishnu (Shri Hari)

Saved image name: `LORD VISHNU - Sheet`

```
Lord Vishnu: deity in traditional devotional-poster form, adult proportions, deep cloud-blue skin (megha-shyam), serene half-closed lotus eyes and a gentle smile, no beard, EXACTLY FOUR ARMS: upper right hand holds the spinning Sudarshan chakra on the finger, upper left hand holds the white Panchajanya conch, lower right hand holds a pink lotus, lower left hand holds the golden mace; tall golden crown (kirit), makara earrings, red-and-white U-shaped Vaishnav tilak, Kaustubh gem and a long vaijayanti flower garland on the chest with the Shrivatsa mark, yellow pitambar dhoti, golden armlets and bracelets, bare chest
```

## Look-alike rule (why the cast is built this way)

Past videos showed several copies of one character in a single scene. This cast is designed so that no two characters can be confused, and the rules below stop copies:

- Every character has its own silhouette and one dominant colour: Tunnu green and tiny, Guru saffron with a white beard, Lakshmi red and gold, Vishnu cloud-blue and yellow, Shesh silver-white serpent, Garud red-gold with wings.
- **One head per character per frame.** Before every submit, count the characters in the ledger row (its census) and write the exact number in the prompt: "exactly N characters in the image, nobody else".
- **Census check after generation.** Look at the start, middle and end frames of every clip and count heads. One extra Tunnu, a second Guru, a second Vishnu or a Garud twin means the clip is rejected and regenerated.
- **No second Vishnu, ever.** No statue, idol, painting, mirror image, reflection in water, shadow figure or poster of any deity may appear in a frame. The only Vishnu in any frame is the real one.
- **No crowds.** No villagers, no extra sages, no animals, no extra Brahmins. Only the cast.
- **Shesh Naag is one serpent.** The seven hoods are one being. Only the large central hood has a face; if the model gives all seven hoods faces, regenerate.
- **Only saved images are used.** The agent never invents, redraws or "improves" a character. If a sheet is missing, it stops and asks for it.
- **Reference slots.** Two slots only. Use the speaker's saved image plus the main listener's saved image. Never put the same character in both slots, and never use a group reference that contains a character already in the other slot. Other characters in the frame are named in the prompt with their identity lock text.

## Dialogue ownership and mouth rule

- Every line belongs to exactly one speaker, named in the ledger. **Only that character speaks that line.** No other character may speak, mouth words or move lips during it.
- **Every other character in the frame keeps a fully closed mouth** (lips pressed together) for the entire clip.
- **During every narrator clip, every character's mouth stays fully closed.** Nobody on screen speaks while the narrator narrates; characters only do small actions that match the narration.
- Shesh Naag's lines are spoken only by his central hood-face; Garud speaks only through his beak with the mouth shapes of speech; the sleeping Vishnu keeps eyes and mouth closed until the awakening clip.
- A clip where a non-speaker's lips move, or a line is spoken by the wrong character, is rejected and regenerated (simpler pose, listener moved to the frame edge, or the line made a solo shot of the speaker).

---

# Bhai Dooj pack — "भैया दूज पर यमराज की बहन" (added)

The locks above belong to the Dev Uthani pack and are unchanged. This pack has its own cast. The same rules apply: paste each lock **word for word** into every image prompt that contains that character; the saved image wins if lock and image ever disagree.

| Code | Character name (used everywhere) | Role | Voice |
|---|---|---|---|
| N | Narrator (never seen) | storyteller | app.clonevoice.ai, language Hindi, voice Neha Verma, calm storytelling cadence |
| J | Jamuni (जमुनी) | 7-year-old little-sister hero | sweet, bright, brave little girl |
| B | Bholu (भोलू) | 10-year-old elder brother | playful, cheeky young boy |
| A | Acharya Somdutt (आचार्य सोमदत्त) | the doubting guru | gruff, booming, slightly pompous elder |
| C | Chitragupt ji (चित्रगुप्त जी) | scribe of the gods, first guest | quick, polite, courteous middle-aged |
| Y | Yamraj ji (यमराज जी) | god of death, second and main guest | very deep, slow, grave yet kind |

## Identity locks (Bhai Dooj pack)

### J — Jamuni

Saved image name: `JAMUNI - Sheet`

```
Jamuni: a 7-year-old Indian girl in chibi proportions (head about 40% of body height), huge round glossy dark-brown eyes with highlights, round cheeks, small nose, a small red bindi, two long black braids tied with marigold-orange ribbons, turquoise-blue lehenga-choli with a thin silver border and a matching turquoise dupatta, silver bangles and silver anklets, bare feet, exactly two arms and two hands
```

### B — Bholu

Saved image name: `BHOLU - Sheet`

```
Bholu: a 10-year-old Indian boy in chibi proportions (head about 35% of body height, a little taller than Jamuni), huge round glossy brown eyes with highlights, round cheeks, short messy black hair, bright mustard-yellow kurta with a brown border, cream pyjama-style trousers, a thin red kalawa thread on the right wrist, bare feet, exactly two arms and two hands
```

### A — Acharya Somdutt

Saved image name: `ACHARYA SOMDUTT - Sheet`

```
Acharya Somdutt: a stout elderly Indian guru, normal adult proportions, bald head with a small white topknot (choti), thick round black-rimmed glasses, bushy white moustache and a short white beard, maroon kurta with a cream shoulder-cloth, white dhoti, a rudraksha mala around the neck, wooden sandals, exactly two arms and two hands
```

### C — Chitragupt ji

Saved image name: `CHITRAGUPT - Sheet`

```
Chitragupt ji: a slim middle-aged Indian scribe-deity, normal adult proportions, wheatish skin, kind round face with a thin black moustache, a tall yellow-and-white turban, yellow kurta with a white dhoti and a white shoulder-cloth, a thick red cloth-bound ledger (bahi-khata) held in his left hand and a long feather pen in his right hand, gold earrings, exactly two arms and two hands
```

### Y — Yamraj ji

Saved image name: `YAMRAJ - Sheet`

```
Yamraj ji (Lord Yama): deity in traditional devotional-poster form, adult proportions, deep dark blue-green complexion, dignified kind face with large calm eyes and a thick black moustache, tall golden crown with two small curved horns, crimson-red royal robe with a golden border, golden shoulder armour, gold necklace, armlets and bracelets, a golden danda (staff) in his right hand and his left hand raised in blessing (abhaya mudra), exactly two arms and two hands, no noose, no weapon pointed at anyone, no buffalo in the frame
```

## Look-alike separation (Bhai Dooj pack)

- Jamuni is tiny, turquoise-blue, with two braids and orange ribbons. Bholu is taller, mustard-yellow, with short messy hair. They are never confused and never drawn twice.
- Acharya Somdutt is stout with glasses, a white moustache and a maroon kurta. Yamraj ji is dark blue-green with a crimson robe and a horned golden crown. Chitragupt ji is slim with a yellow-and-white turban and a red ledger.
- Exactly one head per character per frame; the census in the ledger row is written into every image prompt as "Exactly N characters in the image, each appearing once, nobody else".
- No buffalo, no statues, no extra villagers, no crowd, no second Yamraj, no second Chitragupt, no reflection or shadow figure of any deity.
- Every line has one owner; every other mouth is fully closed; during narrator clips every mouth is closed.
