# Second souffle

Instrumental électronique mélodique, 120 bpm, **Ré mineur** puis **Mi mineur**, 88 mesures (2 min 56). Le morceau se termine une première fois, pour de bon : un petit arc monte vite, se défait jusqu'à une seule note, puis quatre mesures de presque rien. Il repart en demi-temps sur un Ré tenu à la basse, les accords bougent au-dessus sans que la basse cède, un accord suspendu attend quatre mesures, et le vrai sommet arrive un ton plus haut, la basse bougeant enfin sur son premier temps. Le thème du début y passe à la basse pendant qu'une longue phrase chante au-dessus.

## Brief et contraintes

- **Profil : drifting-cycles** (imposé par le brief ; rotation morzak → drifting-cycles → aucun).

Profil : drifting-cycles

- **Tempo** : 120 bpm, lecture « dance » du profil (118–126) ; la reprise (45–60) se lit en demi-temps par la batterie seule, le tempo ne change pas.
- **Tonalité** : Ré mineur naturel (Ré Mi Fa Sol La Si♭ Do), puis **Mi mineur** (+2 demi-tons) à la mesure 61 (69 % du morceau). Une image d'accords par section :
  - **intro** (1–8) : aucun accord, arpège et basse seuls sur Ré ;
  - **cycle 1** (9–24) : **Dm add9 – B♭maj7 – F add9 – Csus4**, deux mesures par accord (harmonie lente) ;
  - **cycle 2** (25–40) : **B♭maj7 – C add9 – Dm7 – Gm7**, une mesure par accord (harmonie rapide) ; ancre : B♭maj7 ;
  - **cycle 3** (45–60) : **Gm7 – B♭maj7** sur pédale de Ré, deux mesures par accord, puis **Esus4** sur Ré tenu quatre mesures (57–60) ; ancres : Gm7 et B♭maj7 ; le Si naturel de Esus4 annonce Mi mineur ;
  - **cycle 4** (61–84) : **Em add9 – G – D add9 – Cmaj7**, une mesure par accord, en Mi mineur ; Esus4 s'y résout ;
  - **fin** (85–88) : Cmaj7 tenu, non résolu, puis coupure.
- **Palette par rôle** (cinq pistes, master) :
  - arpège (couche pincée) : Oscillator en carré, relâchement court, Filter passe-bas automatisé, Echo 1/8. ;
  - basse : Oscillator en dents de scie, Filter passe-bas, propre, capable de tenir une pédale ;
  - nappe : Oscillator en dents de scie, attaque lente, Bloom en ensemble, Reverb ; large ;
  - thème (lead) : Oscillator en carré, Echo 1/4 dont le mélange est automatisé ;
  - pulsation : Drums ; quatre temps dans le premier arc et au sommet, demi-temps à la reprise ;
  - master : Compressor léger, Ceiling.
- **Longueur cible** : 88 mesures.
- **Contraintes** (trois, dont deux gestes du profil) :
  1. *(profil, geste 3)* **une pédale sous des accords qui bougent** : la basse tient Ré de 53 à 60 et ne bouge que sur le premier temps du sommet (61.1, Mi) ;
  2. *(profil, geste 2)* **une montée tardive d'un ton** à 69 %, avec une mesure amincie avant (60 : batterie muette) et une note qui traverse la coupure (Mi) ;
  3. *(la mienne)* **le thème n'a que cinq notes** (La Ré Mi Fa Do, puis Si Mi Fa# Sol Ré) et n'est jamais récrit : il est réharmonisé (cycle 1, cycle 2, cycle 3) puis transposé et donné à la basse.
- **Hypothèses** : pas de voix, aucun fichier audio ; tout vient des instruments et des effets de Faulk.
- **Forme** : `Form: F9 Fausse fin, puis une seconde vie` (les deux passages précédents sont F3 « Braise » et F2 « Apnée », exclus ; le profil nomme F4, F9, F10, F1 ; F4 a servi le 2026-11-11 ; F9 porte la pédale et la montée tardive du profil : la reprise garde la dernière note en pédale, le vrai sommet est dans un autre ton). Écarts à la carte F9 : la montée est d'un ton (profil) et non d'une quarte ; le thème passe à la basse huit mesures seulement (69–76).

