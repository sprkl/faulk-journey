# Deux rives

## Brief et contraintes

Instrumental électronique en deux morceaux qui n'en font qu'un : une rive sombre, lente de sensation, balancée, en **Mi mineur** ; une rive claire, droite, dansante, en **Mi♭ majeur**. Entre les deux, une seule note tenue, Sol : tierce de Mi mineur, tierce de Mi♭ majeur. 100 bpm, 80 mesures (3 min 12).

Form: F5 Deux morceaux en un

Profil : aucun

Profil de style : aucun (rotation morzak → drifting-cycles → aucun). Mes propres choix.

- **Tempo** : 100 bpm, 4/4, un seul tempo. La rive 1 se lit en demi-temps (grosse caisse sur 1, clap sur 3, charley en doubles croches **balancées**) ; la rive 2 en temps plein (quatre temps au sol, charley en croches à contretemps, **droit**).
- **Tonalité** : Mi mineur (mesures 1–36), puis Mi♭ majeur à partir de la mesure 37 : un changement de tonalité lointain (un dièse → trois bémols), par la note commune Sol.
- **Palette par rôles**, deux palettes :
  - rive 1 : pulsation = batterie en demi-temps et charley balancé ; basse = sinus, notes longues ; harmonie = clavier triangle doux, accords tenus ; lead = « Cellule », dent de scie filtrée, sombre ; pas de texture.
  - rive 2 : pulsation = quatre temps, clap sur 2 et 4, charley à contretemps ; basse = la même piste sinus, en croches à contretemps, **pompée par la grosse caisse** ; harmonie = nappe dent de scie large, **pompée elle aussi**, et arpège carré pincé ; lead = « Chant », sinus avec écho.
  - la charnière : le Sol, tenu par le clavier de la rive 1 et par la nappe de la rive 2 qui monte.
- **Longueur** : 80 mesures.
- **Forme** : F5. Les deux fiches précédentes sont F4 « Girouette » et F3 « Lame de fond » (exclues) ; les cinq dernières : F4, F3, F10, F1, F6. Pas de profil, pas d'humeur imposée ; F0 est écartée (rien n'est dit de la forme). Parmi F2, F5, F7, F8, F9, F11, je prends F5 : elle n'a jamais servi, et son idée (une porte, pas une coupure) demande exactement ce qui vient d'arriver dans Faulk : un changement de tonalité posé à une mesure, un charley balancé sur une rive et droit sur l'autre, une nappe qui écoute la grosse caisse.

Trois contraintes :

1. **Une seule note passe la porte.** De 33 à 36 il ne reste que Sol (clavier et nappe) ; tout le reste de la rive 1 se tait avant, tout le reste de la rive 2 entre après.
2. **La cellule de trois notes est la seule mélodie.** Tierce mineure montante, puis seconde descendante, sur le rythme « . . x – x – – – | x – – x – – x – ». Rive 1 : Mi – Sol – Fa♯. Rive 2 : Sol – Si♭ – La♭ (la même tierce mineure, la seconde devenue majeure). Aucune autre idée mélodique.
3. **Le balancement ne tient qu'aux doubles croches.** Un seul device Swing, sur la piste du charley, grille de double croche : le motif de la rive 2 n'a que des croches, que le Swing laisse droites. Le changement de sensation est écrit dans les notes, pas dans un réglage.

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Swing, Filter, Echo, Reverb, Bloom, Compressor, Ceiling).

## Boucle de départ

Le clavier de la rive 1 : Mi m9 – Do maj7 – La m7 – Si m7, une mesure chacun ; Mi et Sol restent au bas de trois accords sur quatre.

```pattern notes "Clavier A" bars=4 grid=4 octave=3 key="E minor" role=chords
E3+G3+B3+F#4 - - - | E3+G3+B3+C4 - - - | E3+G3+A3+C4 - - - | D3+F#3+A3+B3 - - - |
```

La cellule : tierce mineure montante, seconde descendante ; un seul sommet (La5, à la quatrième mesure) ; la fin reste ouverte sur Fa♯.

