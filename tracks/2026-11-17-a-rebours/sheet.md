# À rebours

## Brief et contraintes

Instrumental électronique mélodique, lumineux puis nostalgique, 108 bpm, **Fa majeur** puis **Sol majeur** après une hausse tardive, 80 mesures (2 min 58). Le morceau commence par son sommet : le motif est donné d'emblée, tout le reste le commente, et l'harmonie voyage sous lui sans qu'il change une note.

Form: F1 Arc inversé

Profil de style : **drifting-cycles** (rotation morzak → drifting-cycles → aucun).

- **Tempo** : 108 bpm, 4/4 (lecture « mid » 100–112 du profil, lecture directe, pas de demi-temps).
- **Tonalité** : Fa majeur (Fa Sol La Si♭ Do Ré Mi) ; le relatif (Ré mineur) visité au dépouillement ; hausse d'un ton à la mesure 53, Sol majeur (Sol La Si Do Ré Mi Fa♯) jusqu'à la fin.
- **Palette par rôles** : pulsation = batterie (grosse caisse sur chaque temps, clap, charley) ; basse = sub propre (sinus), capable de tenir une pédale ; harmonie = nappe chaude et large, accords enrichis (add9, maj7, m7, sus4) ; couche pincée = arpège court (carré), contre-chant dans la repousse ; lead = dent de scie doublée (chorus), porte le motif de sept notes puis la phrase chantée.
- **Longueur** : 80 mesures.
- **Forme** : F1. Les deux passages précédents sont F6 et F7 (exclus) ; le profil nomme F4, F9, F10 et F1 ; F4 et F9 sont dans les cinq dernières fiches, F1 n'a jamais servi et son second sommet « le même motif sur une nouvelle image d'accords » est la signature du profil.

Trois contraintes, dont deux gestes du profil :

1. *(profil, geste 5 et signature)* **le motif ne change jamais ses notes** : sept notes, deux mesures, réharmonisées par chaque section (cycle P, cycle S, accord sus tenu, cycle Q, puis D), seulement transposées d'un ton à la hausse.
2. *(profil, gestes 2, 3 et 4)* **une pédale puis une hausse tardive** : la basse tient Fa de 25 à 39 sous des accords qui bougent et sous un Dosus4 tenu huit mesures ; elle ne bouge que sur le premier temps du second sommet (41.1) ; la hausse de +2 demi-tons tombe à 53 (65 %), après une mesure amincie (52) et avec une note du lead tenue à travers la coupe.
3. *(la mienne)* **aucun cycle d'accords ne sert à deux sections** : P, S, pédale et sus, Q, Q haussé, D ; chaque cycle garde un accord du précédent comme ancre.

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Filter, Echo, Reverb, Bloom, Compressor, Ceiling). Pas de compression en sidechain ni de montée de bruit (voir les notes de finition).

## Catalogue d'attributs

- Tempo : 108 bpm, lecture « mid », croches droites.
- Mode et harmonie : majeur, relatif mineur visité au milieu ; cycles de 3 ou 4 accords d'une ou deux mesures ; accords enrichis par défaut (add9, maj7, m7, sus4) ; une section à pédale de tonique ; une hausse tardive d'un ton.
- Son : un lead doublé et désaccordé, une couche pincée arpégée, une nappe chaude et large, un sub propre.
- Rythme : grosse caisse sur chaque temps ; un seul roulement, avant le second sommet.
- Mélodie : un motif court de sept notes donné à la première mesure, varié par les accords qui passent dessous ; une longue phrase chantée dans le dernier tiers (57–64).
- Forme : par sections, F1 : sommet d'entrée, dépouillement, repousse, second sommet modifié, dissolution, dernière voix.
- Mix : bas-médium plein, sub propre, haut présent, nappe large, basse et lead au centre.

## Boucle de départ

Le motif d'abord : sept notes, un seul sommet (Ré5), qui retombe sur sa première note.

