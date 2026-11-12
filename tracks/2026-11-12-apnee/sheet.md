# Apnée

Instrumental électronique, 122 bpm, **Mi mineur**, 72 mesures (2 min 22). Le titre : la mesure où l'on retient son souffle. Le morceau tient sur une seule idée de forme : **l'impact vient de la mesure d'avant**. Un couplet doux et plein (nappe, phrase pincée, basse tenue, pulsation légère), une montée où la phrase se raccourcit, **une mesure de vide**, puis un drop qui a **moins de parties que le couplet** : un kick, une basse en doubles croches et un crochet de trois notes. Aucun profil de style.

## Brief et contraintes

- **Profil de style** : aucun (rotation morzak → drifting-cycles → none).
- **Tempo** : 122 bpm.
- **Tonalité** : Mi mineur naturel. Trois images d'accords :
  - **cycle A** (couplet 1–16, couplet 2 42–49) : **Cmaj7 – Dadd9 – Em7 – Em7** (VI – VII – i – i), deux mesures par accord ;
  - **cycle B** (montée 17–24) : **Am7 – Bm7 – Cmaj7 – D** (iv – v – VI – VII), deux mesures par accord, la voix du haut monte Do, Ré, Mi, Fa# ; la montée s'arrête sur le VII, non résolu, et le vide le laisse en l'air ;
  - **cycle C** (drops 26–41 et 51–57) : **Mi seul** : pas d'accord, la basse tient Mi avec Ré, Sol, La, Si en notes de passage ; le crochet dit Mi, Sol, Si ;
  - fin (66–69) : **Cmaj7** tenu, non résolu (le premier accord du couplet, comme une question).