```pattern notes "Cellule" bars=4 grid=8 octave=5 key="E minor" role=lead
. . E5 - G5 - - - | F#5 - - E5 - - B4 - | . . E5 - G5 - - - | A5 - - G5 - - F#5 - |
```

La basse de la rive 1 : fondamentales longues, une levée.

```pattern notes "Basse T1" bars=4 grid=8 octave=1 key="E minor" role=bass
E1 - - - - - . E1 | C2 - - - - - . . | A1 - - - - - . A1 | B1 - - - - B1 D2 - |
```

La batterie en demi-temps.

```pattern drums "Beat T1" bars=1 grid=16
Kick |x.........x.....|
Clap |........x.......|
```

Le charley de la rive 1 : doubles croches douces, deux accents sur des doubles croches impaires (celles que le Swing retarde).

```pattern drums "Hat T1" bars=1 grid=16
CHat |o.oxo.o.o.oxo.oo|
```

## Variations

- **Fill T1** (gén. 2, rythme) : une seule fois, mesure 24.

```pattern drums "Fill T1" bars=1 grid=16
Kick |x.........x.....|
Clap |........x...o.ox|
```

- **Clavier B** (gén. 3, harmonie) : le second cycle de la rive 1, Do maj7 – La m7 – Mi m7 tenu deux mesures ; la rive 1 s'arrête presque.

```pattern notes "Clavier B" bars=4 grid=4 octave=3 key="E minor" role=chords
E3+G3+B3+C4 - - - | E3+G3+A3+C4 - - - | E3+G3+B3+D4 - - - | - - - - |
```

- **Basse T1 fin** (gén. 4, rythme) : trois notes tenues.

```pattern notes "Basse T1 fin" bars=4 grid=4 octave=1 key="E minor" role=bass
C2 - - - | A1 - - - | E1 - - - | - - - - |
```

- **Cellule fin** (gén. 5, mélodie) : la cellule ne redescend pas : elle reste sur Sol, la note qui passera la porte.

```pattern notes "Cellule fin" bars=4 grid=8 octave=5 key="E minor" role=lead
. . E5 - G5 - - - | F#5 - - E5 - - - - | G5 - - - - - - - | - - - - - - - - |
```

- **Sol tenu** et **Bourdon** (gén. 6, forme) : la charnière. Le clavier tient Sol4 quatre mesures ; la nappe de la rive 2 monte sur Sol3 et Sol4.

```pattern notes "Sol tenu" bars=4 grid=4 octave=4 key="E minor" role=pad
G4 - - - | - - - - | - - - - | - - - - |
```

```pattern notes "Bourdon" bars=4 grid=4 octave=3 key="E minor" role=pad
G3+G4 - - - | - - - - | - - - - | - - - - |
```

- **Beat T2** (gén. 7, rythme) : quatre temps au sol, clap sur 2 et 4.

```pattern drums "Beat T2" bars=1 grid=16
Kick |x...x...x...x...|
Clap |....x.......x...|
```

- **Hat T2** (gén. 8, rythme) : croches à contretemps ; aucune double croche impaire, donc droit sous le Swing.

```pattern drums "Hat T2" bars=1 grid=16
CHat |..x...x...x...x.|
```

- **Roulement** (gén. 9, rythme) : le clap roule sur le dernier temps ; son seul dernier temps annonce la rive 2 (mesure 36), la mesure entière le sommet (mesure 52).

```pattern drums "Roulement" bars=1 grid=16
Kick |x...x...x.......|
Clap |....x.......ooxx|
```

- **Basse T2** (gén. 10, tonalité et rythme) : Mi♭ majeur ; la basse quitte les temps pour les contretemps.

```pattern notes "Basse T2" bars=4 grid=8 octave=1 key="Eb major" role=bass
. Eb2 . Eb2 . Eb2 . Eb2 | . C2 . C2 . C2 . C2 | . Ab1 . Ab1 . Ab1 . Ab1 | . Bb1 . Bb1 . Bb1 Bb1 D2 |
```