```pattern notes "Hook" bars=2 grid=8 octave=4 key="F major" role=hook
A4 . C5 . D5 - C5 . | A4 . G4 . A4 - - . |
```

Le cycle P du sommet d'entrée : Fa add9 – Rém7 – Si♭maj7 – Do add9, deux mesures par accord (harmonie lente).

```pattern notes "Nappe P" bars=8 grid=4 octave=3 key="F major" role=pad
F3+A3+C4+G4 - - - | - - - - | F3+A3+C4+D4 - - - | - - - - |
F3+A3+Bb3+D4 - - - | - - - - | E3+G3+C4+D4 - - - | - - - - |
```

La basse : la fondamentale, une croche pointée d'avance, une levée vers l'accord suivant.

```pattern notes "Basse P" bars=8 grid=8 octave=2 key="F major" role=bass
F2 - - F2 . . F2 . | F2 - - F2 . C2 F2 . |
D2 - - D2 . . D2 . | D2 - - D2 . A1 D2 . |
Bb1 - - Bb1 . . Bb1 . | Bb1 - - Bb1 . F2 Bb1 . |
C2 - - C2 . . C2 . | C2 - - C2 . G1 E2 . |
```

La couche pincée : un arpège par accord, avec un trou à la fin de chaque mesure.

```pattern notes "Pluck P" bars=8 grid=8 octave=4 key="F major" role=arp
F4 C5 G5 C5 F4 C5 G5 . | F4 C5 G5 C5 A4 C5 . . |
D4 A4 F5 A4 D4 A4 F5 . | D4 A4 F5 A4 C5 A4 . . |
D4 A4 F5 A4 D4 Bb4 F5 . | D4 Bb4 F5 Bb4 D5 A4 . . |
E4 G4 D5 G4 E4 G4 D5 . | E4 G4 E5 D5 C5 G4 . . |
```

```pattern drums "Beat" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |o.x.o.x.o.x.o.x.|
```

## Variations

- **Nappe S** (gén. 2, harmonie) : le relatif mineur, cycle S = Rém7 – Solm7 – Si♭maj7 – Lam7, deux mesures par accord ; ancres : Rém7 et Si♭maj7.

```pattern notes "Nappe S" bars=8 grid=4 octave=3 key="F major" role=pad
D3+F3+A3+C4 - - - | - - - - | D3+F3+G3+Bb3 - - - | - - - - |
D3+F3+A3+Bb3 - - - | - - - - | E3+G3+A3+C4 - - - | - - - - |
```

- **Basse pédale** (gén. 3, forme) : Fa tenu en pulsation, une mesure rejouée de 25 à 39.

```pattern notes "Basse pédale" bars=1 grid=8 octave=2 key="F major" role=bass
F2 . F2 . F2 . . F2 |
```

- **Contre** (gén. 4, mélodie et rythme) : le contre-chant de la repousse, dans les trous de la pédale (hoquet), dessine Si♭maj7 – Do – Rém7 – Do au-dessus du Fa tenu, un accord par mesure (harmonie rapide).

```pattern notes "Contre" bars=4 grid=8 octave=5 key="F major" role=arp
. D5 . A4 . Bb4 D5 . | . E5 . G4 . C5 E5 . |
. F5 . A4 . D5 F5 . | . E5 . G4 . C5 G5 - |
```

- **Nappe sus** (gén. 5, harmonie) : Dosus4 tenu, sans résolution avant 41.

```pattern notes "Nappe sus" bars=4 grid=4 octave=3 key="F major" role=pad
C3+F3+G3+C4 - - - | - - - - | - - - - | - - - - |
```

- **Beat charley** (gén. 6, son) : la pulsation sans grosse caisse ni clap.

```pattern drums "Beat charley" bars=1 grid=16
CHat  |o.x.o.x.o.x.o.x.|
```

- **Beat roulement** (gén. 7, rythme) : le seul roulement, mesure 40.

```pattern drums "Beat roulement" bars=1 grid=16
Kick  |x...x...........|
Clap  |....x...x.x.xxxx|
CHat  |o.x.o.x.........|
```

