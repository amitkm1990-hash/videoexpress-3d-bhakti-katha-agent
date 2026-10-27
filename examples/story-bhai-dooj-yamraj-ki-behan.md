# भैया दूज पर यमराज की बहन — Bhai Dooj (original script)

Original Hindi script for the VideoExpress 3D bhakti-katha agent. 16:9, Pixar-style 3D, target about **6 minutes**, 48 new clips plus a reused 4-clip hook. Bhai Dooj 2026 is on 11 November. Cast: Jamuni (little sister hero), Bholu (her brother), Acharya Somdutt (the doubting guru), Yamraj ji, Chitragupt ji, and an unseen narrator.

## Story line

The Acharya reads Bholu's kundli and warns that Yamraj's eye is on him this year. Little Jamuni will not accept it: like Yamuna ji, who once invited her brother Yamraj to her home, she goes to the Yamuna ghat and invites Yamraj for Bhai Dooj lunch. On Bhai Dooj morning Chitragupt ji arrives first as a guest to check the accounts; Jamuni feeds him first and asks him to write her brother's name among the punya. The Acharya does not believe her and calls it a dream. At noon Yamraj ji himself arrives with Chitragupt ji, the Acharya sees them with his own eyes, Jamuni applies the tilak to Yamraj and asks only that her brother never come under his gaze. Yamraj grants the boon: the brother who gets tilak from his sister on this day will not fear death. Jamuni applies tilak to Bholu, Chitragupt ji writes *deerghayu bhava* in his ledger, the Acharya apologises, and everyone eats puri-halwa. Moral: a sister's love is the greatest protective shield.

## Pattern (as requested)

Jamuni, like Yamuna ji, comes to save her brother from Yamraj → the Acharya doubts → **Chitragupt ji** comes as a guest first → the Acharya doubts again → **Yamraj ji** comes as a guest → the Acharya finally sees → tilak, boon, feast.

## Character name registry (these exact names are used in every ledger row and every prompt)

| Code | Name used in ledger and prompts | Reference image used in every clip | 3-view sheet (look reference only) | Voice for dialogue |
|---|---|---|---|---|
| J | Jamuni (जमुनी) | `JAMUNI - Single` | `JAMUNI - Sheet` | sweet, bright, brave little girl (clonevoice Hindi, Priya Mehra) |
| B | Bholu (भोलू) | `BHOLU - Single` | `BHOLU - Sheet` | playful, cheeky young boy (clonevoice Hindi, Aditya Gupta) |
| A | Acharya Somdutt (आचार्य सोमदत्त) | `ACHARYA SOMDUTT - Single` | `ACHARYA SOMDUTT - Sheet` | gruff, booming, slightly pompous elder (clonevoice Hindi, Rajesh Malhotra) |
| C | Chitragupt ji (चित्रगुप्त जी) | `CHITRAGUPT - Single` | `CHITRAGUPT - Sheet` | quick, polite, courteous middle-aged (clonevoice Hindi, Varun Mehta) |
| Y | Yamraj ji (यमराज जी) | `YAMRAJ - Single` | `YAMRAJ - Sheet` | very deep, slow, grave yet kind (clonevoice Hindi, Vikram Khanna) |
| N | Narrator (never seen) | - | - | app.clonevoice.ai, language Hindi, voice Neha Verma |

## Fixed rules for this script

- Every dialogue line is spoken only by the character named in the **Speaker** column. Everyone else in the frame keeps a fully closed mouth.
- During every narrator (N) clip, every character's mouth is closed.
- One copy of each character per frame; the census column is the exact head count and is written into every image prompt. No twin of Jamuni or Bholu (they differ in colour and height), no extra villagers, no animals, no buffalo, no statues.
- Yamraj ji and Chitragupt ji appear only in their traditional, dignified forms (DEITY_ICONOGRAPHY.md), as respected guests. They are never mocked, made foolish, angry or scary. The comedy comes from Jamuni's loving bossiness, Bholu's greed for sweets and the Acharya's disbelief.
- No subtitles in the final video. Never write subtitle, caption or text words in a video prompt.
- **Subscribe clip, then comment-line clip** (clips 1 and 2): the narrator asks viewers to subscribe and then to write the name of the deity of this video in the comments: *जय यमुना मैया, जय यमराज जी*.