- **Arp T2** (gén. 11, son) : Mi♭ maj7 – Do m7 – La♭ maj7 – Si♭ sus4 → Si♭ ; le Mi♭ grave ne bouge qu'à la résolution.

```pattern notes "Arp T2" bars=4 grid=8 octave=4 key="Eb major" role=arp
Eb4 G4 Bb4 D5 G4 Bb4 D5 Bb4 | Eb4 G4 Bb4 C5 G4 Bb4 C5 Bb4 | Eb4 G4 Ab4 C5 G4 Ab4 C5 Ab4 | Eb4 F4 Bb4 Eb5 D4 F4 Bb4 D5 |
```

- **Nappe T2** (gén. 12, harmonie) : les mêmes accords, tenus ; le sus4 se résout à mi-mesure.

```pattern notes "Nappe T2" bars=4 grid=4 octave=3 key="Eb major" role=pad
Eb3+G3+Bb3+D4 - - - | Eb3+G3+Bb3+C4 - - - | Eb3+G3+Ab3+C4 - - - | Eb3+F3+Bb3+Eb4 - D3+F3+Bb3+D4 - |
```

- **Basse T2 B**, **Arp T2 B**, **Nappe T2 B** (gén. 13, harmonie) : le cycle du sommet, La♭ maj7 – Si♭ – Sol m7 – Do m7 : le premier cycle commencé sur son troisième accord, et Sol mineur au milieu (Sol, encore).

```pattern notes "Basse T2 B" bars=4 grid=8 octave=1 key="Eb major" role=bass
. Ab1 . Ab1 . Ab1 . Ab1 | . Bb1 . Bb1 . Bb1 . Bb1 | . G1 . G1 . G1 . G1 | . C2 . C2 . C2 D2 . |
```

```pattern notes "Arp T2 B" bars=4 grid=8 octave=4 key="Eb major" role=arp
Eb4 Ab4 C5 Eb5 Ab4 C5 Eb5 C5 | D4 F4 Bb4 D5 F4 Bb4 D5 Bb4 | D4 G4 Bb4 D5 G4 Bb4 D5 Bb4 | Eb4 G4 C5 Eb5 G4 C5 Eb5 G5 |
```

```pattern notes "Nappe T2 B" bars=4 grid=4 octave=3 key="Eb major" role=pad
Eb3+G3+Ab3+C4 - - - | D3+F3+Bb3+D4 - - - | D3+F3+G3+Bb3 - - - | Eb3+G3+Bb3+C4 - - - |
```

- **Chant** (gén. 14, mélodie) : la cellule de la rive 1 revient transformée : même rythme, Sol – Si♭ – La♭ ; la seconde phrase monte au sommet (Do6, une seule fois).

```pattern notes "Chant" bars=8 grid=8 octave=5 key="Eb major" role=melody
. . G5 - Bb5 - - - | Ab5 - - F5 - - D5 - | . . F5 - G5 - - - | Eb5 - - - - - . . |
. . G5 - Bb5 - - - | C6 - - Bb5 - - Ab5 - | G5 - - F5 - - D5 - | Eb5 - - - - - - - |
```

- **Chant fin** (gén. 15, mélodie) : la cellule seule, deux fois, qui s'arrête sur Fa : le Sol de l'accord final la résout.

```pattern notes "Chant fin" bars=4 grid=8 octave=5 key="Eb major" role=melody
. . G5 - Bb5 - - - | Ab5 - - G5 - - - - | . . G5 - Bb5 - - - | F5 - - - - - - - |
```

- **Accord fin** et **Basse fin** (gén. 16, forme) : Mi♭ add9, joué par le clavier de la rive 1, Sol en haut.

```pattern notes "Accord fin" bars=4 grid=4 octave=3 key="Eb major" role=chords
Eb3+Bb3+F4+G4 - - - | - - - - | - - - - | - - - - |
```

```pattern notes "Basse fin" bars=4 grid=4 octave=2 key="Eb major" role=bass
Eb2 - - - | - - - - | - - - - | - - - - |
```

## Arrangement

Form: F5 Deux morceaux en un