- **Cycle Q** (gén. 8, harmonie) : le second sommet, Si♭maj7 (deux mesures) – Lam7 – Rém7 (une mesure chacun) : il ne touche jamais l'accord de tonique ; ancres : Si♭maj7 et Rém7.

```pattern notes "Nappe Q" bars=4 grid=4 octave=3 key="F major" role=pad
F3+A3+Bb3+D4 - - - | - - - - | E3+G3+A3+C4 - - - | F3+A3+C4+D4 - - - |
```

```pattern notes "Basse Q" bars=4 grid=8 octave=2 key="F major" role=bass
Bb1 - - Bb1 . . Bb1 . | Bb1 - - Bb1 . D2 F2 . |
A1 - - A1 . C2 E2 . | D2 - - D2 . A1 C2 . |
```

```pattern notes "Pluck Q" bars=4 grid=8 octave=4 key="F major" role=arp
Bb3 F4 D5 F4 A4 F4 D5 . | Bb3 F4 D5 F4 A4 D5 . . |
A3 E4 C5 E4 G4 E4 C5 . | D4 A4 F5 A4 C5 A4 F5 . |
```

```pattern drums "Beat ouvert" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |o.x.o.x.o.x.o...|
OHat  |..............x.|
```

- **Hausse** (gén. 9, tonalité) : les quatre motifs du cycle Q un ton plus haut (Domaj7 – Sim7 – Mim7), et le motif.

```pattern notes "Nappe Q haussé" bars=4 grid=4 octave=3 key="G major" role=pad
G3+B3+C4+E4 - - - | - - - - | F#3+A3+B3+D4 - - - | G3+B3+D4+E4 - - - |
```

```pattern notes "Basse Q haussé" bars=4 grid=8 octave=2 key="G major" role=bass
C2 - - C2 . . C2 . | C2 - - C2 . E2 G2 . |
B1 - - B1 . D2 F#2 . | E2 - - E2 . B1 D2 . |
```

```pattern notes "Pluck Q haussé" bars=4 grid=8 octave=4 key="G major" role=arp
C4 G4 E5 G4 B4 G4 E5 . | C4 G4 E5 G4 B4 E5 . . |
B3 F#4 D5 F#4 A4 F#4 D5 . | E4 B4 G5 B4 D5 B4 G5 . |
```

```pattern notes "Hook haussé" bars=2 grid=8 octave=4 key="G major" role=hook
B4 . D5 . E5 - D5 . | B4 . A4 . B4 - - . |
```

- **Hook pont** (gén. 10, forme) : deux énoncés en Fa, le dernier La tenu à travers la coupe (52.3 → 53.2), puis le motif reprend en Sol à son sommet. Sans `key=` : le clip est à cheval sur les deux tonalités.

```pattern notes "Hook pont" bars=8 grid=8 octave=4 role=hook
A4 . C5 . D5 - C5 . | A4 . G4 . A4 - - . |
A4 . C5 . D5 - C5 . | A4 . G4 . A4 - - - |
- - - - E5 - D5 . | B4 . A4 . B4 - - . |
B4 . D5 . E5 - D5 . | B4 . A4 . B4 - - . |
```

- **Chant** (gén. 11, mélodie) : la longue phrase du dernier tiers, huit mesures sur deux tours du cycle haussé, sommet Si5 une seule fois (63.4).

```pattern notes "Chant" bars=8 grid=8 octave=5 key="G major" role=lead
E5 - - D5 E5 - G5 - | - - F#5 - E5 - D5 - |
D5 - - B4 D5 - A5 - | - - G5 - E5 - . . |
E5 - - D5 E5 - G5 - | - - A5 - G5 - F#5 - |
A5 - - F#5 A5 - B5 - | - - A5 - G5 - E5 - |
```