## Catalogue d'attributs

- Tempo : 120 bpm, lecture dance ; demi-temps de batterie à la reprise.
- Mode et harmonie : mineur, accords étendus (add9, maj7, m7, sus4), un cycle par section, une section en pédale, une montée tardive d'un ton.
- Son : couche arpégée pincée, nappe chaude et large, basse propre qui tient une pédale, lead simple.
- Rythme : quatre temps ou caisse en demi-temps ; un roulement seulement avant un changement de section (mesure 24).
- Mélodie : un thème court énoncé tôt (mesure 9), varié par les accords sous lui ; une longue phrase chantée dans le dernier tiers (69–76).
- Forme : par sections, intro sans accords.
- Mix : bas-médium plein, sub propre, haut présent, nappe large, basse et lead au centre.

## Boucle de départ

```pattern notes "Arp intro" bars=1 grid=8 octave=4 key="D minor" role=arp
D A E5 A D A D5 A |
```

La figure : fondamentale, quinte, neuvième, quinte, fondamentale, quinte, octave, quinte. Pas de tierce : elle se transpose telle quelle sur chaque accord et donne la couleur sus2 du profil.

```pattern notes "Basse intro" bars=2 grid=4 octave=2 key="D minor" role=bass
D - - - | D - - C |
```

Ré tenu, et un Do de passage qui ramène au Ré.

```pattern drums "Beat charley" bars=1 grid=16
CHat  |..x...x...x...x.|
```

Le charley fermé à contretemps, seul.

```pattern notes "Thème" bars=4 grid=8 octave=5 key="D minor" role=melody
A4 - - D - E F - | E - - - D - C - | A4 - - D - E F - | A - - - - - . . |
```

Le thème : cinq notes, deux phrases ; la seconde finit sur le La5, sommet, une fois.

```pattern drums "Beat A" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |..x...x...x...x.|
```

Quatre temps, clap sur 2 et 4.

## Variations

```pattern notes "Arp cycle 1" bars=8 grid=8 octave=4 key="D minor" role=arp
D A E5 A D A D5 A | D A E5 A D A D5 A | Bb3 F C5 F Bb3 F Bb F | Bb3 F C5 F Bb3 F Bb F | F3 C G C F3 C F C | F3 C G C F3 C F C | C G D5 G C G C5 G | C G D5 G C G C5 G |
```

Génération 1 (harmonie) : la figure posée sur le cycle 1, deux mesures par accord.

```pattern notes "Basse cycle 1" bars=8 grid=8 octave=2 key="D minor" role=bass
. D . D . D . D | . D . D . D . D | . Bb1 . Bb1 . Bb1 . Bb1 | . Bb1 . Bb1 . Bb1 . Bb1 | . F . F . F . F | . F . F . F . F | . C . C . C . C | . C . C . C . C |
```

Génération 2 (rythme) : la basse à contretemps, entre les kicks.

```pattern notes "Nappe cycle 1" bars=8 grid=1 octave=4 key="D minor" role=pad
F3+A3+D+E | - | F3+Bb3+D+A | - | F3+A3+C+G | - | G3+C+F | - |
```

Génération 3 (son) : Dm add9, B♭maj7, F add9, Csus4 ; le Fa3 reste en bas trois accords.

```pattern drums "Beat roulement" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......xxxx|
CHat  |..x...x...x...x.|
```

Génération 4 (forme) : la mesure 24, un roulement de clap sur le dernier temps.

```pattern notes "Arp cycle 2" bars=4 grid=8 octave=4 key="D minor" role=arp
Bb3 F C5 F Bb3 F Bb F | C G D5 G C G C5 G | D A E5 A D A D5 A | G3 D A D G3 D G D |
```

Génération 5 (harmonie) : le cycle 2, une mesure par accord.