## Locations

### H

Village courtyard layout (never mirror, never relocate): a small terracotta-and-white village house with a red wooden door at frame left; one large neem tree behind the roof at far left; a square marigold-petal rangoli at frame centre in the foreground; a low wooden chowki with a puja thali, one clay diya and a small bowl of roli at frame centre-right; a low mud wall at frame right with the glimmering Yamuna river behind it; swept earth floor; no other people, no animals, no statues

### G

Yamuna ghat layout (never mirror, never relocate): wide stone steps leading down to the calm turquoise Yamuna river at frame centre; one large banyan tree on the steps at frame left; two small floating diyas on the water at frame right; soft mist; no other people, no animals, no statues

## Hook plan (reuse only, no new generation)

Use these finished clips in this order at the very start: clip 10, clip 14, clip 21, clip 37 (about 30 s). Then the new narrator clip 1 (subscribe), then clip 2 (comment line), then clips 3 onward in order from the start. The hook clips stay in the story too.

## Ledger

Columns: # | T (N narrator, D dialogue) | Speaker (owner of the line) | Spoken to | Hindi line | chars | Set | In frame (head count, listeners keep mouths closed) | Shot | Clip s | Ref images (slot 1, slot 2) | Job | Status

Limits: dialogue ≤ 62 characters, narrator ≤ 90 characters.