- **Cycle D** (gén. 12, harmonie) : la dissolution, Mim7 – Domaj7, deux mesures par accord ; ancres : les deux accords viennent du cycle haussé, sans le Sim7. Le morceau finit sur Domaj7 (IV), non résolu.

```pattern notes "Nappe D" bars=4 grid=4 octave=3 key="G major" role=pad
G3+B3+D4+E4 - - - | - - - - | G3+B3+C4+E4 - - - | - - - - |
```

```pattern notes "Basse D" bars=4 grid=4 octave=2 key="G major" role=bass
E2 - - - | - - - . | C2 - - - | - - - . |
```

Dispositif structurel : le hoquet entre la basse pédale (pas 1, 3, 5, 8) et le contre-chant (pas 2, 4, 6, 7) ; l'harmonie voyageuse (six images d'accords pour un seul motif) ; une décision sur le silence (17.1 : batterie et basse disparaissent ; 52 : mesure amincie).

Compte : 23 motifs, dont 4 sont la copie transposée d'un autre (« haussé ») ; 19 matériaux distincts.

## Arrangement

Form: F1 Arc inversé

```arrangement tempo=108
section Sommet         1-16  : Beat, Basse P, Nappe P, Pluck P, Hook
section Dépouillement 17-24  : Nappe S, Hook
section Repousse      25-32  : Beat charley, Basse pédale, Contre
section Repousse 2    33-40  : Beat [mute=40], Beat roulement [from=40], Basse pédale [to=40], Contre, Nappe sus, Hook [from=37]
section Sommet II     41-48  : Beat ouvert, Basse Q, Nappe Q, Pluck Q, Hook
section Bascule       49-56  : Beat ouvert [mute=52], Basse Q [to=52], Basse Q haussé [from=53], Nappe Q [to=53], Nappe Q haussé [from=53], Pluck Q [to=52], Pluck Q haussé [from=53], Hook pont
section Sommet haussé 57-64  : Beat ouvert, Basse Q haussé, Nappe Q haussé, Pluck Q haussé, Chant
section Dissolution   65-76  : Beat [to=69], Beat charley [from=69 to=73], Basse D [to=73], Nappe D, Hook haussé
section Dernière voix 77-80  : Nappe D, Hook haussé [to=79]
```

Cycles d'accords par section :

- Sommet (1–16) : cycle P, Fa add9 – Rém7 – Si♭maj7 – Do add9, deux mesures par accord.
- Dépouillement (17–24) : cycle S, Rém7 – Solm7 – Si♭maj7 – Lam7, deux mesures par accord (relatif mineur).
- Repousse (25–40) : pédale de Fa ; au-dessus Si♭maj7 – Do – Rém7 – Do, une mesure chacun (contre-chant), puis Dosus4 tenu de 33 à 40.
- Sommet II (41–52) : cycle Q, Si♭maj7 (2) – Lam7 – Rém7 ; le sus se résout sur 41.1, la basse quitte Fa.
- Sommet haussé (53–64) : cycle Q un ton plus haut, Domaj7 (2) – Sim7 – Mim7, en Sol majeur.
- Dissolution et dernière voix (65–80) : cycle D, Mim7 – Domaj7, deux mesures par accord ; fin sur Domaj7.

Arc inversé : le moment le plus fort est la première mesure ; le dépouillement retire la batterie et la basse d'un coup ; la repousse reconstruit par la pédale, le hoquet et le filtre ; le second sommet redit le motif sur une autre image, puis un ton plus haut avec la phrase chantée ; la dissolution retire les parties dans un autre ordre que leur entrée (pincé à 65, grosse caisse à 69, basse et charley à 73) ; la dernière voix est le motif sur un son assourdi, puis l'accord seul.

Coutures :