```pattern notes "Basse cycle 2" bars=4 grid=8 octave=2 key="D minor" role=bass
. Bb1 . Bb1 . Bb1 . Bb1 | . C . C . C . C | . D . D . D . D | . G1 . G1 . G1 . G1 |
```

La basse suit le cycle 2.

```pattern notes "Nappe cycle 2" bars=4 grid=1 octave=4 key="D minor" role=pad
F3+Bb3+D+A | G3+C+D+E | F3+A3+C+D | G3+Bb3+D+F |
```

B♭maj7, C add9, Dm7, Gm7.

```pattern drums "Beat pic" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |oooooooooooooooo|
OHat  |..o...o...o...o.|
```

Génération 6 (rythme) : charley fermé en doubles croches douces, charley ouvert à contretemps.

```pattern notes "Note tenue" bars=4 grid=1 octave=5 key="D minor" role=lead
D | - | - | - |
```

Génération 7 (forme) : la seule note qui reste à la fin du premier arc.

```pattern drums "Beat demi" bars=1 grid=16
Kick  |x.........x.....|
Clap  |........x.......|
CHat  |..o...o...o...o.|
```

Génération 8 (rythme) : le demi-temps de la reprise.

```pattern notes "Nappe pédale" bars=4 grid=1 octave=4 key="D minor" role=pad
G3+Bb3+D+F | - | F3+Bb3+D+A | - |
```

Gm7 puis B♭maj7, au-dessus du Ré de la basse.

```pattern notes "Basse pédale" bars=4 grid=1 octave=2 key="D minor" role=bass
D | - | D | - |
```

Contrainte 1 : Ré tenu, deux mesures par note.

```pattern notes "Nappe sus" bars=4 grid=1 octave=4 role=pad
E3+A3+B3+E | - | - | - |
```

Esus4 tenu quatre mesures. Sans `key=` : le Si naturel sort de Ré mineur exprès, c'est la porte vers Mi mineur.

```pattern notes "Mi tenu" bars=2 grid=1 octave=5 key="D minor" role=lead
E | - |
```

La note qui traverse : Mi5, deux mesures (59–60).

```pattern notes "Arp sommet" bars=4 grid=8 octave=4 key="E minor" role=arp
E B F#5 B E B E5 B | G3 D A D G3 D G D | D A E5 A D A D5 A | C G D5 G C G C5 G |
```

Génération 9 (harmonie) : le cycle 4 en Mi mineur.

```pattern notes "Basse sommet" bars=4 grid=8 octave=2 key="E minor" role=bass
. E . E . E . E | . G1 . G1 . G1 . G1 | . D . D . D . D | . C . C . C . C |
```

La basse du cycle 4 : elle quitte enfin le Ré.

```pattern notes "Nappe sommet" bars=4 grid=1 octave=4 key="E minor" role=pad
G3+B3+E+F# | G3+B3+D+G | F#3+A3+D+E | G3+B3+C+E |
```

Em add9, G, D add9, Cmaj7.

```pattern notes "Thème mi" bars=4 grid=8 octave=5 key="E minor" role=melody
B4 - - E - F# G - | F# - - - E - D - | B4 - - E - F# G - | B - - - - - . . |
```

Génération 10 (harmonie) : le thème un ton plus haut, mêmes intervalles.

```pattern notes "Basse thème" bars=8 grid=8 octave=2 key="E minor" role=bass
B1 - - E - F# G - | F# - - - E - D - | B1 - - E - F# G - | B - - - - - . . | B1 - - E - F# G - | F# - - - E - D - | B1 - - E - F# G - | B - - - - - . . |
```

Génération 11 (forme) : échange de rôles, le thème à la basse.

```pattern notes "Chant long" bars=8 grid=4 octave=5 key="E minor" role=melody
B4 - - - | D - - E | F# - - - | G - E - | E - - F# | G - - A | B - - - | - - A G |
```

Génération 12 (mélodie) : la longue phrase du dernier tiers ; elle monte jusqu'au Si5, une fois.

```pattern notes "Nappe fin" bars=4 grid=1 octave=4 key="E minor" role=pad
G3+B3+C+E | - | - | - |
```

