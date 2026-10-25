# सोते भगवान को जगाने वाला बालक — Dev Uthani Ekadashi (original script)

Original Hindi script for the VideoExpress 3D bhakti-katha agent. 16:9, target **6 minutes**, 61 new clips plus a reused 4-clip hook. Cast: Tunnu (child hero), Guru Harisharan, Maa Lakshmi, Shesh Naag, Garud, Lord Vishnu, and an unseen narrator.

## Story line

Chaturmas has lasted four months, the ashram eats only plain khichdi, and hungry little Tunnu loses patience: he wants to wake the sleeping Vishnu himself. Guru Harisharan keeps repeating that Shri Hari will rise only on Ekadashi. Tunnu scolds the sky, and three visitors come to him in turn: Maa Lakshmi (the rule), Shesh Naag (the bed, who cannot move), and Garud (who finally carries Tunnu and the doubting Guru to Kshir Sagar). Each time Tunnu runs to the Guru, who does not believe him; the refrain "Ekadashi par hi uthenge" becomes a running joke Tunnu starts repeating himself. At Kshir Sagar, at first light on Dev Uthani Ekadashi, Tunnu scolds the sleeping Lord and sings the folk wake-up verse; Vishnu wakes, laughs lovingly, and Lakshmi hands out laddoos. The moral: God looks at sincere feeling, not at the clock.

## Pattern (as requested)

Tunnu scolds Vishnu → Guru: "Vishnu ji toh Ekadashi pe hi uthenge" → **Lakshmi ji** comes → Guru doubts → **Shesh Naag** comes → Guru doubts → **Garud** comes → Guru finally sees → **Vishnu wakes**.

## Fixed rules for this script

- Every dialogue line is spoken only by the character named in the "Speaker" column. Everyone else in the frame has a closed mouth.
- During every narrator (N) clip, every character's mouth is closed.
- Deities appear only in their real traditional form (DEITY_ICONOGRAPHY.md). The comedy comes from Tunnu's loving scolding and the Guru's disbelief; no deity is mocked.
- Deity visits happen in the ashram courtyard (Tunnu alone with the visitor, so only two characters in frame). The Guru never shares a frame with a deity until Garud lands (clip 37, when the Guru comes out to the courtyard) and the finale at Kshir Sagar.
- No subtitles in the final video.

## Locations

### A

Ashram courtyard layout (never mirror, never relocate): a raised white-and-terracotta Tulsi Vrindavan platform with one green tulsi plant at frame centre-right; a small mud-and-thatch ashram hut with a wooden door and one hanging brass bell at frame left; a huge banyan tree behind the hut at far left; a low stone wall at frame right with the glimmering Ganga river behind it; swept earth floor in the foreground; two clay diyas on the platform edge; no other people, no animals, no statues

### K

Kshir Sagar layout (never mirror, never relocate): an endless calm milk-white ocean; at frame centre the silver-white coils of Shesh Naag floating on the water with seven hoods fanned behind as a canopy, Lord Vishnu reclining on the coils with his head toward frame right and his feet toward frame left, Maa Lakshmi seated at his feet on frame left; a large round floating pink lotus platform in the foreground where visitors stand; giant pink-and-white lotuses on the water at far left; soft golden clouds and a pale horizon; no other beings

### F

Flight layout: Garud in flight travelling left to right across a pink-gold sunrise sky above soft clouds, body horizontal, wings spread; Tunnu sits in front near Garud's shoulders and Guru Harisharan sits behind him; no other birds, no other beings

## Hook plan (reuse only — no new generation)

Use these finished clips in this order at the very start: clip 10, clip 15, clip 29, clip 47 (about 23 s). Then the new narrator clip 1 (it asks viewers to subscribe), then clips 1–61 in order from the start. The hook clips stay in the story too.

## Ledger

Columns: # | T (N narrator, D dialogue) | Speaker (owner of the line) | Spoken to | Hindi line | chars | Set | In frame (silent, closed-mouth) | Shot | Clip s | Refs | Job ID | Status