```arrangement tempo=100
section Rive1-Entree     1-8   : Clavier A, Hat T1 [from=5], Basse T1 [from=5]
section Rive1-Corps      9-24  : Beat T1 [mute=24], Fill T1 [from=24], Hat T1, Basse T1, Clavier A, Cellule
section Rive1-Fin       25-32  : Clavier B, Basse T1 fin, Cellule fin [to=29], Beat T1 [to=29], Hat T1 [to=31]
section Charniere       33-36  : Sol tenu, Bourdon, Roulement [from=36.4]
section Rive2-Corps     37-52  : Beat T2 [mute=52], Roulement [from=52], Hat T2, Basse T2, Nappe T2, Arp T2 [from=41]
section Rive2-Sommet    53-68  : Beat T2 [mute=68.4], Hat T2, Basse T2 B [mute=68.4], Arp T2 B [mute=68.4], Nappe T2 B, Chant
section Rive2-Dissout   69-76  : Arp T2, Nappe T2, Chant fin, Hat T2 [to=73], Basse T2 [to=73]
section Fin             77-80  : Accord fin, Basse fin
```

Cycles par section :

- Rive 1, entrée et corps (1–24) : Mi m9 – Do maj7 – La m7 – Si m7, une mesure chacun.
- Rive 1, fin (25–32) : Do maj7 – La m7 – Mi m7 – Mi m7 : le cycle s'immobilise sur la tonique.
- Charnière (33–36) : Sol seul.
- Rive 2, corps (37–52) et dissolution (69–76) : Mi♭ maj7 – Do m7 – La♭ maj7 – Si♭ sus4 → Si♭.
- Rive 2, sommet (53–68) : La♭ maj7 – Si♭ – Sol m7 – Do m7.
- Fin (77–80) : Mi♭ add9, Sol en haut.

Coutures :

- 8 → 9 : charley et basse sont déjà là depuis 5 ; seule la batterie et la cellule entrent.
- 24 → 25 : le Fill T1 (mesure 24) ; le charley continue à travers la ligne.
- 28 → 29 : la batterie et la cellule s'arrêtent, le charley tient deux mesures de plus (jusqu'à 30), le clavier et la basse restent sur Mi m7.
- 32 → 33 : coupure franche voulue : tout se tait, sauf Sol. C'est la porte.
- 36 → 37 : anticipation : le dernier temps du Roulement (quatre claps droits, les premières doubles croches droites du morceau) ; l'arpège n'entre qu'à 41.
- 52 → 53 : le Roulement entier ; la nappe et le charley passent la ligne.
- 68 → 69 : le quatrième temps de 68 est vide pour la batterie, la basse et l'arpège ; le chant et la nappe le traversent.
- 72 → 73 : charley et basse sortent, l'arpège reste.
- 76 → 77 : le Fa du chant se résout sur le Sol de l'accord final.

Événements uniques :

1. Mesure 24 : Fill T1, la seule variation de batterie de la rive 1.
2. Mesures 27–28 : la cellule ne redescend pas et reste sur Sol5.
3. **Structurel**, mesures 33–36 : la charnière. Une seule note pour quatre mesures, puis une autre tonalité, une autre sensation, une autre palette.
4. Mesure 36, temps 4 : quatre claps droits, seuls.
5. Mesure 68, temps 4 : un temps de vide sous le chant.
6. Mesure 77 : le clavier de la rive 1, absent depuis 36, joue le dernier accord de la rive 2 (échange de rôles).

## Automation

```automation "Cellule coupure" part="Cellule" param=cutoff curve=ease-in
9.1 55, 24.4 95 step, 25.1 75 ease-out, 28.4 45
```

La coupure du Filter de la cellule s'ouvre lentement puis vite pendant le corps de la rive 1 (700 Hz → 4 kHz), retombe d'un coup à 25 et se referme vite puis lentement : la rive 1 s'éteint par le timbre.

```automation "Nappe volume" part="Bourdon" param=volume curve=linear
33.1 60 ease-in, 36.4 105 step, 37.1 90 linear, 69.1 90 linear, 76.4 70
```