Cmaj7 tenu : la fin ne se résout pas.

## Arrangement

Form: F9 Fausse fin, puis une seconde vie

```arrangement tempo=120
section Intro        1-8   : Arp intro, Basse intro, Beat charley [from=5]
section A            9-24  : Beat A [mute=24], Beat roulement [from=24], Arp cycle 1, Basse cycle 1, Thème, Nappe cycle 1 [from=17]
section Sommet 1    25-32  : Beat pic, Arp cycle 2, Basse cycle 2, Nappe cycle 2, Thème
section Dissolution 33-40  : Beat charley [to=35], Basse cycle 2 [to=35], Arp cycle 2 [to=37], Nappe cycle 2 [to=37], Thème [to=37], Note tenue [from=37]
section Queue       41-44  :
section Reprise     45-60  : Beat demi [to=60], Nappe pédale [to=57], Nappe sus [from=57], Thème [from=49 to=57], Basse pédale [from=53], Mi tenu [from=59]
section Sommet 2    61-84  : Beat pic [mute=84.4], Arp sommet, Nappe sommet, Basse sommet [mute=69-76], Basse thème [from=69 to=77], Thème mi [mute=69-76], Chant long [from=69 to=77]
section Fin         85-88  : Nappe fin
```

Cycles : intro sans accords ; A cycle 1 ; Sommet 1 et Dissolution cycle 2 ; Reprise cycle 3 (pédale de Ré, puis Esus4) ; Sommet 2 cycle 4 en Mi mineur ; Fin Cmaj7.

Coutures : 24 → 25 roulement de clap ; 32 → 33 la batterie tombe au charley seul, puis basse (35), arpège, nappe et thème (37) s'en vont ; 40 → 41 il ne reste que la queue de l'écho ; 44 → 45 la batterie repart seule avec la nappe ; 60 → 61 mesure amincie (batterie muette), Mi5 tenu, la basse passe de Ré à Mi sur 61.1 ; 84 → 85 le kick manque sur 84.4, puis un seul accord.

Événements uniques :

1. 24.4 : roulement de clap (le seul du morceau).
2. 41–44 : **fausse fin**, quatre mesures sans aucune note (structurel).
3. 57–60 : Esus4 tenu quatre mesures sur la pédale ; 60 : batterie muette.
4. 61.1 : la basse bouge enfin, tout monte d'un ton.
5. 69–76 : **échange de rôles**, le thème à la basse, la longue phrase au lead (structurel).
6. 84.4 : le kick manque ; 85 : coupure sur Cmaj7.

Écart à la notation : le Mi5 de 59–60 s'arrête à la barre de 61 dans la fiche (un motif ne traverse pas une section) ; il traverse par l'écho du lead, et Si3 et Mi4 restent dans la nappe de Esus4 à Em add9.

## Automation

```automation "Arp ouverture" part="Arp cycle 1" param=cutoff
9.1 40 ease-in, 24.4 100
```

La coupure du Filter de l'arpège s'ouvre lentement puis vite pendant A : l'arc court.

```automation "Arp fermeture" part="Arp cycle 2" param=cutoff
25.1 110, 33.1 110 ease-out, 36.4 25
```

Au sommet 1 elle est ouverte ; à la dissolution elle tombe vite puis se pose.

```automation "Arp retour" part="Arp sommet" param=cutoff
61.1 110
```

