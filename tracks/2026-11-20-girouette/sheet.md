# Girouette

## Brief et contraintes

Instrumental électronique mélodique, clair, dansant sans dureté, 122 bpm, **Ré majeur** (visite du relatif, Si mineur, au milieu ; hausse tardive d'une tierce mineure vers **Fa majeur**), 96 mesures (3 min 09). Le titre : une girouette ne change pas, c'est le vent qui tourne. Une accroche de huit notes est dite tôt et ne change plus ; à chaque section ce sont les accords, la basse et le rythme qui tournent autour d'elle. Elle passe à la basse, se réduit à son squelette sur une pédale, puis remonte d'une tierce mineure quand la basse bouge enfin.

Form: F4 Thème et variations

Profil : drifting-cycles

Profil de style : **drifting-cycles** (rotation morzak → drifting-cycles → aucun).

- **Tempo** : 122 bpm, 4/4 : la lecture « dance » du profil (118–126), grosse caisse sur les quatre temps ; la variation 1 passe en demi-temps.
- **Tonalité** : Ré majeur ; Si mineur (le relatif) à la variation 2 ; Fa majeur (+3 demi-tons) à partir de la mesure 65 (68 % du morceau). Un seul changement de tonalité.
- **Palette par rôles** (sept pistes) : accroche = carré doux avec écho, au centre ; arpège = dent de scie courte et filtrée, pincée, en 3+3+2 ; nappe = dent de scie lente, large, en retrait ; basse = sinus propre, capable de tenir une pédale ; batterie = grosse caisse et clap ; charley = charley fermé seul sur sa piste, **balancé** (les doubles croches paires à 58 % de la croche) ; chant = sinus avec écho, une seule phrase longue dans le dernier tiers.
- **Longueur** : 96 mesures.
- **Forme** : F4. Les deux fiches précédentes sont F3 « Lame de fond » et F10 « Manège » (exclues). Le profil nomme F4, F9, F10 et F1 ; restent F4 et F9 ; F4 est la plus ancienne dans l'historique (le 11) et sa règle, un paramètre changé par variation, est exactement le geste du profil (la même mélodie, d'autres accords). Écarts assumés à la carte F4 : le changement de centre arrive à la variation 4 (mesure 65) et non à la 3, pour tomber dans la fenêtre du profil (65–75 %) ; la variation « squelette » passe avant lui ; le canon est laissé ; le retour reste en Fa (un seul changement de tonalité) et son détail changé est la phrase chantée.

Trois contraintes, dont deux gestes du profil :

1. *(profil, geste 1 et 5)* **l'accroche ne change jamais de notes** ; chaque section a son cycle d'accords, qui garde un accord du précédent comme ancre (Sol maj7, puis La sus4) ; l'accroche est donc réharmonisée à chaque reprise.
2. *(profil, gestes 2, 3 et 4)* **une pédale, un accord suspendu, une seule hausse** : de 49 à 64 la basse tient Ré sous des accords qui bougent, Ré sus4 n'est jamais résolu ; à 65 la basse bouge pour la première fois, le Sol suspendu descend enfin, mais sur Fa naturel : la résolution est la hausse (+3). La mesure 64 est amincie et le La de l'accroche est tenu à travers la coupure (La : quinte de Ré, tierce de Fa).
3. *(la mienne)* **le rythme 3+3+2 est partout sauf dans la batterie** : accroche, arpège et basse du sommet le portent ; la batterie reste droite, seul le charley est balancé.

Ce que je garde du profil : lecture « dance », majeur avec visite du relatif, cycles de 2 à 4 accords, un cycle par section avec une ancre, accords enrichis (maj7, m7, add9, sus4), une pédale, la hausse tardive avec mesure amincie et note tenue, l'accroche courte réharmonisée, la phrase chantée du dernier tiers, le roulement avant un changement de section seulement, le balancement du seul charley, le contraste harmonie lente (var. 1 et 3) / rapide (thème, var. 2, sommet), une introduction sans accords (arpège et basse, l'accroche à la mesure 5). Ce que je plie : la forme F4 (ordre des variations). Ce que je laisse : le pompage par sidechain et les montées de bruit (dits en prose dans les notes de finition, pas dans la notation).

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Filter, Echo, Reverb, Bloom, Compressor, Ceiling).