Le volume de la nappe : le bourdon monte de −20 dB à −8 dB sur la charnière (lent puis rapide), se pose à −12 dB à 37, puis recule à −16 dB pendant la dissolution. (Au premier rendu il montait de −30 à −10 dB : la charnière se lisait onze décibels sous ses voisines ; relevé après mesure, elle reste neuf décibels dessous, ce qui est voulu : une seule note passe la porte.)

```automation "Arp coupure" part="Arp T2" param=cutoff curve=ease-in
41.1 50, 52.4 100 step, 53.1 100 linear, 69.1 100 ease-out, 76.4 45
```

La coupure du Filter de l'arpège : fermé à son entrée (600 Hz), ouvert au sommet (6 kHz), refermé pendant la dissolution (500 Hz).

## Notes de finition

**Sons** (les notes existent, les sons suivent) :

- **Batterie** : Drums tel quel.
- **Charley** : Drums, précédé de **Swing** (grille double croche, 60 %). Les doubles croches impaires de Hat T1 sont retardées ; Hat T2 n'en a pas.
- **Basse** : Oscillator sinus, attaque 5 ms, relâchement 120 ms ; Filter passe-bas 900 Hz ; **Compressor avec source de détection = Batterie** (seuil −24 dB, ratio 4, attaque 1 ms, relâchement 120 ms) : en rive 2 chaque grosse caisse la creuse.
- **Clavier** : Oscillator triangle, attaque 10 ms, déclin 600 ms, maintien 50 %, relâchement 500 ms ; Reverb taille 40 %, amortissement 50 %, mélange 25 %.
- **Cellule** : Oscillator dent de scie, attaque 20 ms, relâchement 300 ms ; Filter passe-bas (automatisé) ; Echo 1/4, retour 25 %, mélange 20 % ; Reverb taille 40 %, amortissement 50 %, mélange 20 %, pré-délai 40 ms.
- **Arp** : Oscillator carré, déclin 150 ms, maintien 20 %, relâchement 100 ms ; Filter passe-bas (automatisé) ; Echo 1/8., retour 30 %, mélange 15 % ; Reverb taille 40 %, amortissement 50 %, mélange 15 %.
- **Nappe** : Oscillator dent de scie, attaque 400 ms, relâchement 1 s ; Filter passe-bas 2,5 kHz ; Bloom Ensemble, phase stéréo 150, mélange 45 %, tonalité 300 Hz ; Reverb taille 75 %, amortissement 70 %, mélange 40 % ; **Compressor avec source de détection = Batterie** (seuil −30 dB, ratio 6, relâchement 200 ms).
- **Chant** : Oscillator sinus, attaque 30 ms, relâchement 400 ms ; Echo 1/4, retour 25 %, mélange 20 % ; Reverb taille 40 %, amortissement 50 %, mélange 20 %, pré-délai 40 ms (la pièce du plan médian).
- **Master** : Compressor −12 dB ratio 2, compensation 11 dB (6 dB au premier rendu : crête −5,8 dBFS) ; Ceiling −0,3 dB.