- 16 → 17 : coupe franche, la batterie, la basse et l'arpège disparaissent ; le motif continue, le filtre du lead commence à se fermer.
- 24 → 25 : le motif se tait ; la pédale et le charley entrent sur 25.1, le contre-chant sur la deuxième croche.
- 32 → 33 : la grosse caisse revient, la nappe entre en sus sous le volume qui monte.
- 36 → 37 : le motif revient sur l'accord sus (anticipation du second sommet).
- 40 → 41 : la basse se tait à la mesure 40, roulement de clap sur 40.3 ; sur 41.1 la basse joue Si♭, le sus se résout.
- 52 → 53 : mesure 52 amincie (ni batterie, ni basse, ni arpège) ; le La du lead tenu de 52.3 à 53.2 ; tout reprend un ton plus haut sur 53.1.
- 56 → 57 : le motif laisse la place à la phrase chantée.
- 64 → 65 : l'arpège sort ; le motif revient sur Mim7.
- 76 → 77 : le filtre du lead tombe ; le motif une dernière fois, puis Domaj7 seul.

Événements uniques :

1. 17.1 : batterie, basse et arpège disparaissent d'un coup après seize mesures de sommet (structurel).
2. 37.1 : le motif sur l'accord sus tenu, la seule fois où il chante sur la pédale.
3. 40.3 : le roulement de clap, le seul du morceau.
4. 41.1 : la basse quitte Fa pour la première fois depuis 25 (la signature du profil).
5. 52–53 : la mesure amincie, la note tenue à travers la coupe et la hausse d'un ton (structurel).
6. 63.4 : le Si5 de la phrase chantée, la note la plus haute du morceau.

## Automation

La coupure du filtre du lead : ouverte au sommet, elle se ferme vite puis lentement pendant le dépouillement, se rouvre lentement puis vite avec le retour du motif, se referme en S pendant la dissolution et tombe pour la dernière voix (le « son assourdi »).

```automation "Coupure lead" part="Hook" param=cutoff curve=linear
1.1 100 step, 17.1 100 ease-out, 24.4 55 step, 37.1 60 ease-in, 41.1 105 step, 65.1 105 smooth, 76.4 60 step, 77.1 45
```

La coupure du filtre de la couche pincée : fermée au début de la repousse, elle s'ouvre lentement puis vite jusqu'au roulement.

```automation "Coupure pluck" part="Contre" param=cutoff curve=linear
1.1 90 step, 25.1 40 ease-in, 40.4 95 step, 41.1 100
```

Le volume de la nappe : en retrait, il gonfle sous l'accord sus et retombe au second sommet.

```automation "Volume nappe" part="Nappe sus" param=volume curve=linear
1.1 80 step, 33.1 60 ease-in, 40.4 100 step, 41.1 80
```

Dans Faulk : « Coupure lead » = Fréquence de coupure du Filter de la piste Lead ; « Coupure pluck » = Fréquence de coupure du Filter de la piste Pluck ; « Volume nappe » = Volume de la piste Nappe.

## Notes de finition

Sons : Lead = Oscillator dent de scie, relâchement 250 ms, Bloom Chorus (le doublage désaccordé), Filter passe-bas automatisé (≈ 700 Hz à 6 kHz), Echo 1/8. retour 35 % mélange 20 %, Reverb mélange 20 %. Pluck = carré, maintien 0 %, déclin 180 ms, relâchement 150 ms, Filter passe-bas automatisé (≈ 500 Hz à 5 kHz), Echo 1/8. mélange 25 %. Nappe = dent de scie, attaque 300 ms, relâchement 800 ms, Filter passe-bas 1,8 kHz, Bloom Ensemble, Reverb taille 70 % mélange 40 %. Basse = sinus (ou triangle), relâchement 80 ms, sans effet. Drums tels quels. Master : Compressor doux, Ceiling −0,3 dB.

Ce que le profil demande et que la fiche laisse : le pompage par sidechain (à faire par un Compressor déclenché par la grosse caisse sur la nappe, si Faulk le permet), les montées de bruit filtré (avant 41 et 53), le swing sur les charleys.