- **Palette par rôle** (cinq pistes, master) :
  - pulsation : Drums. « Beat couplet » en demi-temps (kick sur 1 et le « et » de 3, clap sur 3), **sans charley** ; « Beat drop » quatre sur le temps, clap 2 et 4, charley ouvert doux sur les contretemps ;
  - basse : Oscillator en dents de scie, relâchement 120 ms, Filter passe-bas 300 Hz, **Contour** (cloche +3 dB vers 90 Hz, creux vers 300 Hz) ; « Basse tenue A / B » (rondes liées) puis « Basse drop » (doubles croches) ;
  - harmonie : nappe, Oscillator en dents de scie, attaque 400 ms, relâchement 900 ms, Filter passe-bas automatisé, **Ripple** en phaser lent, Reverb 40 % ; « Nappe A », « Nappe B », « Nappe fin » ;
  - phrase pincée : Oscillator en carré, relâchement 80 ms, **Contour** en coupe-bas vers 200 Hz, Echo 1/8 dont le mélange est automatisé ; « Phrase », « Phrase montée », « Crochet pincé » ;
  - crochet : Oscillator en dents de scie, attaque 5 ms, relâchement 150 ms, Filter passe-bas 2,5 kHz, **Ripple** en flanger au tempo, dont un réglage est automatisé ; « Crochet », « Crochet mut », « Note seule » ;
  - master : **Contour** (preset d'usine de nettoyage du bas), Compressor, Ceiling.
- **Longueur cible** : 72 mesures.
- **Contraintes** (trois) :
  1. **le drop a moins de parties que le couplet** : quatre au couplet (pulsation, basse tenue, nappe, phrase), trois au drop (pulsation, basse, crochet) ; ni nappe ni phrase dans un drop ;
  2. **le crochet n'a que trois hauteurs** : Mi, Sol, Si ; sa mutation ne change que le rythme et l'ordre ;
  3. **aucun charley avant le drop** : les contretemps de charley ouvert sont réservés aux mesures 26–41 et 51–57.
- **Hypothèses** : pas de voix, aucun fichier audio ; tout vient des instruments et des effets de Faulk.
- **Forme** : `Form: F2 Drop à charnière de silence` (les deux passages précédents sont F4 « Marée » et F6 « Lisière », exclus ; F0 exclu par la ration ; le brief ne donne ni forme ni humeur ; parmi le reste, F2 est celle qui sert le mieux le matériau du jour : deux effets de timbre, Contour et Ripple, dont l'un sculpte le creux et l'autre anime le peu de notes du drop).

## Boucle de départ

La pulsation d'abord, puis la partie qui définit le morceau (la basse et le crochet du drop), puis le couplet.

```pattern drums "Beat drop" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
OHat  |..o...o...o...o.|
```

Quatre sur le temps, clap 2 et 4, charley ouvert doux (60) sur chaque contretemps : la seule figure de charley du morceau (contrainte 3).

```pattern notes "Basse drop" bars=2 grid=16 octave=1 key="E minor" role=bass
E . . E . . E . . . E2 . D2 . . . | E . . E . . E . . . G . A . B . |
```

Mi en 3 + 3 + 4 doubles croches contre le kick, un saut d'octave et Ré à la fin de la première mesure, Sol La Si qui remontent vers le Mi à la fin de la seconde. Notes courtes (une double croche).

```pattern notes "Crochet" bars=2 grid=16 octave=5 key="E minor" role=hook
E . . E . . B4 . . . E . . . . . | B4 . . B4 . . E . G . . . . . . . |
```

Trois hauteurs (contrainte 2), le même 3 + 3 + 4 que la basse ; le Sol5, sommet, une seule fois, puis presque une mesure de vide : le crochet laisse plus de place qu'il n'en prend.

```pattern drums "Beat couplet" bars=1 grid=16
Kick  |x.........x.....|
Clap  |........x.......|
```

Demi-temps, sans charley : la pulsation « légère » du couplet.

```pattern notes "Phrase" bars=2 grid=8 octave=4 key="E minor" role=melody
B . G B . E5 . D5 | . B . G A . B . |
```

La phrase pincée du couplet : neuf croches, le Mi5 au sommet une fois, toutes dans la pentatonique de Mi mineur : elles tiennent sur Cmaj7, Dadd9 et Em7.

```pattern notes "Nappe A" bars=8 grid=4 octave=3 key="E minor" role=pad
C3+E3+G3+B3 - - - | - - - - | D3+F#3+A3+E4 - - - | - - - - | E3+G3+B3+D4 - - - | - - - - | - - - - | - - - - |
```

Cycle A : Cmaj7, Dadd9 (deux mesures chacun), Em7 tenu quatre mesures.

```pattern notes "Basse tenue A" bars=8 grid=4 octave=2 key="E minor" role=bass
C2 - - - | - - - - | D2 - - - | - - - - | E2 - - - | - - - - | - - - - | - - - - |
```

Les fondamentales du cycle A en notes longues : la basse du couplet ne bouge pas, celle du drop ne tient pas.

## Variations

```pattern notes "Nappe B" bars=8 grid=4 octave=3 key="E minor" role=pad
E3+G3+A3+C4 - - - | - - - - | F#3+A3+B3+D4 - - - | - - - - | G3+B3+C4+E4 - - - | - - - - | A3+D4+F#4 - - - | - - - - |
```

Génération 1 (harmonie) : cycle B, Am7, Bm7, Cmaj7 (renversés, la fondamentale à la basse tenue), D : la voix du haut monte Do4, Ré4, Mi4, Fa#4.

```pattern notes "Basse tenue B" bars=8 grid=4 octave=1 key="E minor" role=bass
A1 - - - | - - - - | B1 - - - | - - - - | C2 - - - | - - - - | D2 - - - | - - - - |
```

Génération 2 (harmonie) : les fondamentales du cycle B, qui montent par degrés vers le Mi du drop sans l'atteindre.

```pattern notes "Phrase montée" bars=8 grid=8 octave=4 key="E minor" role=melody
B . G B . E5 . D5 | . B . G A . B . | B . G B . E5 . D5 | B . G B . E5 . D5 | B . G B B . G B | B . G B B . G B | B . B . B . B . | B B B B B B B B |
```

Génération 3 (forme) : la phrase se raccourcit : entière (8 temps), sa première mesure deux fois (4 temps), sa première cellule quatre fois (2 temps), puis le Si seul à la noire (1 temps) et à la croche. Le Mi5 revient trois fois : c'est une répétition qui se resserre, pas une mélodie à sommet unique (décision).

```pattern notes "Crochet mut" bars=2 grid=16 octave=5 key="E minor" role=hook
G . . E . . E . . . B4 . . . E . | G . . E . . B4 . E . . . B4 . E . |
```

Génération 4 (rythme et ordre, contrainte 2) : les trois mêmes hauteurs, mais le crochet part du sommet et remplit le vide de la fin ; le Sol5 ouvre chaque mesure (deux fois : décision, c'est la version « impatiente » du second drop).

```pattern notes "Crochet pincé" bars=2 grid=16 octave=4 key="E minor" role=hook
E . . E . . B3 . . . E . . . . . | B3 . . B3 . . E . G . . . . . . . |
```

Génération 5 (son et registre) : le crochet une octave plus bas, sur l'instrument pincé, pour le couplet 2 : la mélodie du drop revient sur les accords du couplet.

```pattern notes "Note seule" bars=1 grid=4 octave=5 key="E minor" role=lead
E - - - |
```

Génération 6 (silence) : le second vide n'est pas vide : un Mi5 seul, tenu une mesure.

```pattern notes "Nappe fin" bars=4 grid=4 octave=3 key="E minor" role=pad
C3+E3+G3+B3 - - - | - - - - | - - - - | - - - - |
```

Génération 7 (forme) : Cmaj7 tenu quatre mesures : la fin ne résout pas.

## Arrangement

Form: F2 Drop à charnière de silence

```arrangement tempo=122
section Couplet    1-16  : Beat couplet, Basse tenue A, Nappe A, Phrase
section Montee    17-24  : Beat couplet [to=24.3], Basse tenue B, Nappe B, Phrase montée
section Vide      25-25  :
section Drop      26-41  : Beat drop [to=41.4], Basse drop, Crochet
section Couplet2  42-49  : Beat couplet, Basse tenue A, Nappe A, Crochet pincé
section Vide2     50-50  : Note seule
section Drop2     51-57  : Beat drop [to=57.3], Basse drop [to=57.3], Crochet mut
section Sortie    58-72  : Crochet pincé [to=66], Nappe fin [from=66 to=70]
```

Longueurs irrégulières voulues : les deux vides d'une mesure (25 et 50), le second drop de **sept** mesures (51–57, coupé une mesure plus tôt que l'oreille ne l'attend), la sortie de quinze (58–72 : huit mesures de crochet seul, quatre de nappe, trois de queue).

Cycles par section : Couplet et Couplet 2 : cycle A (Cmaj7 – Dadd9 – Em7 – Em7) ; Montée : cycle B (Am7 – Bm7 – Cmaj7 – D) ; Drop et Drop 2 : Mi seul (cycle C) ; Sortie : rien, puis Cmaj7.

Coutures :
- 16 → 17 : la phrase continue sans changer (la montée commence par la phrase entière) ; seule l'harmonie bouge ;
- 24 → 25 → 26 : la pulsation s'arrête au temps 3 de 24 (`to=24.3`), la dernière croche de la phrase est jetée dans l'écho (automation), la mesure 25 n'a que des queues ; le drop entre plein au temps 1 de 26 ;
- 41 → 42 : le Beat drop perd son dernier temps (`to=41.4`, hésitation) ; le crochet change d'instrument sans changer de notes ;
- 49 → 50 → 51 : le Em7 du couplet 2 finit, le Mi5 seul tient la mesure 50, le drop 2 entre ;
- 57 → 58 : pulsation et basse coupées au temps 3 de 57 (`to=57.3`), le crochet muté finit seul ; le crochet pincé reprend à 58 ;
- 65 → 66 : la nappe entre quand le crochet s'arrête ; 70–72 : la queue de la Reverb.

Événements uniques :
1. **mesure 25 : une mesure de silence** (structurel) ;
2. mesure 24, temps 4 : la dernière croche de la phrase jetée dans l'écho ;
3. **mesure 50 : une note seule** à la place du vide (structurel) ;
4. mesure 57, temps 3 : le second drop coupé au milieu de sa septième mesure ;
5. mesure 41, temps 4 : le kick manque une fois.

Arc : le sommet est le premier drop (26–41, 36 à 57 % du morceau), préparé par le vide ; le second drop est plus court et plus nerveux ; la sortie est la mémoire du crochet.

## Automation

```automation "Nappe ouverture" part="Nappe B" param=cutoff curve=ease-in
17.1 40, 24.4 110
```

La coupure du Filter de la nappe s'ouvre de 600 Hz à 6 kHz pendant la montée (`ease-in` : lente puis rapide) ; elle est ramenée à 600 Hz par un point à 26.1 (hors du bloc : la partie n'y joue plus).

```automation "Phrase écho" part="Phrase montée" cc=94 curve=step
17.1 30, 24.4 115
```

Le mélange de l'Echo de la phrase saute de 25 % à 90 % au temps 4 de 24 (`step` : un saut) : la dernière croche est jetée dans le vide ; il retombe à 25 % à 26.1.

```automation "Crochet balayage" part="Crochet" param=modulation curve=linear
26.1 20, 41.4 110
```

Un réglage de Ripple sur le crochet (le centre du balayage, ou à défaut le mélange) monte en ligne droite sur les seize mesures du drop : les mêmes huit notes, de plus en plus creusées.

## Notes de finition

- Sons : voir la palette. Presets d'usine comme points de départ : Ripple « slow phaser » sur la nappe, « synced flanger » sur le crochet ; Contour « low cut tidy » sur le master.
- Mix: Pulsation : C, devant (ni Reverb ni Echo), sans largeur, kick 50–100 Hz, clap 1–4 kHz, charley au-dessus de 6 kHz
- Mix: Basse : C, devant (pas de Reverb, Filter passe-bas 300 Hz, Contour +3 dB à 90 Hz et −3 dB à 300 Hz), sans largeur, 40–300 Hz
- Mix: Nappe : C, fond (Reverb mélange 40 %, Filter passe-bas 600 Hz → 6 kHz), Ripple phaser lent pour la largeur, 250 Hz–4 kHz
- Mix: Phrase : L20, milieu (Echo 1/8 mélange 25 %, Contour coupe-bas 200 Hz), sans largeur, 400 Hz–5 kHz
- Mix: Crochet : R10, devant (Filter passe-bas 2,5 kHz, pas de Reverb), Ripple flanger au tempo pour la largeur, 500 Hz–6 kHz
- Mono check : 1, 3 et 4 à la lecture (basse et kick au centre et mono ; la largeur ne vient que de Ripple et de la Reverb, jamais d'une paire de pistes) ; 2 (ce que le flanger devient en mono) laissé à l'oreille.
- Humaniser : rien ; la raideur du drop est voulue. Le clap pourrait reculer de quelques millisecondes.
- Laissé à l'oreille : la profondeur et le retour de Ripple, le gain exact des bandes de Contour, le niveau de la note seule.
- Version suivante : un troisième drop à contretemps, la phrase en canon dans la sortie, une vraie caisse claire.

## Check

```
[drums] 'Beat drop'  bars=1 grid=16 notes=10

[notes] 'Basse drop'  bars=2 grid=16 notes=11
  OK     all 11 notes are in E minor
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 3 / leaps 3, up 19 / down 12 semitones, 5.5 notes per bar

[notes] 'Crochet'  bars=2 grid=16 notes=8
  OK     all 8 notes are in E minor
  INFO   contour: range 8 semitones, highest note occurs 1x, steps 0 / leaps 5, up 13 / down 10 semitones, 4.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[drums] 'Beat couplet'  bars=1 grid=16 notes=3

[notes] 'Phrase'  bars=2 grid=8 notes=9
  OK     all 9 notes are in E minor
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 3 / leaps 5, up 13 / down 13 semitones, 4.5 notes per bar

[notes] 'Nappe A'  bars=8 grid=4 notes=12
  OK     all 12 notes are in E minor

[notes] 'Basse tenue A'  bars=8 grid=4 notes=3
  OK     all 3 notes are in E minor
  INFO   contour: range 4 semitones, highest note occurs 1x, steps 2 / leaps 0, up 4 / down 0 semitones, 0.4 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Nappe B'  bars=8 grid=4 notes=15
  OK     all 15 notes are in E minor

[notes] 'Basse tenue B'  bars=8 grid=4 notes=4
  OK     all 4 notes are in E minor
  INFO   contour: range 5 semitones, highest note occurs 1x, steps 3 / leaps 0, up 5 / down 0 semitones, 0.5 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Phrase montée'  bars=8 grid=8 notes=43
  OK     all 43 notes are in E minor
  INFO   contour: range 9 semitones, highest note occurs 3x, steps 5 / leaps 21, up 47 / down 47 semitones, 5.4 notes per bar
  INFO   contour: the highest note repeats; a memorable line usually has a single peak

[notes] 'Crochet mut'  bars=2 grid=16 notes=11
  OK     all 11 notes are in E minor
  INFO   contour: range 8 semitones, highest note occurs 2x, steps 0 / leaps 9, up 18 / down 21 semitones, 5.5 notes per bar
  INFO   contour: the highest note repeats; a memorable line usually has a single peak
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Crochet pincé'  bars=2 grid=16 notes=8
  OK     all 8 notes are in E minor
  INFO   contour: range 8 semitones, highest note occurs 1x, steps 0 / leaps 5, up 13 / down 10 semitones, 4.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Note seule'  bars=1 grid=4 notes=1
  OK     all 1 notes are in E minor

[notes] 'Nappe fin'  bars=4 grid=4 notes=4
  OK     all 4 notes are in E minor

[arrangement] tempo=122
  Couplet        bars   1-16  (16) 4 parts
  Montee         bars  17-24  ( 8) 4 parts
                 edits: Beat couplet [to=24.3]
  Vide           bars  25-25  ( 1) 0 parts  <- length not a multiple of 4 bars
  Drop           bars  26-41  (16) 3 parts
                 edits: Beat drop [to=41.4]
  Couplet2       bars  42-49  ( 8) 4 parts
  Vide2          bars  50-50  ( 1) 1 parts  <- length not a multiple of 4 bars
  Drop2          bars  51-57  ( 7) 3 parts  <- length not a multiple of 4 bars
                 edits: Beat drop [to=57.3]; Basse drop [to=57.3]
  Sortie         bars  58-72  (15) 2 parts  <- length not a multiple of 4 bars
                 edits: Crochet pincé [to=66]; Nappe fin [from=66 to=70]
  total 72 bars

[automation] 'Nappe ouverture'  part='Nappe B' cc=74 (cutoff) curve=ease-in points=2

[automation] 'Phrase écho'  part='Phrase montée' cc=94 (cc94) curve=step points=2

[automation] 'Crochet balayage'  part='Crochet' cc=1 (modulation) curve=linear points=2

RESULT ok
```