Limits: dialogue ≤ 62 characters, narrator ≤ 90 characters (a 10 s clip at storytelling pace).

| # | T | Speaker | To | Hindi line | chars | Set | In frame | Shot | Clip s | Ref images (slot 1, slot 2) | Job | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | N | Narrator | - | दोस्तों, कहानी अच्छी लगे तो चैनल को सब्सक्राइब ज़रूर कीजिए। तो चलिए, कहानी शुरू करते हैं। **[subscribe line]** | 89 | A (late afternoon) | Tunnu, Guru Harisharan | W | 10 | GR-TG | | |
| 2 | N | Narrator | - | गंगा किनारे आश्रम में गुरुजी और नन्हा टुन्नू रहते थे। चातुर्मास के चार महीने बीत रहे थे। | 88 | A (late afternoon) | Tunnu, Guru Harisharan | M-shot: W, C | 10 | GR-TG | | |
| 3 | N | Narrator | - | इन दिनों न कोई उत्सव था, न भोग-प्रसाद। और टुन्नू के पेट में चूहे दौड़ रहे थे। | 77 | A (late afternoon) | Tunnu | C | 10 | TUNNU - Sheet | | |
| 4 | D | Tunnu | Guru Harisharan | ओहो! चार महीने से बस खिचड़ी, खिचड़ी और खिचड़ी! | 46 | A (late afternoon) | Guru Harisharan | M | 7 | TUNNU - Sheet + GURU HARISHARAN - Sheet | | |
| 5 | D | Guru Harisharan | Tunnu | चातुर्मास में विष्णु जी सोते हैं बेटा, सादा भोजन ही मिलेगा। | 59 | A (late afternoon) | Tunnu | M | 7 | GURU HARISHARAN - Sheet + TUNNU - Sheet | | |
| 6 | D | Tunnu | Guru Harisharan | तो भगवान को ही जगा देते हैं, गुरुजी! फिर लड्डू मिलेंगे। | 55 | A (late afternoon) | Guru Harisharan | C | 7 | TUNNU - Sheet + GURU HARISHARAN - Sheet | | |
| 7 | D | Guru Harisharan | Tunnu | अरे पगले! श्रीहरि तो एकादशी पर ही उठेंगे, उससे पहले नहीं। | 57 | A (late afternoon) | Tunnu | M | 7 | GURU HARISHARAN - Sheet + TUNNU - Sheet | | |
| 8 | D | Tunnu | Guru Harisharan | तब तक हम भूखे मर जाएँगे! मैं तो उन्हें डाँटूँगा! | 48 | A (late afternoon) | Guru Harisharan | C | 7 | TUNNU - Sheet + GURU HARISHARAN - Sheet | | |
| 9 | N | Narrator | - | शाम ढली। टुन्नू तुलसी चबूतरे पर पहुँचा और आसमान की ओर मुँह उठाकर बोला। | 70 | A (dusk) | Tunnu | W | 9 | TUNNU - Sheet | | |
| 10 | D | Tunnu | (sky, off-screen) | हे श्रीहरि! चार महीने से सो रहे हो, और यहाँ हम भूखे हैं! उठिए! **[HOOK-1]** | 62 | A (dusk) | — | C | 8 | TUNNU - Sheet | | |
| 11 | N | Narrator | - | तभी तुलसी के पास सुनहरी रोशनी फैली, और कमल पर माँ लक्ष्मी प्रकट हुईं। | 69 | A (dusk) | Tunnu, Maa Lakshmi | M-shot: W, C | 9 | TUNNU - Sheet + MAA LAKSHMI - Sheet | | |
| 12 | D | Maa Lakshmi | Tunnu | बेटा, इतना शोर क्यों? प्रभु तो योगनिद्रा में हैं। | 49 | A (dusk) | Tunnu | M | 7 | MAA LAKSHMI - Sheet + TUNNU - Sheet | | |
| 13 | D | Tunnu | Maa Lakshmi | माँ, आप ही प्रभु को उठा दीजिए ना! हम भूखे हैं! | 46 | A (dusk) | Maa Lakshmi | C | 7 | TUNNU - Sheet + MAA LAKSHMI - Sheet | | |
| 14 | D | Maa Lakshmi | Tunnu | नियम है बेटा, प्रभु एकादशी पर ही उठेंगे। थोड़ा धीरज रख। | 55 | A (dusk) | Tunnu | M | 7 | MAA LAKSHMI - Sheet + TUNNU - Sheet | | |
| 15 | D | Tunnu | Maa Lakshmi | नियम-नियम! माँ, नियम से पेट नहीं भरता, हमें लड्डू चाहिए! **[HOOK-2]** | 56 | A (dusk) | Maa Lakshmi | C | 7 | TUNNU - Sheet + MAA LAKSHMI - Sheet | | |
| 16 | N | Narrator | - | माँ लक्ष्मी मुस्कुराकर अंतर्धान हो गईं। टुन्नू भागा-भागा गुरुजी के पास पहुँचा। | 78 | A (dusk) | Tunnu, Maa Lakshmi | W | 10 | TUNNU - Sheet + MAA LAKSHMI - Sheet | | |
| 17 | D | Tunnu | Guru Harisharan | गुरुजी! माँ लक्ष्मी आई थीं! कहती हैं, प्रभु एकादशी पर उठेंगे! | 61 | A (night, diya light) | Guru Harisharan | C | 8 | TUNNU - Sheet + GURU HARISHARAN - Sheet | | |
| 18 | D | Guru Harisharan | Tunnu | हा हा! सपना देखा होगा। चल सो जा, प्रभु एकादशी पर ही उठेंगे। | 59 | A (night, diya light) | Tunnu | M | 7 | GURU HARISHARAN - Sheet + TUNNU - Sheet | | |
| 19 | N | Narrator | - | अगली रात चाँदनी में आँगन की धरती हिली, और सात फनों वाले शेषनाग जी प्रकट हुए। | 76 | A (moonlit night) | Tunnu, Shesh Naag | M-shot: W, C | 10 | TUNNU - Sheet + SHESH NAAG - Sheet | | |
| 20 | D | Tunnu | Shesh Naag | अरे बाप रे! नमस्ते शेषनाग जी, आप तो प्रभु के बिस्तर हैं ना? | 59 | A (moonlit night) | Shesh Naag | C | 7 | TUNNU - Sheet + SHESH NAAG - Sheet | | |
| 21 | D | Shesh Naag | Tunnu | हाँ बालक, चार महीने से प्रभु मेरे ही ऊपर सो रहे हैं। | 52 | A (moonlit night) | Tunnu | M | 7 | SHESH NAAG - Sheet + TUNNU - Sheet | | |
| 22 | D | Tunnu | Shesh Naag | तो आप ज़रा हिल जाइए, प्रभु अपने आप जाग जाएँगे! | 46 | A (moonlit night) | Shesh Naag | C | 7 | TUNNU - Sheet + SHESH NAAG - Sheet | | |
| 23 | D | Shesh Naag | Tunnu | हा हा! मैं हिला तो पूरा क्षीरसागर हिल जाएगा, बालक। | 50 | A (moonlit night) | Tunnu | M | 7 | SHESH NAAG - Sheet + TUNNU - Sheet | | |
| 24 | D | Tunnu | Shesh Naag | तो फिर प्रभु कब जागेंगे? | 24 | A (moonlit night) | Shesh Naag | C | 7 | TUNNU - Sheet + SHESH NAAG - Sheet | | |
| 25 | D | Shesh Naag | Tunnu | प्रभु की नींद ऐसे नहीं टूटती। एकादशी की भोर तक रुको। | 52 | A (moonlit night) | Tunnu | M | 7 | SHESH NAAG - Sheet + TUNNU - Sheet | | |
| 26 | N | Narrator | - | शेषनाग जी आशीर्वाद देकर चले गए। टुन्नू फिर गुरुजी के पास दौड़ा। | 63 | A (moonlit night) | Tunnu, Shesh Naag | W | 8 | TUNNU - Sheet + SHESH NAAG - Sheet | | |
| 27 | D | Tunnu | Guru Harisharan | गुरुजी! अबकी शेषनाग जी आए थे, सात फनों वाले! सच्ची! | 51 | A (night, diya light) | Guru Harisharan | C | 7 | TUNNU - Sheet + GURU HARISHARAN - Sheet | | |
| 28 | D | Guru Harisharan | Tunnu | सात फन? अब कहानी बना रहा है! प्रभु एकादशी पर ही उठेंगे। | 55 | A (night, diya light) | Tunnu | M | 7 | GURU HARISHARAN - Sheet + TUNNU - Sheet | | |
| 29 | D | Tunnu | Guru Harisharan | एकादशी पर ही उठेंगे... सब यही रट लगाए बैठे हैं! **[HOOK-3]** | 47 | A (night, diya light) | Guru Harisharan | C | 7 | TUNNU - Sheet + GURU HARISHARAN - Sheet | | |
| 30 | N | Narrator | - | तीसरी सुबह आसमान में तेज़ हवा चली और पंख फैलाए गरुड़ जी आँगन में उतर आए। | 72 | A (early dawn) | Tunnu, Garud | M-shot: W, C | 9 | TUNNU - Sheet + GARUD - Sheet | | |
| 31 | D | Tunnu | Garud | वाह! गरुड़ जी! प्रभु के वाहन! मुझे अपनी पीठ पर घुमाओगे? | 55 | A (early dawn) | Garud | C | 7 | TUNNU - Sheet + GARUD - Sheet | | |
| 32 | D | Garud | Tunnu | बालक, मैं प्रभु का संदेश लाया हूँ, सैर कराने नहीं। | 50 | A (early dawn) | Tunnu | M | 7 | GARUD - Sheet + TUNNU - Sheet | | |
| 33 | D | Tunnu | Garud | तो प्रभु से कहिए, चार महीने बहुत होते हैं! | 42 | A (early dawn) | Garud | C | 7 | TUNNU - Sheet + GARUD - Sheet | | |
| 34 | D | Garud | Tunnu | प्रभु तो एकादशी की भोर में ही उठते हैं, बालक। | 45 | A (early dawn) | Tunnu | M | 7 | GARUD - Sheet + TUNNU - Sheet | | |
| 35 | D | Tunnu | Garud | लगता है आप सब आपस में मिले हुए हैं! | 35 | A (early dawn) | Garud | C | 7 | TUNNU - Sheet + GARUD - Sheet | | |
| 36 | D | Garud | Tunnu | हा हा! चलो, तुम्हें और तुम्हारे गुरु को प्रभु के पास ले चलूँ। | 61 | A (early dawn) | Tunnu | M | 8 | GARUD - Sheet + TUNNU - Sheet | | |
| 37 | D | Tunnu | Guru Harisharan | गुरुजी चलिए! गरुड़ जी हमें प्रभु के पास ले जा रहे हैं! | 54 | A (early dawn) | Guru Harisharan, Garud | M | 7 | TUNNU - Sheet + GURU HARISHARAN - Sheet | | |
| 38 | D | Guru Harisharan | Garud | हे नारायण! ये तो सचमुच गरुड़ देव हैं! टुन्नू, तू सच कह रहा था! | 62 | A (early dawn) | Tunnu, Garud | C | 8 | GURU HARISHARAN - Sheet + GARUD - Sheet | | |
| 39 | D | Garud | Guru Harisharan | गुरुवर, मेरी पीठ पर बैठिए, यात्रा तेज़ है। | 42 | A (early dawn) | Tunnu, Guru Harisharan | M | 7 | GARUD - Sheet + GURU HARISHARAN - Sheet | | |
| 40 | D | Guru Harisharan | Tunnu | टुन्नू बेटा, मेरा हाथ मत छोड़ना! | 32 | A (early dawn) | Tunnu, Garud | C | 7 | GURU HARISHARAN - Sheet + TUNNU - Sheet | | |
| 41 | N | Narrator | - | गरुड़ जी ने पंख फैलाए और आकाश चीरते हुए क्षीरसागर की ओर उड़ चले। | 64 | F (flight, sunrise sky) | Tunnu, Guru Harisharan, Garud | M-shot: W, C, W | 8 | GR-FLIGHT | | |
| 42 | D | Tunnu | Guru Harisharan | गुरुजी, देखिए! बादल कितने नीचे हैं! मज़ा आ गया! | 47 | F (flight, sunrise sky) | Guru Harisharan, Garud | C | 7 | GR-FLIGHT | | |
| 43 | D | Guru Harisharan | Tunnu | आँखें बंद हैं बेटा, तू ही बता कब उतरेंगे। | 41 | F (flight, sunrise sky) | Tunnu, Garud | C | 7 | GR-FLIGHT | | |
| 44 | N | Narrator | - | सामने था क्षीरसागर, जहाँ श्रीहरि योगनिद्रा में थे और माँ लक्ष्मी उनके चरण दबा रही थीं। | 86 | K (pre-dawn) | Tunnu, Guru Harisharan, Maa Lakshmi, Shesh Naag, Lord Vishnu | M-shot: W, C | 10 | GR-K + GR-TG | | |
| 45 | D | Tunnu | Lord Vishnu | प्रभु! उठिए! चार महीने हो गए, हम खिचड़ी खा-खाकर थक गए! | 54 | K (pre-dawn) | Guru Harisharan, Maa Lakshmi, Lord Vishnu | C | 7 | TUNNU - Sheet + GR-K | | |
| 46 | D | Maa Lakshmi | Tunnu | धीरे बेटा, प्रभु गहरी योगनिद्रा में हैं। | 40 | K (pre-dawn) | Tunnu, Lord Vishnu | M | 7 | MAA LAKSHMI - Sheet + TUNNU - Sheet | | |
| 47 | D | Tunnu | Maa Lakshmi | उठिए ना प्रभु, वरना मैं आपकी शिकायत माँ लक्ष्मी से कर दूँगा! **[HOOK-4]** | 60 | K (pre-dawn) | Maa Lakshmi, Lord Vishnu | C | 7 | TUNNU - Sheet + GR-K | | |
| 48 | D | Maa Lakshmi | Tunnu | बेटा, शिकायत मुझसे ही कर रहा है? मैं तो यहीं बैठी हूँ! | 54 | K (pre-dawn) | Tunnu, Lord Vishnu | M | 7 | MAA LAKSHMI - Sheet + TUNNU - Sheet | | |
| 49 | D | Shesh Naag | Tunnu | बालक, सूर्योदय होने वाला है। एक सच्चा गीत गाकर पुकारो। | 54 | K (pre-dawn) | Tunnu, Guru Harisharan, Maa Lakshmi, Lord Vishnu | M | 7 | SHESH NAAG - Sheet + TUNNU - Sheet | | |
| 50 | D | Tunnu | Lord Vishnu | उठो देव, बैठो देव, अंगुरिया चटकाओ देव! | 38 | K (first light) | Maa Lakshmi, Lord Vishnu | C | 7 | TUNNU - Sheet + GR-K | | |
| 51 | N | Narrator | - | सूरज की पहली किरण छूते ही प्रभु की पलकें हिलीं, और पूरा क्षीरसागर जगमगा उठा। | 76 | K (sunrise) | Tunnu, Guru Harisharan, Maa Lakshmi, Shesh Naag, Lord Vishnu | M-shot: C, W, C | 10 | GR-K + GR-TG | | |
| 52 | D | Lord Vishnu | Tunnu | किसने इतने प्यार से पुकारा मुझे? कौन है यह नन्हा बालक? | 54 | K (sunrise) | Tunnu, Maa Lakshmi | C | 7 | LORD VISHNU - Sheet + TUNNU - Sheet | | |
| 53 | D | Tunnu | Lord Vishnu | प्रभु, मैं टुन्नू हूँ! आपने चार महीने सोकर हमें भूखा रखा! | 57 | K (sunrise) | Maa Lakshmi, Lord Vishnu | C | 7 | TUNNU - Sheet + LORD VISHNU - Sheet | | |
| 54 | D | Lord Vishnu | Tunnu | आज देव उठनी एकादशी है, बालक। तेरी पुकार ठीक समय पर पहुँची। | 58 | K (sunrise) | Tunnu, Maa Lakshmi | M | 7 | LORD VISHNU - Sheet + TUNNU - Sheet | | |
| 55 | D | Maa Lakshmi | Tunnu | टुन्नू, ये लो प्रसाद। आज से सारे मंगल काम और भोज शुरू! | 54 | K (sunrise) | Tunnu, Lord Vishnu | M | 7 | MAA LAKSHMI - Sheet + TUNNU - Sheet | | |
| 56 | D | Tunnu | Maa Lakshmi | इतने लड्डू! अब गुरुजी का हिस्सा भी मैं ही खा लूँगा! | 51 | K (sunrise) | Guru Harisharan, Maa Lakshmi, Lord Vishnu | C | 7 | TUNNU - Sheet + MAA LAKSHMI - Sheet | | |
| 57 | D | Guru Harisharan | Tunnu | अरे! मेरे हिस्से के लड्डू तो छोड़ दे, पगले! | 43 | K (sunrise) | Tunnu, Lord Vishnu | M | 7 | GURU HARISHARAN - Sheet + TUNNU - Sheet | | |
| 58 | D | Lord Vishnu | Tunnu | याद रखना, भगवान समय नहीं, सच्चा भाव देखकर जागते हैं। **[moral]** | 52 | K (sunrise) | Tunnu, Guru Harisharan, Maa Lakshmi | M | 7 | LORD VISHNU - Sheet + TUNNU - Sheet | | |
| 59 | N | Narrator | - | उसी दिन आश्रम में तुलसी विवाह की धूम मची, और पूरे गाँव में मंगल गीत गूँजे। | 74 | A (festive morning, diyas) | Tunnu, Guru Harisharan | M-shot: W, C | 9 | GR-TG | | |
| 60 | D | Tunnu | Guru Harisharan | गुरुजी, अगले चातुर्मास में मैं लड्डू पहले ही छुपाकर रखूँगा! **[final gag]** | 59 | A (festive morning, diyas) | Guru Harisharan | C | 7 | TUNNU - Sheet + GURU HARISHARAN - Sheet | | |
| 61 | N | Narrator | - | तो दोस्तों, भगवान भाव के भूखे हैं। बोलिए, देव उठनी एकादशी की जय! **[closing]** | 64 | A (festive morning, diyas) | Tunnu, Guru Harisharan | W | 8 | GR-TG | | |

Estimated length: story clips ≈ 347 s (speech plus about one second per clip, before trimming) plus the reused hook ≈ 23 s. After trimming each clip to its speech and leaving about half a second between clips this lands near 6 minutes. Measure the real runtime after assembly; if it is under 5:45 or over 6:15, say so in the report.

## YouTube title and description

**Title:** सोते भगवान को जगाने वाला बालक | Dev Uthani Ekadashi Katha | 3D भक्ति कथा

**Description:** चार महीने से सोते भगवान विष्णु को जगाने निकला नन्हा टुन्नू! देव उठनी एकादशी की यह मज़ेदार और भावुक कहानी देखिए, जिसमें माँ लक्ष्मी, शेषनाग जी और गरुड़ जी भी आते हैं। कहानी अच्छी लगे तो चैनल को सब्सक्राइब करें। #DevUthaniEkadashi #BhaktiKatha #3DAnimation #LordVishnu #HindiKahani