Mix: Batterie: −10 dB, C, avant (pas de Reverb), pas de largeur, grosse caisse 40–100 Hz, clap 1–5 kHz
Mix: Charley: −18 dB, L25 (sa propre piste Drums), milieu (pas de Reverb : la piste est sèche et discrète), pas de largeur, au-dessus de 5 kHz
Mix: Basse: −6 dB, C, avant (pas de Reverb, Filter passe-bas 900 Hz), pas de largeur, 40–200 Hz
Mix: Clavier: −12 dB, C, milieu (Reverb taille 0,4 amortissement 0,5 mélange 0,25), pas de largeur, 150 Hz–2 kHz
Mix: Cellule (lead de la rive 1): −10 dB, C, bord avant de la pièce (Reverb taille 0,4 amortissement 0,5 mélange 0,2 pré-délai 0,04, Echo 1/4 retour 0,25 mélange 0,2, Filter passe-bas automatisé 700 Hz–4 kHz), pas de largeur, 500 Hz–4 kHz
Mix: Arp: −14 dB, R35, milieu (Reverb taille 0,4 amortissement 0,5 mélange 0,15, Echo 1/8. retour 0,3 mélange 0,15, Filter passe-bas automatisé), pas de largeur, 300 Hz–6 kHz
Mix: Nappe: −12 dB, C, arrière (Reverb taille 0,75 amortissement 0,7 mélange 0,4, Filter passe-bas 2,5 kHz), Bloom ensemble phase stéréo 150 mélange 0,45 tonalité 300 Hz, 150 Hz–2,5 kHz
Mix: Chant (lead de la rive 2): −7 dB (−9 dB au premier rendu, relevé après le lead check), C, bord avant de la pièce (Reverb taille 0,4 amortissement 0,5 mélange 0,2 pré-délai 0,04, Echo 1/4 retour 0,25 mélange 0,2, pas de Filter : sinus), pas de largeur, 600 Hz–2 kHz
Mono check: 1, 3 et 4 à la lecture (grosse caisse, basse et leads au centre ; le seul Bloom est sur la nappe, tonalité 300 Hz, mélange 0,45 ; l'arpège à R35 garde sa Reverb à 0,15) ; 2 sans objet (pas de paire en miroir) ; le reste à l'oreille
Lead check: mesures 53–68, là où le Chant sonne, −14,9 dBFS RMS, −16,3 sans le lead : 1,3 dB (sur les seize mesures entières : −15,1 et −16,3, soit 1,2 dB). Premier rendu, Chant à −9 dB : −15,4 et −16,3, soit 0,9 dB, lead enterré selon la règle, donc relevé de 2 dB.

Niveaux : la basse à −6 dB porte les deux rives ; la cellule (dent de scie) est 4 dB sous son fader ; le chant (sinus) était 3 dB dessous au premier rendu, où le lead check l'a mesuré enterré (0,9 dB) : il finit 1 dB sous la basse, hors de la fourchette de 2 à 4 dB de la règle des faders, parce que la mesure sur le rendu le demande (les deux règles se contredisent ici : à trancher à l'oreille) ; la batterie Drums se lit une dizaine de dB au-dessus d'un Oscillator à fader égal, d'où −10 dB.

**Humaniser** : la coupure de la cellule et de l'arpège bougent déjà ; à l'oreille, laisser dériver le déclin du clavier.

**Laissé à l'oreille** : la quantité de Swing (58 à 62 %), la profondeur du pompage, le niveau du bourdon à la mesure 36, l'équilibre entre les deux rives.

**Version suivante** : la cellule en canon avec elle-même au sommet ; un vrai changement de tempo à la porte ; une rive 2 en 6/8.

## Check