Au vrai sommet l'arpège revient ouvert d'un coup (dans Faulk : le point de 36.4 est en palier jusqu'à 61.1).

```automation "Nappe gonfle" part="Nappe pédale" param=volume curve=smooth
45.1 50, 56.4 100
```

Le volume de la nappe monte en S pendant la pédale (dans Faulk : −13 dB tenu en palier depuis la mesure 1, −24 dB à 45.1, courbe en S jusqu'à −13 dB à 56.4).

```automation "Thème écho" part="Note tenue" param=delay
33.1 30 step, 37.1 100 step, 45.1 30
```

Le mélange de l'Echo du lead saute sur la note tenue : c'est elle qui fait la queue de la fausse fin ; il revient à sa valeur à la reprise.

## Notes de finition

- Arpège : carré, attaque 2 ms, relâchement 120 ms ; Filter passe-bas (coupure automatisée, 400 Hz à 6 kHz) ; Echo 1/8., retour 30 %, mélange 15 %.
- Basse : dents de scie, relâchement 100 ms, Filter passe-bas 500 Hz.
- Nappe : dents de scie, attaque 400 ms, relâchement 1,2 s, Filter passe-bas 2,5 kHz, Bloom Ensemble, Reverb.
- Thème : carré, attaque 10 ms, relâchement 250 ms, Filter passe-bas 3,5 kHz, Echo 1/4 retour 45 %.
- Mix arpège : L30 ; plan milieu (Echo 1/8. retour 30 % mélange 15 %) ; étroit ; 300 Hz–3 kHz.
- Mix basse : C ; plan avant, sans Reverb ; mono ; 40–250 Hz (Filter passe-bas 500 Hz).
- Mix nappe : C ; plan arrière (Reverb taille 70 %, amortissement 70 %, mélange 40 %) ; large (Bloom Ensemble, phase stéréo 150, tonalité 300 Hz, mélange 45 %) ; 200 Hz–2,5 kHz.
- Mix thème : C ; plan avant (Echo 1/4, mélange 25 %, automatisé) ; point au centre ; 500 Hz–5 kHz.
- Mix pulsation : C ; plan avant ; mono ; kick 40–100 Hz, charleys au-dessus de 5 kHz.
- Contrôle mono : lu sur la fiche : kick, basse et lead au centre, aucun Bloom sous 150 Hz (tonalité 300 Hz), mélange du Bloom ≤ 50 %, l'arpège à L30 garde son écho des deux côtés. Laissé à l'oreille : la tenue de la nappe Bloom coupé.
- Humaniser : vélocités du charley, léger retard du clap ; non fait.
- Laissé à l'oreille : l'équilibre basse / kick au sommet 2, le niveau de la longue phrase.
- Version suivante : la montée d'une tierce mineure au lieu d'un ton ; le thème en canon à la reprise.

## Vérification

Sortie de `sheet_tool.py check` (mot pour mot) :

```

[notes] 'Arp intro'  bars=1 grid=8 notes=8
  OK     all 8 notes are in D minor
  INFO   contour: range 14 semitones, highest note occurs 1x, steps 0 / leaps 7, up 26 / down 19 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse intro'  bars=2 grid=4 notes=3
  OK     all 3 notes are in D minor
  INFO   contour: range 2 semitones, highest note occurs 2x, steps 1 / leaps 0, up 0 / down 2 semitones, 1.5 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[drums] 'Beat charley'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Thème'  bars=4 grid=8 notes=12
  OK     all 12 notes are in D minor
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 7 / leaps 4, up 20 / down 8 semitones, 3.0 notes per bar

[drums] 'Beat A'  bars=1 grid=16 notes=10

[notes] 'Arp cycle 1'  bars=8 grid=8 notes=64
  OK     all 64 notes are in D minor
  INFO   contour: range 23 semitones, highest note occurs 2x, steps 0 / leaps 62, up 208 / down 203 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse cycle 1'  bars=8 grid=8 notes=32
  OK     all 32 notes are in D minor
  INFO   contour: range 7 semitones, highest note occurs 8x, steps 0 / leaps 3, up 7 / down 9 semitones, 4.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Nappe cycle 1'  bars=8 grid=1 notes=15
  OK     all 15 notes are in D minor

[drums] 'Beat roulement'  bars=1 grid=16 notes=13

[notes] 'Arp cycle 2'  bars=4 grid=8 notes=32
  OK     all 32 notes are in D minor
  INFO   contour: range 21 semitones, highest note occurs 1x, steps 0 / leaps 31, up 104 / down 100 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse cycle 2'  bars=4 grid=8 notes=16
  OK     all 16 notes are in D minor
  INFO   contour: range 7 semitones, highest note occurs 4x, steps 2 / leaps 1, up 4 / down 7 semitones, 4.0 notes per bar

[notes] 'Nappe cycle 2'  bars=4 grid=1 notes=16
  OK     all 16 notes are in D minor

[drums] 'Beat pic'  bars=1 grid=16 notes=26

[notes] 'Note tenue'  bars=4 grid=1 notes=1
  OK     all 1 notes are in D minor

[drums] 'Beat demi'  bars=1 grid=16 notes=7

[notes] 'Nappe pédale'  bars=4 grid=1 notes=8
  OK     all 8 notes are in D minor

[notes] 'Basse pédale'  bars=4 grid=1 notes=2
  OK     all 2 notes are in D minor

[notes] 'Nappe sus'  bars=4 grid=1 notes=4

[notes] 'Mi tenu'  bars=2 grid=1 notes=1
  OK     all 1 notes are in D minor

[notes] 'Arp sommet'  bars=4 grid=8 notes=32
  OK     all 32 notes are in E minor
  INFO   contour: range 23 semitones, highest note occurs 1x, steps 0 / leaps 30, up 104 / down 101 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse sommet'  bars=4 grid=8 notes=16
  OK     all 16 notes are in E minor
  INFO   contour: range 9 semitones, highest note occurs 4x, steps 1 / leaps 2, up 7 / down 11 semitones, 4.0 notes per bar

[notes] 'Nappe sommet'  bars=4 grid=1 notes=16
  OK     all 16 notes are in E minor

[notes] 'Thème mi'  bars=4 grid=8 notes=12
  OK     all 12 notes are in E minor
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 7 / leaps 4, up 20 / down 8 semitones, 3.0 notes per bar

[notes] 'Basse thème'  bars=8 grid=8 notes=24
  OK     all 24 notes are in E minor
  INFO   contour: range 12 semitones, highest note occurs 2x, steps 14 / leaps 9, up 40 / down 28 semitones, 3.0 notes per bar

[notes] 'Chant long'  bars=8 grid=4 notes=13
  OK     all 13 notes are in E minor
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 9 / leaps 2, up 15 / down 7 semitones, 1.6 notes per bar

[notes] 'Nappe fin'  bars=4 grid=1 notes=4
  OK     all 4 notes are in E minor

[arrangement] tempo=120
  Intro          bars   1-8   ( 8) 3 parts
                 edits: Beat charley [from=5]
  A              bars   9-24  (16) 6 parts
                 edits: Beat A [mute=24]; Beat roulement [from=24]; Nappe cycle 1 [from=17]
  Sommet 1       bars  25-32  ( 8) 5 parts
  Dissolution    bars  33-40  ( 8) 6 parts
                 edits: Beat charley [to=35]; Basse cycle 2 [to=35]; Arp cycle 2 [to=37]; Nappe cycle 2 [to=37]; Thème [to=37]; Note tenue [from=37]
  Queue          bars  41-44  ( 4) 0 parts
  Reprise        bars  45-60  (16) 6 parts
                 edits: Beat demi [to=60]; Nappe pédale [to=57]; Nappe sus [from=57]; Thème [from=49 to=57]; Basse pédale [from=53]; Mi tenu [from=59]
  Sommet 2       bars  61-84  (24) 7 parts
                 edits: Beat pic [mute=84.4]; Basse sommet [mute=69-76]; Basse thème [from=69 to=77]; Thème mi [mute=69-76]; Chant long [from=69 to=77]
  Fin            bars  85-88  ( 4) 1 parts
  total 88 bars

[automation] 'Arp ouverture'  part='Arp cycle 1' cc=74 (cutoff) curve=linear points=2

[automation] 'Arp fermeture'  part='Arp cycle 2' cc=74 (cutoff) curve=linear points=3

[automation] 'Arp retour'  part='Arp sommet' cc=74 (cutoff) curve=linear points=1
  NOTE   a single point is a constant value, not a move

[automation] 'Nappe gonfle'  part='Nappe pédale' cc=7 (volume) curve=smooth points=2

[automation] 'Thème écho'  part='Note tenue' cc=94 (delay) curve=linear points=3

RESULT ok
```
