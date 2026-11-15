# Qui répond ?

## Brief et contraintes

Instrumental électronique joueur et rythmique, 110 bpm, **Sol mixolydien**, 64 mesures (2 min 20). Le titre : deux voix qui se parlent. Le morceau n'est pas une échelle de densité : ses sections sont des **locuteurs**. Le lead pose une question sur les accords, sans batterie ; la basse et la batterie répondent, sans lead ; puis les deux se coupent la parole de plus en plus vite, et ne jouent ensemble qu'à la fin.

Form: F7 Appel et réponse entre sections

Profil de style : aucun (rotation morzak → drifting-cycles → aucun).

- **Tempo** : 110 bpm, 4/4. Assez lent pour que les doubles de la batterie rebondissent, assez vif pour que le 3-3-2 des accords tienne lieu de pulsation dans les appels.
- **Tonalité** : Sol mixolydien (Sol La Si Do Ré Mi Fa). Le Fa bécarre donne la couleur ; il appartient aux accords et à la basse.
- **Palette par rôles** : pulsation = accords plaqués en 3-3-2 dans les appels, batterie dans les réponses ; basse = dent de scie filtrée, courte ; harmonie = accords plaqués (carré doux, ensemble, réverbération) ; lead = carré, écho pointé, un peu de réverbération ; texture = contre-chant en arpège brisé à gauche, dans l'écho.
- **Longueur** : 64 mesures.
- **Forme** : F7 (les formes des deux derniers passages, F9 et F3, sont exclues ; F2 et F4 l'ont été juste avant). Humeur joueuse et rythmique : c'est la ligne « Suits » de F7.

Trois contraintes arbitraires :

1. **Le lead et la basse ne sonnent jamais en même temps avant la mesure 49.** Appels sans basse, réponses sans lead ; dans la Fusion ils alternent par deux mesures, dans le Hoquet par temps.
2. **Le lead n'a que cinq notes** (Sol La Si Ré Mi, la pentatonique majeure de Sol). Une seule exception, écrite : le Fa5 de la mesure 48.
3. **Pas de grosse caisse dans un appel.** Un appel est porté par les accords en 3-3-2 (et un charley ouvert à contretemps dans l'appel B).

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Filter, Echo, Reverb, Bloom, Compressor, Ceiling).

Retour d'écoute de la veille pris en compte : aucune section n'est vide (les réponses gardent des accords à contretemps, la fin est portée par le contre-chant et un accord tenu) ; les notes tenues (fins de phrase du lead, accord final) passent par la réverbération et restent sous le niveau du reste.

## Boucle de départ

La question : deux mesures, une levée de trois notes puis une tenue. Elle finit sur La, la quinte de Ré mineur, loin de la tonique.

```pattern notes "Appel A" bars=8 grid=8 octave=4 key="G mixolydian" role=lead
B . D5 B . G A . | B - - . . . . . |
A . D5 A . G A . | A - - . . . B D5 |
D5 . E5 D5 . B G . | E - - . . . . . |
A . D5 A . G E . | A - - - - - . . |
```

Les accords des appels : Sol – Fa – Do – Ré mineur, deux mesures chacun, plaqués en 3-3-2. Ce sont eux la pulsation.

```pattern notes "Accords appel" bars=8 grid=8 octave=3 key="G mixolydian" role=chords
G3+B3+D4 . . G3+B3+D4 . . G3+B3+D4 . | G3+B3+D4 . . G3+B3+D4 . . G3+B3+D4 . |
F3+A3+C4 . . F3+A3+C4 . . F3+A3+C4 . | F3+A3+C4 . . F3+A3+C4 . . F3+A3+C4 . |
G3+C4+E4 . . G3+C4+E4 . . G3+C4+E4 . | G3+C4+E4 . . G3+C4+E4 . . G3+C4+E4 . |
F3+A3+D4 . . F3+A3+D4 . . F3+A3+D4 . | F3+A3+D4 . . F3+A3+D4 . . F3+A3+D4 . |
```

La réponse : la basse parle en rythme sur un autre cycle (Mi mineur – Do – Fa – Sol) et finit sur la tonique.

```pattern notes "Réponse A" bars=8 grid=8 octave=2 key="G mixolydian" role=bass
E . E E . E . G | E . . E . B1 D . |
C . C C . C . E | C . . C . E G . |
F . F F . F . A | F . . F . A C3 . |
G . G G . G . B | G . . D . D G - |
```

```pattern drums "Beat R" bars=1 grid=16
Kick  |x.....x...x.....|
Clap  |....x.......x...|
CHat  |o.o.o.o.o.o.o.o.|
OHat  |..............x.|
```

Dans les réponses, les accords ne font que ponctuer, à contretemps des temps 2 et 4.

```pattern notes "Accords réponse" bars=8 grid=8 octave=3 key="G mixolydian" role=chords
. . . G3+B3+E4 . . . G3+B3+E4 | . . . G3+B3+E4 . . . G3+B3+E4 |
. . . G3+C4+E4 . . . G3+C4+E4 | . . . G3+C4+E4 . . . G3+C4+E4 |
. . . A3+C4+F4 . . . A3+C4+F4 | . . . A3+C4+F4 . . . A3+C4+F4 |
. . . B3+D4+G4 . . . B3+D4+G4 | . . . B3+D4+G4 . . . B3+D4+G4 |
```

## Variations

- **Appel B** (gén. 2, registre) : la même question une tierce à une quinte plus haut, sommet Sol5 à la mesure 21, fin sur Mi5 (la neuvième de Ré mineur) : plus haut, plus ouvert.

```pattern notes "Appel B" bars=8 grid=8 octave=4 key="G mixolydian" role=lead
D5 . E5 D5 . B D5 . | D5 - - . . . B D5 |
D5 . E5 D5 . A D5 . | A - - . . . D5 E5 |
G5 . E5 D5 . E5 D5 . | E5 - - . . . . . |
D5 . A D5 . E5 D5 . | E5 - - - - - . . |
```

- **Réponse B** (gén. 3, rythme et registre) : la basse ajoute des sauts d'octave.

```pattern notes "Réponse B" bars=8 grid=8 octave=2 key="G mixolydian" role=bass
E . E E3 . E . G | E . E3 E . B1 D . |
C . C C3 . C . E | C . C3 C . E G . |
F . F F3 . F . A | F . F3 F . A C3 . |
G . G G3 . G . B | G . G3 D . D G - |
```

- **Contre-chant** (gén. 4, une voix de plus) : un arpège brisé qui entre dans la réponse B, là où le lead se tait.

```pattern notes "Contre-chant" bars=8 grid=8 octave=4 key="G mixolydian" role=arp
. B E5 . B G . . | . B E5 . B G B . |
. C5 E5 . C5 G . . | . C5 E5 . C5 G C5 . |
. C5 F5 . C5 A . . | . C5 F5 . C5 A C5 . |
. D5 G5 . D5 B . . | . D5 G5 . D5 B D5 . |
```

- **Beat R fill** (gén. 5) : la mesure 16, roulement de clap, charleys coupés.

```pattern drums "Beat R fill" bars=1 grid=16
Kick  |x.....x...x.....|
Clap  |....x.......x.xx|
CHat  |o.o.o.o.o.o.....|
```

- **Beat appel** : le seul rythme permis dans un appel, un charley ouvert doux à contretemps.

```pattern drums "Beat appel" bars=1 grid=16
OHat  |..o...o...o...o.|
```

- **Beat F** (gén. 6) : la batterie de la Fusion, une grosse caisse de plus et des charleys accentués.

```pattern drums "Beat F" bars=1 grid=16
Kick  |x.....x...x..x..|
Clap  |....x.......x...|
CHat  |x.o.x.o.x.o.x.o.|
```

- **Fusion** (gén. 7, forme) : un troisième cycle (La mineur – Fa – Do – Sol, une mesure par accord). Le lead parle deux mesures, la basse répond deux mesures.

```pattern notes "Accords fusion" bars=4 grid=8 octave=3 key="G mixolydian" role=chords
A3+C4+E4 . . A3+C4+E4 . . A3+C4+E4 . | A3+C4+F4 . . A3+C4+F4 . . A3+C4+F4 . |
G3+C4+E4 . . G3+C4+E4 . . G3+C4+E4 . | G3+B3+D4 . . G3+B3+D4 . . G3+B3+D4 . |
```

```pattern notes "Lead fusion" bars=4 grid=8 octave=4 key="G mixolydian" role=lead
E5 . D5 E5 . A D5 . | D5 . A G . A - - |
. . . . . . . . | . . . . . . . . |
```

Le Mi5 du « Lead fusion » revient deux fois : décision (une cellule de notes répétées, pas une ligne à sommet).

```pattern notes "Basse fusion" bars=4 grid=8 octave=2 key="G mixolydian" role=bass
. . . . . . . . | . . . . . . . . |
C . C C3 . C E G | G . G G3 . D G - |
```

- **Hoquet** (gén. 8, le procédé structurel) : la même conversation au temps près. Le lead prend les temps 1 et 3, la basse les temps 2 et 4 ; aucune croche n'est commune.

```pattern notes "Lead hoquet" bars=4 grid=8 octave=4 key="G mixolydian" role=lead
E5 D5 . . E5 A . . | D5 A . . D5 G . . |
E5 D5 . . G5 E5 . . | D5 B . . D5 G . . |
```

```pattern notes "Basse hoquet" bars=4 grid=8 octave=2 key="G mixolydian" role=bass
. . A A . . A3 E | . . F F . . F3 C3 |
. . C C . . C3 G | . . G G . . G3 D3 |
```

- **Lead hoquet fin** : le second tour, dont la dernière mesure tient un Fa5, la seule note du lead hors de ses cinq notes (décision : c'est la septième mixolydienne, que le lead n'a jamais dite ; la Résolution lui répond).

```pattern notes "Lead hoquet fin" bars=4 grid=8 octave=4 key="G mixolydian" role=lead
E5 D5 . . E5 A . . | D5 A . . D5 G . . |
E5 D5 . . G5 E5 . . | D5 B . . F5 - - . |
```

- **Résolution** : les deux voix ensemble, enfin, sur une pédale de Sol (Sol – Do/Sol – Fa/Sol – Sol). Le thème reprend la question de l'appel A et la mène à la tonique.

```pattern notes "Thème résolu" bars=8 grid=8 octave=4 key="G mixolydian" role=lead
B . D5 B . G A . | G - - . . . D5 E5 |
D5 . A D5 . A G . | B - - . . . D5 E5 |
G5 . E5 D5 . B D5 . | E5 . D5 B . G E . |
A . D5 A . G A . | G - - - - - - - |
```

```pattern notes "Basse pédale" bars=2 grid=8 octave=2 key="G mixolydian" role=bass
G . G G . G . G3 | G . . G . G3 G . |
```

```pattern notes "Accords résolution" bars=4 grid=8 octave=3 key="G mixolydian" role=pad
G3+B3+D4 - - - - - - - | G3+C4+E4 - - - - - - - |
A3+C4+F4 - - - - - - - | G3+B3+D4 - - - - - - - |
```

- **Envoi** : le contre-chant revient seul sur la pédale, puis un accord de Fa sur Sol se pose sur Sol.

```pattern notes "Contre-chant résolu" bars=4 grid=8 octave=4 key="G mixolydian" role=arp
. D5 G5 . D5 B . . | . C5 E5 . C5 G . . |
. C5 F5 . C5 A . . | . D5 G5 . D5 B D5 . |
```

```pattern notes "Accord fin" bars=4 grid=8 octave=3 key="G mixolydian" role=pad
A3+C4+F4 - - - - - - - | - - - - - - - - |
G3+B3+D4 - - - - - - - | - - - - - - - - |
```

## Arrangement

Form: F7 Appel et réponse entre sections

```arrangement tempo=110
section Appel A      1-8   : Accords appel, Appel A
section Réponse A    9-16  : Beat R [to=16], Beat R fill [from=16], Réponse A, Accords réponse
section Appel B     17-24  : Accords appel [mute=24], Appel B, Beat appel
section Réponse B   25-32  : Beat R, Réponse B, Accords réponse, Contre-chant
section Fusion      33-40  : Beat F [mute=40], Accords fusion, Lead fusion, Basse fusion
section Hoquet      41-48  : Beat F, Accords fusion, Lead hoquet [to=45], Lead hoquet fin [from=45], Basse hoquet [to=48.3]
section Résolution  49-56  : Beat F, Accords résolution, Thème résolu, Basse pédale
section Envoi       57-64  : Beat appel [to=61], Accords résolution [to=61], Accord fin [from=61], Basse pédale [to=61], Contre-chant résolu [to=63]
```

Cycles d'accords par section :

- Appel A, Appel B : Sol – Fa – Do – Rém (I – ♭VII – IV – v), deux mesures par accord ; finit hors de la tonique.
- Réponse A, Réponse B : Mim – Do – Fa – Sol (vi – IV – ♭VII – I), deux mesures par accord ; finit sur la tonique.
- Fusion, Hoquet : Lam – Fa – Do – Sol (ii – ♭VII – IV – I), une mesure par accord.
- Résolution, Envoi : Sol – Do/Sol – Fa/Sol – Sol sur pédale de Sol ; puis Fa/Sol → Sol (61–64).

Arc : le sommet est la Résolution (49–56, 77 à 88 %), parce que c'est le seul moment où tout le monde joue ; avant, l'intensité vient de la vitesse de l'échange (8 mesures, 2 mesures, 1 temps), pas du nombre de parties.

Coutures :

- 8 → 9 : coupe franche voulue (l'autre locuteur prend la parole) ; le La tenu du lead s'arrête deux croches avant la barre.
- 16 → 17 : anticipation, roulement de clap sur 16.4 ; les charleys se taisent dès 16.4.
- 24 → 25 : les accords se taisent la mesure 24 ; le Mi5 du lead reste seul avec le charley ouvert, dans l'écho (mélange de l'écho monté à 24.1).
- 32 → 33 : la basse tient son Sol sur la dernière croche de 32 ; les accords changent de cycle sur 33.1.
- 40 → 41 : la batterie se tait la mesure 40 (la basse répond seule sur les accords), et revient sur 41.1 avec le hoquet.
- 48 → 49 : le Fa5 tenu de 48.3, la basse muette sur 48.3 et 48.4, puis tout le monde sur 49.1.
- 56 → 57 : le Sol tenu du thème passe la mesure 56 entière ; la batterie se réduit au charley ouvert sur 57.1.
- 60 → 61 : basse, charley et accords tenus s'arrêtent ; l'accord de Fa sur Sol entre, le contre-chant continue deux mesures.

Événements uniques :

1. 16.4 : roulement de clap (une fois).
2. 24 : une mesure sans accords, le Mi5 du lead seul dans l'écho (structurel : la question reste en l'air).
3. 40 : la batterie se tait une mesure, la basse répond seule (structurel).
4. 48.3 : le Fa5 du lead, sa seule note hors des cinq, tenu un temps et demi.
5. 49 : première fois que le lead et la basse jouent ensemble (structurel : la contrainte 1 tombe ici, c'est écrit).
6. 61 : l'accord de Fa sur Sol tenu deux mesures sans rien dessous que le contre-chant, entendu nulle part ailleurs ainsi.

## Automation

La coupure du filtre de la basse : chaque réponse s'ouvre en parlant (lente puis rapide), plus haut la seconde fois ; elle se referme en douceur dans l'Envoi (rapide puis lente).

```automation "Coupure basse" part="Réponse A" param=cutoff curve=linear
9.1 50 ease-in, 16.4 85 step, 25.1 60 ease-in, 32.4 100 step, 57.1 100 ease-out, 60.4 45
```

Le volume des accords : pleins dans les appels, en retrait dans les réponses (paliers aux coutures : ce sont des prises de parole, pas des fondus), puis une descente en S sous le dernier accord.

```automation "Volume accords" part="Accords appel" param=volume curve=step
1.1 100, 9.1 80, 17.1 105, 25.1 80, 33.1 100, 61.1 100 smooth, 64.4 70
```

L'écho du lead : monté d'un coup pour la note tenue de la mesure 24, redescendu à la réponse.

```automation "Echo lead" part="Appel B" param=delay curve=step
17.1 25, 24.1 70, 25.1 25
```

Dans Faulk : « Coupure basse » = Fréquence de coupure du Filter de la piste Basse ; « Volume accords » = Volume de la piste Accords ; « Echo lead » = Mélange de l'Echo de la piste Lead.

## Notes de finition

Sons : Lead = Oscillator carré, attaque 5 ms, relâchement 200 ms, Filter passe-bas 4 kHz, Echo 1/8. retour 35 % mélange 25 %, Reverb mélange 15 % pré-délai 30 ms. Basse = dent de scie, relâchement 80 ms, Filter passe-bas automatisé (≈ 400 Hz à 2 kHz). Accords = carré, attaque 10 ms, relâchement 300 ms, Filter passe-bas 2,5 kHz, Bloom Ensemble, Reverb 25 %. Contre-chant = carré court, Echo 1/4 retour 45 % mélange 30 %, Reverb 35 %. Drums tels quels.

Mix: Lead: C, front (Reverb size 0.5 mix 0.15 predelay 0.03, Echo eighth_dotted feedback 0.35 mix 0.25, Filter lowpass 4 kHz), no width, 400 Hz–5 kHz (G4–G5)
Mix: Basse: C, front (no Reverb, Filter lowpass 400 Hz–2 kHz automated), no width, 60–250 Hz (B1–G3)
Mix: Accords: C, middle (Reverb size 0.5 damping 0.5 mix 0.25, Filter lowpass 2.5 kHz), Bloom ensemble stereo_phase 150 depth 40 % tone 300 Hz mix 0.45, 170 Hz–2.5 kHz (F3–G4)
Mix: Contre-chant: L40, back (Reverb size 0.7 damping 0.7 mix 0.35, Echo quarter feedback 0.45 mix 0.3), no width, 400 Hz–3 kHz (G4–G5, only while the lead is silent)
Mix: Drums: C, front (no Reverb), no width, kick 50–100 Hz, hats above 5 kHz
Mono check: 1, 3 and 4 by reading (kick, bass and lead at C; Bloom only on the chords with tone 300 Hz and mix 0.45; the contre-chant at L40 keeps both sides of its reverb); 2 does not apply (no mirrored pair); the rest is left to the ear.

Humanisation : aucune dans la fiche ; les charleys fantômes (vélocité 60) et le filtre de la basse portent le mouvement. Laissé à l'oreille : le niveau du Fa5 de 48, la longueur de l'écho sur la mesure 24, l'équilibre basse / grosse caisse. Une seconde version pourrait essayer : la réponse B allongée à dix mesures, le hoquet resserré à la croche sur les deux dernières mesures, un second timbre pour le lead de l'appel B.

## Check

```
[notes] 'Appel A'  bars=8 grid=8 notes=26
  OK     all 26 notes are in G mixolydian
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 9 / leaps 14, up 36 / down 38 semitones, 3.2 notes per bar

[notes] 'Accords appel'  bars=8 grid=8 notes=72
  OK     all 72 notes are in G mixolydian

[notes] 'Réponse A'  bars=8 grid=8 notes=36
  OK     all 36 notes are in G mixolydian
  INFO   contour: range 13 semitones, highest note occurs 1x, steps 2 / leaps 17, up 37 / down 34 semitones, 4.5 notes per bar

[drums] 'Beat R'  bars=1 grid=16 notes=14

[notes] 'Accords réponse'  bars=8 grid=8 notes=48
  OK     all 48 notes are in G mixolydian

[notes] 'Appel B'  bars=8 grid=8 notes=28
  OK     all 28 notes are in G mixolydian
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 13 / leaps 12, up 38 / down 36 semitones, 3.5 notes per bar

[notes] 'Réponse B'  bars=8 grid=8 notes=40
  OK     all 40 notes are in G mixolydian
  INFO   contour: range 20 semitones, highest note occurs 2x, steps 2 / leaps 32, up 133 / down 130 semitones, 5.0 notes per bar

[notes] 'Contre-chant'  bars=8 grid=8 notes=36
  OK     all 36 notes are in G mixolydian
  INFO   contour: range 12 semitones, highest note occurs 2x, steps 2 / leaps 32, up 71 / down 68 semitones, 4.5 notes per bar

[drums] 'Beat R fill'  bars=1 grid=16 notes=13

[drums] 'Beat appel'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[drums] 'Beat F'  bars=1 grid=16 notes=14

[notes] 'Accords fusion'  bars=4 grid=8 notes=36
  OK     all 36 notes are in G mixolydian

[notes] 'Lead fusion'  bars=4 grid=8 notes=9
  OK     all 9 notes are in G mixolydian
  INFO   contour: range 9 semitones, highest note occurs 2x, steps 4 / leaps 3, up 9 / down 16 semitones, 2.2 notes per bar
  INFO   contour: the highest note repeats; a memorable line usually has a single peak

[notes] 'Basse fusion'  bars=4 grid=8 notes=11
  OK     all 11 notes are in G mixolydian
  INFO   contour: range 19 semitones, highest note occurs 1x, steps 0 / leaps 7, up 36 / down 29 semitones, 2.8 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Lead hoquet'  bars=4 grid=8 notes=16
  OK     all 16 notes are in G mixolydian
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 4 / leaps 11, up 29 / down 38 semitones, 4.0 notes per bar

[notes] 'Basse hoquet'  bars=4 grid=8 notes=16
  OK     all 16 notes are in G mixolydian
  INFO   contour: range 21 semitones, highest note occurs 1x, steps 1 / leaps 9, up 49 / down 44 semitones, 4.0 notes per bar

[notes] 'Lead hoquet fin'  bars=4 grid=8 notes=15
  OK     all 15 notes are in G mixolydian
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 4 / leaps 10, up 32 / down 31 semitones, 3.8 notes per bar

[notes] 'Thème résolu'  bars=8 grid=8 notes=32
  OK     all 32 notes are in G mixolydian
  INFO   contour: range 15 semitones, highest note occurs 1x, steps 12 / leaps 19, up 48 / down 52 semitones, 4.0 notes per bar

[notes] 'Basse pédale'  bars=2 grid=8 notes=9
  OK     all 9 notes are in G mixolydian
  INFO   contour: range 12 semitones, highest note occurs 2x, steps 0 / leaps 4, up 24 / down 24 semitones, 4.5 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Accords résolution'  bars=4 grid=8 notes=12
  OK     all 12 notes are in G mixolydian

[notes] 'Contre-chant résolu'  bars=4 grid=8 notes=17
  OK     all 17 notes are in G mixolydian
  INFO   contour: range 12 semitones, highest note occurs 2x, steps 1 / leaps 15, up 33 / down 33 semitones, 4.2 notes per bar

[notes] 'Accord fin'  bars=4 grid=8 notes=6
  OK     all 6 notes are in G mixolydian

[arrangement] tempo=110
  Appel A        bars   1-8   ( 8) 2 parts
  Réponse A      bars   9-16  ( 8) 4 parts
                 edits: Beat R [to=16]; Beat R fill [from=16]
  Appel B        bars  17-24  ( 8) 3 parts
                 edits: Accords appel [mute=24]
  Réponse B      bars  25-32  ( 8) 4 parts
  Fusion         bars  33-40  ( 8) 4 parts
                 edits: Beat F [mute=40]
  Hoquet         bars  41-48  ( 8) 5 parts
                 edits: Lead hoquet [to=45]; Lead hoquet fin [from=45]; Basse hoquet [to=48.3]
  Résolution     bars  49-56  ( 8) 4 parts
  Envoi          bars  57-64  ( 8) 5 parts
                 edits: Beat appel [to=61]; Accords résolution [to=61]; Accord fin [from=61]; Basse pédale [to=61]; Contre-chant résolu [to=63]
  total 64 bars

[automation] 'Coupure basse'  part='Réponse A' cc=74 (cutoff) curve=linear points=6

[automation] 'Volume accords'  part='Accords appel' cc=7 (volume) curve=step points=7

[automation] 'Echo lead'  part='Appel B' cc=94 (delay) curve=step points=3

RESULT ok
```