```

[notes] 'Clavier A'  bars=4 grid=4 notes=16
  OK     all 16 notes are in E minor

[notes] 'Cellule'  bars=4 grid=8 notes=10
  OK     all 10 notes are in E minor
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 5 / leaps 4, up 13 / down 11 semitones, 2.5 notes per bar

[notes] 'Basse T1'  bars=4 grid=8 notes=8
  OK     all 8 notes are in E minor
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 1 / leaps 3, up 13 / down 3 semitones, 2.0 notes per bar

[drums] 'Beat T1'  bars=1 grid=16 notes=3

[drums] 'Hat T1'  bars=1 grid=16 notes=11
  NOTE   no kick in this pattern: fine if another part carries the pulse

[drums] 'Fill T1'  bars=1 grid=16 notes=6

[notes] 'Clavier B'  bars=4 grid=4 notes=12
  OK     all 12 notes are in E minor

[notes] 'Basse T1 fin'  bars=4 grid=4 notes=3
  OK     all 3 notes are in E minor
  INFO   contour: range 8 semitones, highest note occurs 1x, steps 0 / leaps 2, up 0 / down 8 semitones, 0.8 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Cellule fin'  bars=4 grid=8 notes=5
  OK     all 5 notes are in E minor
  INFO   contour: range 3 semitones, highest note occurs 2x, steps 2 / leaps 2, up 6 / down 3 semitones, 1.2 notes per bar
  INFO   contour: the highest note repeats; a memorable line usually has a single peak

[notes] 'Sol tenu'  bars=4 grid=4 notes=1
  OK     all 1 notes are in E minor

[notes] 'Bourdon'  bars=4 grid=4 notes=2
  OK     all 2 notes are in E minor

[drums] 'Beat T2'  bars=1 grid=16 notes=6

[drums] 'Hat T2'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[drums] 'Roulement'  bars=1 grid=16 notes=8

[notes] 'Basse T2'  bars=4 grid=8 notes=17
  OK     all 17 notes are in Eb major
  INFO   contour: range 7 semitones, highest note occurs 4x, steps 1 / leaps 3, up 6 / down 7 semitones, 4.2 notes per bar

[notes] 'Arp T2'  bars=4 grid=8 notes=32
  OK     all 32 notes are in Eb major
  INFO   contour: range 13 semitones, highest note occurs 1x, steps 6 / leaps 25, up 70 / down 59 semitones, 8.0 notes per bar

[notes] 'Nappe T2'  bars=4 grid=4 notes=20
  OK     all 20 notes are in Eb major

[notes] 'Basse T2 B'  bars=4 grid=8 notes=16
  OK     all 16 notes are in Eb major
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 2 / leaps 2, up 9 / down 3 semitones, 4.0 notes per bar

[notes] 'Arp T2 B'  bars=4 grid=8 notes=32
  OK     all 32 notes are in Eb major
  INFO   contour: range 17 semitones, highest note occurs 1x, steps 0 / leaps 31, up 83 / down 67 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Nappe T2 B'  bars=4 grid=4 notes=16
  OK     all 16 notes are in Eb major

[notes] 'Chant'  bars=8 grid=8 notes=17
  OK     all 17 notes are in Eb major
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 8 / leaps 8, up 18 / down 22 semitones, 2.1 notes per bar

[notes] 'Chant fin'  bars=4 grid=8 notes=7
  OK     all 7 notes are in Eb major
  INFO   contour: range 5 semitones, highest note occurs 2x, steps 2 / leaps 3, up 6 / down 8 semitones, 1.8 notes per bar
  INFO   contour: the highest note repeats; a memorable line usually has a single peak

[notes] 'Accord fin'  bars=4 grid=4 notes=4
  OK     all 4 notes are in Eb major

[notes] 'Basse fin'  bars=4 grid=4 notes=1
  OK     all 1 notes are in Eb major

[arrangement] tempo=100
  Rive1-Entree   bars   1-8   ( 8) 3 parts
                 edits: Hat T1 [from=5]; Basse T1 [from=5]
  Rive1-Corps    bars   9-24  (16) 6 parts
                 edits: Beat T1 [mute=24]; Fill T1 [from=24]
  Rive1-Fin      bars  25-32  ( 8) 5 parts
                 edits: Cellule fin [to=29]; Beat T1 [to=29]; Hat T1 [to=31]
  Charniere      bars  33-36  ( 4) 3 parts
                 edits: Roulement [from=36.4]
  Rive2-Corps    bars  37-52  (16) 6 parts
                 edits: Beat T2 [mute=52]; Roulement [from=52]; Arp T2 [from=41]
  Rive2-Sommet   bars  53-68  (16) 6 parts
                 edits: Beat T2 [mute=68.4]; Basse T2 B [mute=68.4]; Arp T2 B [mute=68.4]
  Rive2-Dissout  bars  69-76  ( 8) 5 parts
                 edits: Hat T2 [to=73]; Basse T2 [to=73]
  Fin            bars  77-80  ( 4) 2 parts
  total 80 bars

[automation] 'Cellule coupure'  part='Cellule' cc=74 (cutoff) curve=ease-in points=4

[automation] 'Nappe volume'  part='Bourdon' cc=7 (volume) curve=linear points=5

[automation] 'Arp coupure'  part='Arp T2' cc=74 (cutoff) curve=ease-in points=5

RESULT ok
```

Chant fin : la note la plus haute (Si♭5) revient deux fois : c'est la cellule dite deux fois, voulu. Arp T2 B : que des sauts, c'est un arpège.