| # | T | Speaker | To | Hindi line | chars | Set | In frame | Shot | Clip s | Ref images | Job | Status |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | N | Narrator | - | दोस्तों, कहानी अच्छी लगे तो चैनल को सब्सक्राइब ज़रूर कीजिए। **[subscribe]** | 59 | H (morning) | 2: Jamuni, Bholu | W | 8 | JAMUNI - Single + BHOLU - Single | | |
| 2 | N | Narrator | - | और कमेंट में 'जय यमुना मैया, जय यमराज जी' लिखना न भूलिए। चलिए, शुरू करें! **[comment]** | 73 | H (morning) | 2: Jamuni, Bholu | M | 9 | JAMUNI - Single + BHOLU - Single | | |
| 3 | N | Narrator | - | यमुना किनारे के एक गाँव में नन्ही जमुनी अपने भैया भोलू के साथ रहती थी। | 70 | H (morning) | 2: Jamuni, Bholu | M-shot: W, C | 9 | JAMUNI - Single + BHOLU - Single | | |
| 4 | N | Narrator | - | भैया दूज आने वाली थी, और आचार्य सोमदत्त आँगन में पोथी खोले बैठे थे। | 67 | H (morning) | 3: Jamuni, Bholu, Acharya Somdutt | M-shot: W, C | 9 | JAMUNI - Single + BHOLU - Single | | |
| 5 | D | Acharya Somdutt | Bholu | भोलू बेटा, तेरी कुंडली में इस साल यमराज की नज़र दिख रही है। | 59 | H (morning) | 3: Jamuni, Bholu, Acharya Somdutt | M | 8 | ACHARYA SOMDUTT - Single + BHOLU - Single | | |
| 6 | D | Bholu | Acharya Somdutt | यमराज? आचार्य जी, मुझे तो बस हलवे की नज़र लगी है! | 49 | H (morning) | 3: Jamuni, Bholu, Acharya Somdutt | C | 7 | BHOLU - Single + ACHARYA SOMDUTT - Single | | |
| 7 | D | Jamuni | Acharya Somdutt | आचार्य जी, मेरे भैया को कोई नहीं ले जाएगा! | 42 | H (morning) | 3: Jamuni, Bholu, Acharya Somdutt | C | 7 | JAMUNI - Single + ACHARYA SOMDUTT - Single | | |
| 8 | D | Acharya Somdutt | Jamuni | बेटी, यमराज के आगे किसी की नहीं चलती। रहने दे। | 46 | H (morning) | 3: Jamuni, Bholu, Acharya Somdutt | M | 7 | ACHARYA SOMDUTT - Single + JAMUNI - Single | | |
| 9 | D | Jamuni | Bholu | भैया, डरो मत! मैं यमराज को ही खाने पर बुला लूँगी! | 49 | H (morning) | 2: Jamuni, Bholu | C | 7 | JAMUNI - Single + BHOLU - Single | | |
| 10 | D | Bholu | Jamuni | पगली! यमराज कोई तेरे मामा हैं, जो खाने पर आ जाएँगे? **[HOOK]** | 51 | H (morning) | 2: Jamuni, Bholu | M | 7 | BHOLU - Single + JAMUNI - Single | | |
| 11 | N | Narrator | - | जमुनी को याद था कि यमुना मैया ने भी अपने भाई यमराज को घर बुलाया था। | 67 | H (morning) | 2: Jamuni, Bholu | M | 9 | JAMUNI - Single + BHOLU - Single | | |
| 12 | D | Jamuni | Bholu | यमुना मैया बुला सकती हैं, तो उनकी तरह मैं भी बुलाऊँगी! | 54 | H (morning) | 2: Jamuni, Bholu | C | 7 | JAMUNI - Single + BHOLU - Single | | |
| 13 | N | Narrator | - | अगली सुबह जमुनी यमुना घाट पर पहुँची और हाथ जोड़कर आँखें मूँद लीं। | 65 | G (dawn) | 1: Jamuni | W | 9 | JAMUNI - Single | | |
| 14 | D | Jamuni | the Yamuna river (off-screen) | यमराज भैया! कल भैया दूज है, मेरे घर खाना खाने आइए! **[HOOK]** | 50 | G (dawn) | 1: Jamuni | C | 7 | JAMUNI - Single | | |
| 15 | N | Narrator | - | यमुना की लहरें जगमगाईं, और दूर कहीं एक घंटी की आवाज़ गूँज उठी। | 62 | G (dawn) | 1: Jamuni | W | 9 | JAMUNI - Single | | |
| 16 | N | Narrator | - | भैया दूज की सुबह आँगन में रंगोली सजी थी, और पूजा की थाली तैयार थी। | 66 | H (morning) | 2: Jamuni, Bholu | W | 9 | JAMUNI - Single + BHOLU - Single | | |
| 17 | D | Bholu | Jamuni | जमुनी, यमराज तो आए नहीं, तेरे सारे लड्डू मैं खा लूँगा! | 54 | H (morning) | 2: Jamuni, Bholu | M | 7 | BHOLU - Single + JAMUNI - Single | | |
| 18 | D | Jamuni | Bholu | खबरदार भैया! पहले मेहमान, फिर तुम! | 34 | H (morning) | 2: Jamuni, Bholu | C | 7 | JAMUNI - Single + BHOLU - Single | | |
| 19 | N | Narrator | - | तभी आँगन में रोशनी फैली, और बही-खाता लिए चित्रगुप्त जी आ पहुँचे। | 64 | H (morning) | 3: Jamuni, Bholu, Chitragupt ji | M-shot: W, C | 9 | JAMUNI - Single + BHOLU - Single | | |
| 20 | D | Chitragupt ji | Jamuni | नमस्ते बेटी! यमराज जी ने मुझे पहले भेजा है, हिसाब देखने। | 56 | H (morning) | 3: Jamuni, Bholu, Chitragupt ji | M | 8 | CHITRAGUPT - Single + JAMUNI - Single | | |
| 21 | D | Jamuni | Chitragupt ji | चित्रगुप्त जी, पहले खाना खा लीजिए, हिसाब बाद में! **[HOOK]** | 49 | H (morning) | 3: Jamuni, Bholu, Chitragupt ji | C | 7 | JAMUNI - Single + CHITRAGUPT - Single | | |
| 22 | D | Chitragupt ji | Jamuni | वाह! मेरी बही में तो तुम्हारा नाम पुण्य में लिखा है। | 52 | H (morning) | 3: Jamuni, Bholu, Chitragupt ji | M | 7 | CHITRAGUPT - Single + JAMUNI - Single | | |
| 23 | D | Jamuni | Chitragupt ji | तो भैया का नाम भी पुण्य में लिख दो ना! | 38 | H (morning) | 3: Jamuni, Bholu, Chitragupt ji | C | 7 | JAMUNI - Single + CHITRAGUPT - Single | | |
| 24 | D | Chitragupt ji | Jamuni | यह फैसला तो यमराज जी ही करेंगे, बेटी। | 37 | H (morning) | 3: Jamuni, Bholu, Chitragupt ji | M | 7 | CHITRAGUPT - Single + JAMUNI - Single | | |
| 25 | N | Narrator | - | चित्रगुप्त जी मुस्कुराकर चले गए। जमुनी दौड़कर आचार्य जी को बताने गई। | 68 | H (noon) | 2: Jamuni, Acharya Somdutt | W | 9 | JAMUNI - Single + ACHARYA SOMDUTT - Single | | |
| 26 | D | Jamuni | Acharya Somdutt | आचार्य जी! चित्रगुप्त जी आए थे, हाथ में मोटी बही लेकर! | 54 | H (noon) | 2: Jamuni, Acharya Somdutt | C | 7 | JAMUNI - Single + ACHARYA SOMDUTT - Single | | |
| 27 | D | Acharya Somdutt | Jamuni | चित्रगुप्त और हमारे आँगन में? सपना देखा होगा बेटी। | 50 | H (noon) | 2: Jamuni, Acharya Somdutt | M | 7 | ACHARYA SOMDUTT - Single + JAMUNI - Single | | |
| 28 | D | Bholu | Acharya Somdutt | आचार्य जी, मैंने भी देखा! वो बही बहुत मोटी थी! | 46 | H (noon) | 3: Jamuni, Bholu, Acharya Somdutt | C | 7 | BHOLU - Single + ACHARYA SOMDUTT - Single | | |
| 29 | D | Acharya Somdutt | Bholu | तुम दोनों मिलकर मुझे बना रहे हो! यमराज यहाँ नहीं आएँगे। | 55 | H (noon) | 3: Jamuni, Bholu, Acharya Somdutt | M | 7 | ACHARYA SOMDUTT - Single + BHOLU - Single | | |
| 30 | N | Narrator | - | दोपहर में धरती काँपी, और लाल रोशनी के साथ यमराज जी उतरे। साथ में चित्रगुप्त जी भी थे। | 85 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | M-shot: W, C | 10 | JAMUNI - Single + BHOLU - Single | | |
| 31 | D | Acharya Somdutt | Jamuni | हे नारायण! जमुनी बेटी, ये तो सचमुच यमराज जी हैं! | 48 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | M | 7 | ACHARYA SOMDUTT - Single + JAMUNI - Single | | |
| 32 | D | Yamraj ji | Jamuni | जमुनी, तूने प्यार से बुलाया, इसलिए मैं आ गया। | 45 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | M | 7 | YAMRAJ - Single + JAMUNI - Single | | |
| 33 | D | Jamuni | Yamraj ji | यमराज भैया, आप मेरे भैया भोलू को ले तो नहीं जाओगे? | 50 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | C | 7 | JAMUNI - Single + YAMRAJ - Single | | |
| 34 | D | Yamraj ji | Jamuni | पहले मुझे तिलक कर, जैसे यमुना किया करती थी। | 43 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | M | 7 | YAMRAJ - Single + JAMUNI - Single | | |
| 35 | N | Narrator | - | जमुनी ने यमराज जी के माथे पर रोली का तिलक लगाकर आरती उतारी। | 59 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | M-shot: M, C | 8 | JAMUNI - Single + BHOLU - Single | | |
| 36 | D | Yamraj ji | Jamuni | बेटी, मैं प्रसन्न हूँ। माँग, तुझे क्या वरदान चाहिए? | 51 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | M | 7 | YAMRAJ - Single + JAMUNI - Single | | |
| 37 | D | Jamuni | Yamraj ji | बस इतना कि मेरे भैया पर कभी आपकी नज़र न पड़े! **[HOOK]** | 45 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | C | 7 | JAMUNI - Single + YAMRAJ - Single | | |
| 38 | D | Yamraj ji | Jamuni | आज जो भाई बहन से तिलक लगवाएगा, उसे यम का भय नहीं होगा। **[moral]** | 54 | H (afternoon, red-gold glow) | 5: Jamuni, Bholu, Acharya Somdutt, Chitragupt ji, Yamraj ji | M | 7 | YAMRAJ - Single + JAMUNI - Single | | |
| 39 | N | Narrator | - | जमुनी ने भोलू के माथे पर तिलक लगाया और उसकी कलाई पर मौली बाँधी। | 63 | H (afternoon, red-gold glow) | 2: Jamuni, Bholu | M | 9 | JAMUNI - Single + BHOLU - Single | | |
| 40 | D | Bholu | Jamuni | जमुनी, तू तो मेरी छोटी रक्षक है! ये ले, मेरे हिस्से का लड्डू! | 61 | H (afternoon, red-gold glow) | 2: Jamuni, Bholu | C | 8 | BHOLU - Single + JAMUNI - Single | | |
| 41 | D | Chitragupt ji | Bholu | लो भोलू, मैंने तुम्हारी बही में लिख दिया: दीर्घायु भव! | 54 | H (afternoon, red-gold glow) | 2: Bholu, Chitragupt ji | M | 7 | CHITRAGUPT - Single + BHOLU - Single | | |
| 42 | D | Acharya Somdutt | Jamuni | बेटी, मुझे क्षमा करना। मैंने तुझ पर शक किया था। | 47 | H (afternoon, red-gold glow) | 2: Jamuni, Acharya Somdutt | M | 7 | ACHARYA SOMDUTT - Single + JAMUNI - Single | | |
| 43 | D | Yamraj ji | Acharya Somdutt | आचार्य, बहन का प्रेम सबसे बड़ा रक्षा-कवच होता है। | 49 | H (afternoon, red-gold glow) | 2: Acharya Somdutt, Yamraj ji | M | 7 | YAMRAJ - Single + ACHARYA SOMDUTT - Single | | |
| 44 | D | Jamuni | Yamraj ji | अब खाना खाइए यमराज भैया! गरमागरम पूरी-हलवा बना है! | 50 | H (afternoon, red-gold glow) | 2: Jamuni, Yamraj ji | C | 7 | JAMUNI - Single + YAMRAJ - Single | | |
| 45 | D | Yamraj ji | Jamuni | वाह! ऐसा स्वाद तो पूरे यमलोक में भी नहीं मिलता! | 47 | H (afternoon, red-gold glow) | 2: Jamuni, Yamraj ji | M | 7 | YAMRAJ - Single + JAMUNI - Single | | |
| 46 | N | Narrator | - | शाम को यमराज जी और चित्रगुप्त जी आशीर्वाद देकर अंतर्धान हो गए। आँगन में दीप जल उठे। | 83 | H (evening, diyas) | 3: Jamuni, Bholu, Acharya Somdutt | W | 10 | JAMUNI - Single + BHOLU - Single | | |
| 47 | D | Acharya Somdutt | Bholu | अगली भैया दूज पर कुंडली नहीं, पूरी-हलवा देखूँगा! **[final gag]** | 48 | H (evening, diyas) | 3: Jamuni, Bholu, Acharya Somdutt | C | 7 | ACHARYA SOMDUTT - Single + BHOLU - Single | | |
| 48 | N | Narrator | - | तो दोस्तों, बहन का प्रेम हर संकट से बड़ा है। जय यमुना मैया, जय यमराज जी! **[closing]** | 72 | H (evening, diyas) | 3: Jamuni, Bholu, Acharya Somdutt | W | 9 | JAMUNI - Single + BHOLU - Single | | |

Estimated length: story clips sum to about 369 s before trimming, plus the reused hook (about 30 s). After trimming each clip to its speech and leaving about half a second between clips, measure the real runtime after assembly; if it is under 5:45 or over 6:30, say so in the report and trim clips or lines.

## YouTube title and description

**Title:** भैया दूज पर यमराज की बहन | Bhai Dooj Katha | Jamuni aur Yamraj | 3D भक्ति कथा

**Description:** भैया दूज पर नन्ही जमुनी ने यमुना मैया की तरह अपने भैया को यमराज से बचाने के लिए यमराज जी को ही खाने पर बुला लिया! चित्रगुप्त जी और यमराज जी मेहमान बनकर आए, और आचार्य जी देखते रह गए। कहानी अच्छी लगे तो चैनल को सब्सक्राइब करें और कमेंट में 'जय यमुना मैया, जय यमराज जी' ज़रूर लिखें। #BhaiDooj #YamDwitiya #BhaktiKatha #3DAnimation #HindiKahani