## Catalogue d'attributs

- **Son** : une accroche carrée douce avec écho au tempo ; un arpège pincé filtré dont la coupure bouge ; une nappe large ; une basse sinus propre qui tient une pédale ; un chant sinus.
- **Harmonie** : Ré majeur ; thème Ré maj7 – Si m7 – Sol maj7 – La sus4 (une mesure chacun) ; var. 1 Sol maj7 – Mi m7 (deux mesures chacun) ; var. 2 Si m7 – Fa♯ m7 – Sol maj7 – La sus4 ; var. 3 Sol add9 – Mi m7 – Ré sus4 sur pédale de Ré ; sommet Fa maj7 – Ré m7 – Si♭ maj7 – Do sus4 → Do.
- **Mélodie** : une accroche de huit notes, dite à la mesure 5, variée par les accords ; une phrase chantée longue à 81.
- **Rythme** : quatre temps droits, demi-temps à la variation 1 ; un roulement de clap avant un changement de section seulement ; charley balancé seul.
- **Forme** : par sections, introduction sans accords, hausse à 68 %.
- **Tempo** : 122 bpm.
- **Mix** : bas-médiums pleins, sub propre, aigu présent, nappe large, basse et accroche au centre.

## Boucle de départ

L'accroche : huit notes en 3+3+2, un seul sommet (Fa♯5, la première note), une fin ouverte sur La.

```pattern notes "Accroche" bars=4 grid=8 octave=4 key="D major" role=hook
F#5 - - E5 - - D5 - | A4 - - - - - . . | B4 - - D5 - - E5 - | A4 - - - - - - . |
```

L'arpège du thème : la cellule de trois notes en 3+3+2 ; le Ré grave ne bouge qu'à la quatrième mesure.

```pattern notes "Arp A" bars=4 grid=8 octave=4 key="D major" role=arp
D4 A4 C#5 D4 A4 C#5 D4 A4 | D4 A4 B4 D4 A4 B4 D4 A4 | D4 G4 B4 D4 G4 B4 D4 G4 | E4 A4 D5 E4 A4 D5 E4 A4 |
```

La basse du thème : les fondamentales, tenues, avec une levée.

```pattern notes "Basse A" bars=4 grid=8 octave=1 key="D major" role=bass
D2 - - - - - . D2 | B1 - - - - - . B1 | G1 - - - - - . G1 | A1 - - - - - A1 C#2 |
```

La nappe du thème : Ré maj7 – Si m7 – Sol maj7 – La sus4 ; la voix du bas tient Ré.

```pattern notes "Nappe A" bars=4 grid=4 octave=3 key="D major" role=pad
D3+F#3+A3+C#4 - - - | D3+F#3+A3+B3 - - - | D3+F#3+G3+B3 - - - | D3+E3+A3+D4 - - - |
```

La batterie : quatre temps, clap sur 2 et 4.

```pattern drums "Beat A" bars=1 grid=16
Kick |x...x...x...x...|
Clap |....x.......x...|
```

Le charley balancé : quatre doubles croches par temps, les paires retardées à 58 % de la croche (grille de 96 : pas 0, 7, 12, 19 de chaque temps), la croche en l'air accentuée.

```pattern drums "Hat S" bars=1 grid=96
CHat |o......o....x......o....o......o....x......o....o......o....x......o....o......o....x......o....|
```

## Variations

- **Arp B** (gén. 2, harmonie) : Sol maj7 deux mesures, Mi m7 deux mesures ; l'harmonie ralentit.

```pattern notes "Arp B" bars=4 grid=8 octave=4 key="D major" role=arp
D4 G4 B4 D4 G4 B4 D4 G4 | D4 F#4 B4 D4 F#4 B4 D4 F#4 | E4 G4 B4 E4 G4 B4 E4 G4 | D4 G4 B4 D4 G4 B4 E4 G4 |
```