Mix: Drums: C, front (no Reverb), no width, kick 50–100 Hz, hats above 5 kHz
Mix: Basse: C, front (no Reverb, no effect), no width, 55–100 Hz (G1–G2)
Mix: Nappe: C, back (Reverb size 0.7 mix 0.4, Filter lowpass 1.8 kHz), Bloom ensemble stereo_phase 150 mix 0.45, 130 Hz–1.8 kHz (C3–G4)
Mix: Pluck: R25, middle (Echo eighth_dotted feedback 0.4 mix 0.25, Filter lowpass 500 Hz–5 kHz automated, no Reverb), no width, 220 Hz–4 kHz (A3–G5)
Mix: Lead: C, front to middle (Reverb size 0.5 mix 0.2, Echo eighth_dotted feedback 0.35 mix 0.2, Filter lowpass 700 Hz–6 kHz automated), Bloom chorus mix 0.3, 390 Hz–6 kHz (G4–B5)
Mono check: 1, 3 and 4 by reading (kick, bass and lead at C; Bloom ensemble only on the pad, chorus at mix 0.3 on the lead; the pluck at R25 has an echo but no reverb, nothing is hard-panned); 2 does not apply (no mirrored pair); the rest is left to the ear.

Humanisation : aucune dans la fiche ; les charleys fantômes (vélocité 60) et les filtres portent le mouvement. Laissé à l'oreille : le niveau du sub contre la grosse caisse, la durée du trou de la mesure 52, le niveau du lead assourdi de la dernière voix. Une seconde version pourrait essayer : la hausse d'une tierce mineure au lieu d'un ton, le motif à la basse dans la dissolution, un demi-temps de batterie dans la repousse.

Profil : gardé = la lecture « mid », le majeur avec visite du relatif, les cycles de 3 ou 4 accords, un nouveau cycle par section avec une ancre, les accords enrichis, la pédale de tonique, l'accord sus résolu au sommet, la hausse tardive à 65 % avec mesure amincie et note tenue, le motif réharmonisé, la phrase chantée du dernier tiers, la signature (basse tenue qui bouge sur le premier accord de la section suivante ; la même mélodie sur d'autres accords). Plié = l'introduction sans accords (F1 ouvre sur le sommet ; la repousse 25–32 en tient lieu : arpège et basse seuls). Laissé = le sidechain, les montées de bruit, le swing des charleys.

## Check