- **Basse B** (gén. 3, rythme) : deux notes longues et un Fa♯ de passage.

```pattern notes "Basse B" bars=4 grid=8 octave=1 key="D major" role=bass
G1 - - - - - - - | - - - - - - F#1 . | E1 - - - - - - - | - - - - - - F#1 . |
```

- **Nappe B** (gén. 4, harmonie) : Sol maj7 puis Mi m7 ; une seule voix bouge (Fa♯ → Mi).

```pattern notes "Nappe B" bars=4 grid=4 octave=3 key="D major" role=pad
G3+B3+D4+F#4 - - - | - - - - | G3+B3+D4+E4 - - - | - - - - |
```

- **Beat H** (gén. 5, rythme) : le demi-temps de la variation 1.

```pattern drums "Beat H" bars=1 grid=16
Kick |x.........x.....|
Clap |........x.......|
```

- **Roulement** (gén. 6, rythme) : le clap roule sur le dernier temps ; avant un changement de section seulement.

```pattern drums "Roulement" bars=1 grid=16
Kick |x...x...x.......|
Clap |....x.......ooxx|
```

- **Basse C** (gén. 7, forme) : l'accroche passe à la basse, trois octaves plus bas.

```pattern notes "Basse C" bars=4 grid=8 octave=2 key="B minor" role=bass
F#2 - - E2 - - D2 - | A1 - - - - - . . | B1 - - D2 - - E2 - | A1 - - - - - - . |
```