```

[notes] 'Hook'  bars=2 grid=8 notes=7
  OK     all 7 notes are in F major
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 4 / leaps 2, up 7 / down 7 semitones, 3.5 notes per bar

[notes] 'Nappe P'  bars=8 grid=4 notes=16
  OK     all 16 notes are in F major

[notes] 'Basse P'  bars=8 grid=8 notes=28
  OK     all 28 notes are in F major
  INFO   contour: range 10 semitones, highest note occurs 7x, steps 1 / leaps 10, up 28 / down 29 semitones, 3.5 notes per bar

[notes] 'Pluck P'  bars=8 grid=8 notes=52
  OK     all 52 notes are in F major
  INFO   contour: range 17 semitones, highest note occurs 3x, steps 2 / leaps 49, up 174 / down 172 semitones, 6.5 notes per bar

[drums] 'Beat'  bars=1 grid=16 notes=14

[notes] 'Nappe S'  bars=8 grid=4 notes=16
  OK     all 16 notes are in F major

[notes] 'Basse pédale'  bars=1 grid=8 notes=4
  OK     all 4 notes are in F major
  INFO   contour: range 0 semitones, highest note occurs 4x, steps 0 / leaps 0, up 0 / down 0 semitones, 4.0 notes per bar

[notes] 'Contre'  bars=4 grid=8 notes=16
  OK     all 16 notes are in F major
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 4 / leaps 11, up 37 / down 32 semitones, 4.0 notes per bar

[notes] 'Nappe sus'  bars=4 grid=4 notes=4
  OK     all 4 notes are in F major

[drums] 'Beat charley'  bars=1 grid=16 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[drums] 'Beat roulement'  bars=1 grid=16 notes=13

[notes] 'Nappe Q'  bars=4 grid=4 notes=12
  OK     all 12 notes are in F major

[notes] 'Basse Q'  bars=4 grid=8 notes=15
  OK     all 15 notes are in F major
  INFO   contour: range 8 semitones, highest note occurs 1x, steps 1 / leaps 7, up 17 / down 15 semitones, 3.8 notes per bar

[notes] 'Pluck Q'  bars=4 grid=8 notes=27
  OK     all 27 notes are in F major
  INFO   contour: range 20 semitones, highest note occurs 2x, steps 0 / leaps 26, up 106 / down 87 semitones, 6.8 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[drums] 'Beat ouvert'  bars=1 grid=16 notes=14

[notes] 'Nappe Q haussé'  bars=4 grid=4 notes=12
  OK     all 12 notes are in G major

[notes] 'Basse Q haussé'  bars=4 grid=8 notes=15
  OK     all 15 notes are in G major
  INFO   contour: range 8 semitones, highest note occurs 1x, steps 1 / leaps 7, up 17 / down 15 semitones, 3.8 notes per bar

[notes] 'Pluck Q haussé'  bars=4 grid=8 notes=27
  OK     all 27 notes are in G major
  INFO   contour: range 20 semitones, highest note occurs 2x, steps 0 / leaps 26, up 106 / down 87 semitones, 6.8 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Hook haussé'  bars=2 grid=8 notes=7
  OK     all 7 notes are in G major
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 4 / leaps 2, up 7 / down 7 semitones, 3.5 notes per bar

[notes] 'Hook pont'  bars=8 grid=8 notes=26
  INFO   contour: range 9 semitones, highest note occurs 2x, steps 15 / leaps 8, up 30 / down 28 semitones, 3.2 notes per bar
  INFO   contour: the highest note repeats; a memorable line usually has a single peak

[notes] 'Chant'  bars=8 grid=8 notes=27
  OK     all 27 notes are in G major
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 14 / leaps 10, up 30 / down 30 semitones, 3.4 notes per bar

[notes] 'Nappe D'  bars=4 grid=4 notes=8
  OK     all 8 notes are in G major

[notes] 'Basse D'  bars=4 grid=4 notes=2
  OK     all 2 notes are in G major

[arrangement] tempo=108
  Sommet         bars   1-16  (16) 5 parts
  Dépouillement  bars  17-24  ( 8) 2 parts
  Repousse       bars  25-32  ( 8) 3 parts
  Repousse 2     bars  33-40  ( 8) 6 parts
                 edits: Beat [mute=40]; Beat roulement [from=40]; Basse pédale [to=40]; Hook [from=37]
  Sommet II      bars  41-48  ( 8) 5 parts
  Bascule        bars  49-56  ( 8) 8 parts
                 edits: Beat ouvert [mute=52]; Basse Q [to=52]; Basse Q haussé [from=53]; Nappe Q [to=53]; Nappe Q haussé [from=53]; Pluck Q [to=52]; Pluck Q haussé [from=53]
  Sommet haussé  bars  57-64  ( 8) 5 parts
  Dissolution    bars  65-76  (12) 5 parts
                 edits: Beat [to=69]; Beat charley [from=69 to=73]; Basse D [to=73]
  Dernière voix  bars  77-80  ( 4) 2 parts
                 edits: Hook haussé [to=79]
  total 80 bars

[automation] 'Coupure lead'  part='Hook' cc=74 (cutoff) curve=linear points=8

[automation] 'Coupure pluck'  part='Contre' cc=74 (cutoff) curve=linear points=4

[automation] 'Volume nappe'  part='Nappe sus' cc=7 (volume) curve=linear points=4

RESULT ok
```

Rappels gardés, chacun une décision : les arpèges (« Pluck P », « Pluck Q » et sa copie haussée) sont presque tout en sauts et répètent leur note haute (c'est la figure) ; la basse pédale n'a qu'une note (c'est la pédale) ; « Hook pont » porte deux fois son sommet parce qu'il contient deux énoncés du motif.