- **Arp C** (gén. 8, harmonie) : Si m7 – Fa♯ m7 – Sol maj7 – La sus4 ; les deux dernières mesures sont celles du thème (l'ancre).

```pattern notes "Arp C" bars=4 grid=8 octave=4 key="B minor" role=arp
B3 F#4 A4 B3 F#4 A4 B3 F#4 | C#4 F#4 A4 C#4 F#4 A4 C#4 E4 | D4 G4 B4 D4 G4 B4 D4 G4 | E4 A4 D5 E4 A4 D5 E4 A4 |
```

- **Nappe C** (gén. 9, harmonie) : les accords choisis pour la basse qui chante (Fa♯, La, Si, La sont des notes des accords).

```pattern notes "Nappe C" bars=4 grid=4 octave=3 key="B minor" role=pad
D3+F#3+A3+B3 - - - | E3+F#3+A3+C#4 - - - | D3+F#3+G3+B3 - - - | D3+E3+A3+D4 - - - |
```

- **Squelette** (gén. 10, mélodie) : l'accroche réduite à la première note de chaque mesure ; le dernier La est celui qui traverse la coupure.

```pattern notes "Squelette" bars=4 grid=4 octave=4 key="D major" role=hook
F#5 - - - | A4 - - - | B4 - - - | A4 - - - |
```

- **Arp D** (gén. 11, texture) : trois notes par mesure, toujours en 3+3+2, communes aux trois accords de la pédale.

```pattern notes "Arp D" bars=1 grid=8 octave=4 key="D major" role=arp
D5 . . A4 . . G4 . |
```

- **Basse D** (gén. 12, harmonie) : la pédale. Un Ré tenu quatre mesures (la signature du profil).

```pattern notes "Basse D" bars=4 grid=4 octave=2 key="D major" role=bass
D2 - - - | - - - - | - - - - | - - - - |
```

- **Nappe D** (gén. 13, harmonie) : Sol add9 – Mi m7 – Ré sus4 tenu quatre mesures, jamais résolu.

```pattern notes "Nappe D" bars=8 grid=4 octave=3 key="D major" role=pad
G3+A3+B3+D4 - - - | - - - - | G3+B3+D4+E4 - - - | - - - - | G3+A3+D4+G4 - - - | - - - - | - - - - | - - - - |
```

- **Kick 4** (gén. 14, densité) : la grosse caisse seule sous la pédale.

```pattern drums "Kick 4" bars=1 grid=16
Kick |x...x...x...x...|
```

- **Accroche F** (gén. 15, tonalité) : la même accroche, une tierce mineure plus haut.

```pattern notes "Accroche F" bars=4 grid=8 octave=5 key="F major" role=hook
A5 - - G5 - - F5 - | C5 - - - - - . . | D5 - - F5 - - G5 - | C5 - - - - - - . |
```

- **Arp E** (gén. 16, tonalité) : l'arpège du thème en Fa ; une note changée (le Mi5 de la dernière mesure) pour la résolution du sus.

```pattern notes "Arp E" bars=4 grid=8 octave=4 key="F major" role=arp
F4 C5 E5 F4 C5 E5 F4 C5 | F4 C5 D5 F4 C5 D5 F4 C5 | F4 Bb4 D5 F4 Bb4 D5 F4 Bb4 | G4 C5 F5 G4 C5 E5 G4 C5 |
```

- **Basse E** (gén. 17, rythme) : la basse bouge enfin, et prend le 3+3+2.

```pattern notes "Basse E" bars=4 grid=8 octave=1 key="F major" role=bass
F1 - . F1 - . F1 - | D2 - . D2 - . D2 - | Bb1 - . Bb1 - . Bb1 - | C2 - . C2 - . C2 E2 |
```

- **Nappe E** (gén. 18, harmonie) : Fa maj7 – Ré m7 – Si♭ maj7 – Do sus4 qui se résout en Do à mi-mesure.

```pattern notes "Nappe E" bars=4 grid=4 octave=3 key="F major" role=pad
F3+A3+C4+E4 - - - | F3+A3+C4+D4 - - - | F3+A3+Bb3+D4 - - - | F3+G3+C4+F4 - E3+G3+C4+E4 - |
```

- **Chant** (gén. 19, mélodie) : la phrase longue du dernier tiers, par degrés, un seul sommet (La5).

```pattern notes "Chant" bars=8 grid=8 octave=5 key="F major" role=melody
C5 - - - - - D5 E5 | F5 - - - - - E5 D5 | D5 - - - - - C5 Bb4 | C5 - - - - - . . |
E5 - - - - - F5 G5 | A5 - - - - - G5 F5 | F5 - - - - - E5 D5 | C5 - - - - - - - |
```

- **Nappe fin** et **Basse fin** (gén. 20) : Fa add9 tenu quatre mesures sur Fa.

```pattern notes "Nappe fin" bars=4 grid=4 octave=3 key="F major" role=pad
F3+A3+C4+G4 - - - | - - - - | - - - - | - - - - |
```

```pattern notes "Basse fin" bars=4 grid=4 octave=1 key="F major" role=bass
F1 - - - | - - - - | - - - - | - - - - |
```

26 motifs (21 mélodiques, 5 de batterie) : plus que la vingtaine conseillée, mais chacun diffère par ses notes (cinq cycles d'accords sur trois pistes) ; les entrées, sorties et coupes sont des fenêtres.

## Arrangement

Form: F4 Thème et variations

```arrangement tempo=122
section Intro      1-8    : Arp A, Basse A, Accroche [from=5]
section Theme      9-16   : Accroche, Arp A, Basse A, Nappe A, Beat A
section Var1      17-32   : Accroche, Arp B, Basse B, Nappe B, Beat H [mute=32], Roulement [from=32], Hat S
section Var2      33-48   : Arp C, Basse C, Nappe C, Beat A [to=48.3], Hat S [to=48.3]
section Var3      49-64   : Squelette, Arp D [mute=64], Basse D, Nappe D, Kick 4 [mute=64]
section Sommet    65-80   : Accroche F, Arp E, Basse E, Nappe E, Beat A [mute=80], Roulement [from=80], Hat S
section Retour    81-88   : Chant, Arp E, Basse E, Nappe E, Beat A [to=88.4], Hat S [to=88.4]
section Coda      89-92   : Accroche F, Arp E, Nappe E
section Fin       93-96   : Nappe fin, Basse fin
```

Toutes les sections sont des multiples de quatre mesures. Le roulement est une fenêtre (`Roulement [from=32]`, `[from=80]`) sur la dernière mesure de la section, où le motif de batterie se tait (`[mute=32]`, `[mute=80]`).

Cycles d'accords par section :

- Intro, Thème (1–16) : Ré maj7 | Si m7 | Sol maj7 | La sus4, une mesure chacun (sans nappe de 1 à 8 : l'arpège et la basse seuls les disent).
- Variation 1 (17–32) : Sol maj7 (2) | Mi m7 (2). Ancre : Sol maj7. L'accroche y devient 7e majeure, 9e, quinte, 11e.
- Variation 2 (33–48) : Si m7 | Fa♯ m7 | Sol maj7 | La sus4. Ancres : Sol maj7 et La sus4. L'accroche est à la basse, la piste d'accroche se tait.
- Variation 3 (49–64) : Sol add9 (2) | Mi m7 (2) | Ré sus4 (4), sur pédale de Ré. Ancre : Mi m7.
- Sommet, Retour, Coda (65–92) : Fa maj7 | Ré m7 | Si♭ maj7 | Do sus4 → Do. Note commune à la coupure : La (et Sol).
- Fin (93–96) : Fa add9.

Coutures et événements uniques :

1. **5.1** : l'accroche entre seule sur l'arpège et la basse (introduction sans accords).
2. **17.1** : demi-temps et charley balancé, l'harmonie ralentit (deux mesures par accord).
3. **32** : roulement de clap sur le quatrième temps.
4. **48.3** : batterie et charley coupés deux temps (hésitation) avant la pédale.
5. **64** *(structurel)* : mesure amincie, ni batterie ni arpège ; le La4 de l'accroche et Ré sus4 tenus.
6. **65.1** *(structurel)* : la basse quitte Ré pour la première fois en seize mesures, tout monte d'une tierce mineure, le Sol suspendu tombe sur Fa.
7. **80** : second roulement ; **88.4** : la batterie s'arrête un temps avant la coda.
8. **93** : Fa add9 tenu, l'écho de l'accroche finit seul.

## Automation

```automation "Coupure arp" part="Arp A" param=cutoff curve=linear
1.1 45 ease-in, 17.1 85 linear, 33.1 70 linear, 49.1 50 ease-in, 64.4 95 step, 65.1 110 linear, 89.1 110 ease-out, 96.4 40
```

La coupure du Filter de l'arpège : elle s'ouvre lentement puis vite sur l'introduction, se referme un peu en Si mineur, repart de bas sous la pédale et s'ouvre en accélérant jusqu'à la coupure ; grande ouverte au sommet ; elle retombe vite puis doucement à la fin.

```automation "Volume nappe" part="Nappe A" param=volume curve=smooth
9.1 70 smooth, 17.1 90 linear, 49.1 80 ease-in, 63.4 110 step, 64.1 85 step, 65.1 105 linear, 93.1 105 ease-out, 96.4 50
```

Le niveau de la nappe : elle entre en fondu, gonfle sous la pédale, s'efface d'un palier à la mesure amincie, revient pleine au sommet.

```automation "Coupure basse" part="Basse C" param=cutoff curve=ease-in
33.1 50 ease-in, 48.2 105 step, 49.1 45
```

La coupure du Filter de la basse quand elle porte l'accroche (variation 2) : elle s'ouvre pour chanter, puis se referme d'un coup pour la pédale.

```automation "Echo accroche" part="Accroche" param=delay curve=step
5.1 25 step, 31.1 70 step, 33.1 25 step, 63.1 80 step, 65.1 30 step, 91.1 85
```

Le mélange de l'Echo de l'accroche, par paliers : lancé aux fins de section (31–32, 63–64) et à la dernière reprise (91).

## Notes de finition

- **Sons** : accroche = Oscillator carré, attaque 5 ms, déclin 200 ms, maintien 60 %, relâchement 200 ms, Echo au tempo 1/8. (le pas pointé répond au 3+3+2) ; arpège = Oscillator dent de scie, déclin 120 ms, maintien 20 %, relâchement 100 ms, Filter passe-bas automatisé, Echo léger ; nappe = dent de scie, attaque 400 ms, relâchement 1 s, Filter 1,5 kHz, Bloom Ensemble, Reverb ; basse = sinus, attaque 5 ms, relâchement 150 ms, Filter passe-bas automatisé (peu d'effet sur un sinus : passer la basse en dent de scie filtrée à la variation 2 si l'oreille le demande) ; chant = sinus, attaque 30 ms, Echo 1/4, Reverb.
- **Sidechain et bruit** (laissés hors notation) : un pompage de la nappe et de la basse sur la grosse caisse (Compressor de la nappe déclenché par la batterie) du sommet à 88 ; une montée de bruit filtré de 61 à 64. À faire si Faulk le permet ; sinon c'est un manque.
- **Balancement** : le charley à 58 % ; si l'outil ne sait faire que le triolet (66,7 %), le dire.
- Mix: Accroche: C, devant (Echo 1/8. mélange 25 %, pas de Reverb), sans largeur, 500 Hz–4 kHz
- Mix: Arpège: L20, milieu (Echo mélange 15 %, Filter passe-bas automatisé 600 Hz–6 kHz), sans largeur, 300 Hz–5 kHz
- Mix: Nappe: C, fond (Reverb taille 70 % mélange 35 %, Filter passe-bas 1,5 kHz), Bloom Ensemble phase stéréo 150 mélange 45 %, 200 Hz–2 kHz
- Mix: Basse: C, devant (pas de Reverb), sans largeur, 40–200 Hz
- Mix: Batterie: C, devant (sèche), sans largeur, 50 Hz–5 kHz
- Mix: Charley: R20, milieu (sec), sans largeur, au-dessus de 6 kHz
- Mix: Chant: R10, milieu (Echo 1/4 mélange 25 %, Reverb mélange 20 %), sans largeur, 500 Hz–3 kHz
- **Contrôle mono** : la basse, la batterie et l'accroche sont au centre et sans élargissement ; seule la nappe est large (Bloom) : à vérifier à l'oreille en mono qu'elle ne s'efface pas. Mesuré sur l'export : niveaux gauche et droite par section ; l'écoute mono reste à faire.
- **Humaniser** : vélocités du charley (fantômes à 60, la croche en l'air à 100) ; rien d'autre.
- **Laissé à l'oreille** : le niveau de l'accroche face à l'arpège (même registre), la longueur de l'écho lancé, le dosage du pompage.
- **Version suivante** : le canon de la carte F4 (l'accroche contre elle-même deux mesures plus tard) dans le retour ; une seconde visite du relatif en Fa (Ré mineur).

## Check

`python sheet_tool.py check fiche-girouette.md` :

```
[notes] 'Accroche'  bars=4 grid=8 notes=8
  OK     all 8 notes are in D major
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 7 / down 16 semitones, 2.0 notes per bar

[notes] 'Arp A'  bars=4 grid=8 notes=32
  OK     all 32 notes are in D major
  INFO   contour: range 12 semitones, highest note occurs 2x, steps 2 / leaps 29, up 102 / down 95 semitones, 8.0 notes per bar

[notes] 'Basse A'  bars=4 grid=8 notes=9
  OK     all 9 notes are in D major
  INFO   contour: range 7 semitones, highest note occurs 2x, steps 1 / leaps 3, up 6 / down 7 semitones, 2.2 notes per bar

[notes] 'Nappe A'  bars=4 grid=4 notes=16
  OK     all 16 notes are in D major

[drums] 'Beat A'  bars=1 grid=16 notes=6

[drums] 'Hat S'  bars=1 grid=96 notes=16
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Arp B'  bars=4 grid=8 notes=32
  OK     all 32 notes are in D major
  INFO   contour: range 9 semitones, highest note occurs 8x, steps 1 / leaps 30, up 83 / down 78 semitones, 8.0 notes per bar

[notes] 'Basse B'  bars=4 grid=8 notes=4
  OK     all 4 notes are in D major
  INFO   contour: range 3 semitones, highest note occurs 1x, steps 3 / leaps 0, up 2 / down 3 semitones, 1.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Nappe B'  bars=4 grid=4 notes=8
  OK     all 8 notes are in D major

[drums] 'Beat H'  bars=1 grid=16 notes=3

[drums] 'Roulement'  bars=1 grid=16 notes=8

[notes] 'Basse C'  bars=4 grid=8 notes=8
  OK     all 8 notes are in B minor
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 7 / down 16 semitones, 2.0 notes per bar

[notes] 'Arp C'  bars=4 grid=8 notes=32
  OK     all 32 notes are in B minor
  INFO   contour: range 15 semitones, highest note occurs 2x, steps 1 / leaps 30, up 94 / down 84 semitones, 8.0 notes per bar

[notes] 'Nappe C'  bars=4 grid=4 notes=16
  OK     all 16 notes are in B minor

[notes] 'Squelette'  bars=4 grid=4 notes=4
  OK     all 4 notes are in D major
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 2 / leaps 1, up 2 / down 11 semitones, 1.0 notes per bar

[notes] 'Arp D'  bars=1 grid=8 notes=3
  OK     all 3 notes are in D major
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 1 / leaps 1, up 0 / down 7 semitones, 3.0 notes per bar

[notes] 'Basse D'  bars=4 grid=4 notes=1
  OK     all 1 notes are in D major

[notes] 'Nappe D'  bars=8 grid=4 notes=12
  OK     all 12 notes are in D major

[drums] 'Kick 4'  bars=1 grid=16 notes=4

[notes] 'Accroche F'  bars=4 grid=8 notes=8
  OK     all 8 notes are in F major
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 7 / down 16 semitones, 2.0 notes per bar

[notes] 'Arp E'  bars=4 grid=8 notes=32
  OK     all 32 notes are in F major
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 2 / leaps 29, up 101 / down 94 semitones, 8.0 notes per bar

[notes] 'Basse E'  bars=4 grid=8 notes=13
  OK     all 13 notes are in F major
  INFO   contour: range 11 semitones, highest note occurs 1x, steps 1 / leaps 3, up 15 / down 4 semitones, 3.2 notes per bar

[notes] 'Nappe E'  bars=4 grid=4 notes=20
  OK     all 20 notes are in F major

[notes] 'Chant'  bars=8 grid=8 notes=20
  OK     all 20 notes are in F major
  INFO   contour: range 11 semitones, highest note occurs 1x, steps 16 / leaps 1, up 16 / down 16 semitones, 2.5 notes per bar

[notes] 'Nappe fin'  bars=4 grid=4 notes=4
  OK     all 4 notes are in F major

[notes] 'Basse fin'  bars=4 grid=4 notes=1
  OK     all 1 notes are in F major

[arrangement] tempo=122
  Intro          bars   1-8   ( 8) 3 parts
                 edits: Accroche [from=5]
  Theme          bars   9-16  ( 8) 5 parts
  Var1           bars  17-32  (16) 7 parts
                 edits: Beat H [mute=32]; Roulement [from=32]
  Var2           bars  33-48  (16) 5 parts
                 edits: Beat A [to=48.3]; Hat S [to=48.3]
  Var3           bars  49-64  (16) 5 parts
                 edits: Arp D [mute=64]; Kick 4 [mute=64]
  Sommet         bars  65-80  (16) 7 parts
                 edits: Beat A [mute=80]; Roulement [from=80]
  Retour         bars  81-88  ( 8) 6 parts
                 edits: Beat A [to=88.4]; Hat S [to=88.4]
  Coda           bars  89-92  ( 4) 3 parts
  Fin            bars  93-96  ( 4) 2 parts
  total 96 bars

[automation] 'Coupure arp'  part='Arp A' cc=74 (cutoff) curve=linear points=8

[automation] 'Volume nappe'  part='Nappe A' cc=7 (volume) curve=smooth points=8

[automation] 'Coupure basse'  part='Basse C' cc=74 (cutoff) curve=ease-in points=3

[automation] 'Echo accroche'  part='Accroche' cc=94 (delay) curve=step points=6

RESULT ok
```
