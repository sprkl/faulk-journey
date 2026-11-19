# Lame de fond

## Brief et contraintes

Instrumental électronique sombre et chaud, lent, porté par le grave, 84 bpm, **Fa mineur** (éolien, puis dorien), 96 mesures (4 min 34). Le titre : une lame de fond, une vague qui vient de loin et ne retombe pas avant la fin. Une figure d'arpège presque éteinte grossit sans que rien ne s'empile après la mesure 33 : le filtre s'ouvre, la figure se subdivise et monte d'une octave, la basse passe de la pédale à la croche, la nappe gonfle, le chant se développe (énoncé, varié, étendu en triolets) ; au sommet, le dernier accord du cycle bascule sa tierce à chaque tour. Puis un seul accord tenu, sous lequel la basse reprend la figure du début.

Form: F3 Crescendo unique

Profil : morzak

Profil de style : **morzak** (rotation morzak → drifting-cycles → aucun).

- **Tempo** : 84 bpm, 4/4 (famille lente du profil, 70–90 ; lue telle quelle, pas comme la moitié de 168 : la batterie est en demi-temps, clap sur le troisième temps).
- **Tonalité** : Fa mineur, la tonalité de prédilection du profil. La note qui porte le morceau est le sixième degré : **Ré♭** (éolien) dans la graine, **Ré** (dorien, IV majeur) dans la montée, les deux dans le sommet.
- **Palette par rôles** (six pistes, peu de couches) : arpège = carré court filtré, l'ostinato, un rôle à part ; basse = dent de scie mono filtrée, dominante ; nappe = dent de scie lente, sombre, en retrait ; chant = sinus-carré doux avec écho, la ligne qui se développe ; batterie = grosse caisse et clap en demi-temps, droits ; charley = charley fermé seul sur sa piste, **balancé** (le contretemps à 0,6 du temps).
- **Longueur** : 96 mesures.
- **Forme** : F3. Les deux fiches précédentes sont F10 « Manège » et F1 « À rebours » (exclues). Le profil nomme F3 et F6 ; les deux restent permises ; F6 a servi au dernier passage morzak (« Contre-jour », le 16), F3 à celui d'avant (« Braise », le 13) : F3, la plus ancienne des deux. Pour ne pas refaire « Braise » : famille lente au lieu du groove moyen, pas de grille de sommet descendante, la bascule de tierce à chaque tour du sommet et non une seule fois, un charley balancé, un chant en triolets. Écarts assumés à la carte F3 : la graine n'est pas un ostinato seul pendant 32 mesures (charley et basse à 9, nappe et grosse caisse à 17, tous très bas) ; la fin n'est pas une coupure sèche mais un accord tenu de huit mesures.

Trois contraintes, dont deux gestes du profil :

1. *(profil, « Où va le style » 4)* **les sommets viennent du jeu, pas de l'empilement** : de la mesure 33 à la mesure 88 les six mêmes pistes jouent, aucune n'entre ni ne sort (sauf une mesure de souffle à 64) ; tout ce qui grossit est filtre, résonance, registre, subdivision, écho lancé puis repris, niveau de la nappe, et l'accord qui change.
2. *(profil, « Gestes à essayer » 5)* **le contretemps balancé d'une seule partie** : le charley tombe à 0,6 du temps (pas en triolet, 0,667) ; grosse caisse, clap, basse et arpège restent droits.
3. *(la mienne)* **le sixième degré raconte le morceau** : Ré♭ seulement avant 33, Ré seulement de 33 à 64, puis Ré et Ré♭ dans la même mesure à chaque tour du sommet (la signature du profil : Si♭ majeur devient Si♭ mineur).

Ce que je garde du profil : mineur modal, Fa, cycles courts (2 puis 4 accords), IV majeur dorien, basse dominante, peu de couches, un élément discret dans les aigus du début à la fin (le charley, de 9 à 88), un chant qui se développe, des couloirs d'automation. Ce que je plie : la fin (huit mesures au lieu de quelques secondes). Ce que je laisse : la grille de sommet descendante, les deux sommets.

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Filter, Echo, Reverb, Bloom, Compressor, Ceiling).

## Catalogue d'attributs

- **Son** : un arpège carré filtré dont la coupure et la résonance bougent ; une basse dent de scie mono sous 300 Hz ; une nappe sombre ; un chant doux avec écho au tempo ; peu de réverbération dans le grave.
- **Harmonie** : Fa mineur ; graine Fam7 – Ré♭ add9 (deux mesures chacun) ; montée Fam7 – La♭ – Mi♭ – Si♭ (une mesure chacun, IV majeur dorien) ; sommet : le même, Si♭ devenant Si♭ mineur à mi-mesure.
- **Mélodie** : arpèges en cascade ; un chant énoncé, varié, puis étendu en triolets de croches au sommet.
- **Rythme** : droit, sauf le charley balancé à 0,6 ; batterie en demi-temps, jamais chargée.
- **Forme** : un arc sans creux, sommet tardif (68–92 %), fin de huit mesures.
- **Tempo** : 84 bpm.
- **Mix** : grave dominant, peu de présence, facteur de crête de 11 à 16 dB, pas d'écrasement.

## Boucle de départ

L'ostinato, à la noire : Fa mineur deux mesures, Ré♭ deux mesures ; le Mi♭4 de la fin est son seul sommet.

```pattern notes "Arp S" bars=4 grid=4 octave=3 key="F minor" role=arp
F3 C4 Ab3 C4 | F3 C4 G3 C4 | F3 Db4 Ab3 Db4 | F3 C4 Ab3 Eb4 |
```

La basse : une pédale, Fa puis Ré♭, avec une levée.

```pattern notes "Basse S" bars=4 grid=8 octave=1 key="F minor" role=bass
F1 - - - - - - . | F1 - - - - - F1 . | Db1 - - - - - - . | Db1 - - - - - Eb1 . |
```

La nappe : Fam7 puis Ré♭ add9 sur Fa ; une seule voix bouge (Do → Ré♭).

```pattern notes "Nappe S" bars=4 grid=4 octave=3 key="F minor" role=pad
F3+Ab3+C4+Eb4 - - - | - - - - | F3+Ab3+Db4+Eb4 - - - | - - - - |
```

Le charley balancé : cinq pas par temps, le contretemps sur le quatrième (0,6 du temps), tout en notes fantômes.

```pattern drums "Hat" bars=1 grid=20
CHat |o..o. o..o. o..o. o..o.|
```

La grosse caisse de la graine : le premier temps seulement.

```pattern drums "Kick S" bars=1 grid=16
Kick |x... .... .... ....|
```

## Variations

- **Arp S8** (gén. 2, rythme) : la même figure à la croche, avec l'octave du Fa en plus.

```pattern notes "Arp S8" bars=4 grid=8 octave=3 key="F minor" role=arp
F3 C4 Ab3 C4 F4 C4 Ab3 C4 | F3 C4 G3 C4 F4 C4 G3 C4 |
F3 Db4 Ab3 Db4 F4 Db4 Ab3 Db4 | F3 C4 Ab3 C4 F4 C4 Ab3 Eb4 |
```

- **Arp A** (gén. 3, harmonie) : le cycle passe à quatre accords, une mesure chacun ; le Ré naturel arrive à la quatrième mesure.

```pattern notes "Arp A" bars=4 grid=8 octave=3 key="F dorian" role=arp
F3 C4 Ab3 C4 F4 C4 Ab3 C4 | Eb3 C4 Ab3 C4 Eb4 C4 Ab3 C4 |
Eb3 Bb3 G3 Bb3 Eb4 Bb3 G3 Bb3 | D3 Bb3 F3 Bb3 D4 Bb3 F3 Bb3 |
```

- **Arp A16** (gén. 4, rythme) : à la double croche, en cascade sur deux octaves.

```pattern notes "Arp A16" bars=4 grid=16 octave=3 key="F dorian" role=arp
F3 Ab3 C4 F4 Ab4 F4 C4 Ab3 F3 Ab3 C4 F4 C5 F4 C4 Ab3 |
Eb3 Ab3 C4 Eb4 Ab4 Eb4 C4 Ab3 Eb3 Ab3 C4 Eb4 C5 Eb4 C4 Ab3 |
Eb3 G3 Bb3 Eb4 G4 Eb4 Bb3 G3 Eb3 G3 Bb3 Eb4 Bb4 Eb4 Bb3 G3 |
D3 F3 Bb3 D4 F4 D4 Bb3 F3 D3 F3 Bb3 D4 Bb4 D4 Bb3 F3 |
```

- **Arp P** (gén. 5, registre et harmonie) : une octave plus haut ; dans la seconde moitié de la quatrième mesure, les trois Ré deviennent Ré♭ (Si♭ mineur). Pas de `key=` : Ré et Ré♭ y sont tous les deux, c'est voulu.

```pattern notes "Arp P" bars=4 grid=16 octave=4 role=arp
F4 Ab4 C5 F5 Ab5 F5 C5 Ab4 F4 Ab4 C5 F5 C6 F5 C5 Ab4 |
Eb4 Ab4 C5 Eb5 Ab5 Eb5 C5 Ab4 Eb4 Ab4 C5 Eb5 C6 Eb5 C5 Ab4 |
Eb4 G4 Bb4 Eb5 G5 Eb5 Bb4 G4 Eb4 G4 Bb4 Eb5 Bb5 Eb5 Bb4 G4 |
D4 F4 Bb4 D5 F5 D5 Bb4 F4 Db4 F4 Bb4 Db5 Bb5 Db5 Bb4 F4 |
```

- **Basse A** (gén. 6, rythme) : la basse se met à marcher, fondamentales et une levée sur une note de l'accord ; sommet Fa2 une fois.

```pattern notes "Basse A" bars=4 grid=8 octave=1 key="F dorian" role=bass
F1 . F1 . . F1 . C2 | Ab1 . Ab1 . . Ab1 . Eb2 | Eb1 . Eb1 . . Eb1 . Bb1 | Bb1 . Bb1 . . Bb1 D2 F2 |
```

- **Basse A8** (gén. 7, rythme) : à la croche, avec l'octave ; ni Ré ni Ré♭ : elle sert Si♭ majeur comme Si♭ mineur.

```pattern notes "Basse A8" bars=4 grid=8 octave=1 key="F dorian" role=bass
F1 F1 F2 F1 F1 F1 F2 C2 | Ab1 Ab1 Ab2 Ab1 Ab1 Ab1 Ab2 Eb2 | Eb1 Eb1 Eb2 Eb1 Eb1 Eb1 Eb2 Bb1 | Bb1 Bb1 Bb2 Bb1 Bb1 Bb1 Bb2 F2 |
```

- **Nappe A** (gén. 8, harmonie) : Fam7 – La♭ – Mi♭ – Si♭, voix serrées.

```pattern notes "Nappe A" bars=4 grid=4 octave=3 key="F dorian" role=pad
F3+Ab3+C4+Eb4 - - - | Eb3+Ab3+C4+Eb4 - - - | Eb3+G3+Bb3+Eb4 - - - | D3+F3+Bb3+D4 - - - |
```

- **Nappe P** (gén. 9, harmonie) : la quatrième mesure se coupe en deux, Si♭ puis Si♭ mineur (la signature). Pas de `key=`.

```pattern notes "Nappe P" bars=4 grid=4 octave=3 role=pad
F3+Ab3+C4+Eb4 - - - | Eb3+Ab3+C4+Eb4 - - - | Eb3+G3+Bb3+Eb4 - - - | D3+F3+Bb3+D4 - Db3+F3+Bb3+Db4 - |
```

- **Chant A** (gén. 10, mélodie) : l'énoncé, notes longues ; le Ré4 de la quatrième mesure dit le dorien ; sommet Mi♭5 une fois.

```pattern notes "Chant A" bars=8 grid=8 octave=4 key="F dorian" role=melody
C5 - - Ab4 - - F4 - | Eb4 - - - . . Ab4 Bb4 | G4 - - Bb4 - - G4 - | F4 - - - D4 - . . |
C5 - - Ab4 - - F4 - | Eb5 - - - C5 - Ab4 Bb4 | G4 - - Bb4 - - G4 - | F4 - - - - - . . |
```

- **Chant B** (gén. 11, mélodie) : la variation, plus de mouvement, le même contour ; sommet Fa5 une fois.

```pattern notes "Chant B" bars=8 grid=8 octave=4 key="F dorian" role=melody
C5 - Ab4 C5 - Ab4 F4 - | Eb4 - Ab4 - C5 - Ab4 Bb4 | G4 - Bb4 G4 - Bb4 Eb5 - | D5 - - Bb4 F4 - . . |
C5 - Ab4 C5 - Ab4 F4 - | Eb5 - C5 - F5 - Eb5 C5 | Bb4 - G4 Bb4 - G4 Eb4 - | F4 - - - - - . . |
```

- **Chant P** (gén. 12, rythme et registre) : l'extension du sommet, en triolets de croches (douze pas par mesure), une octave plus haut ; il chante la bascule (Ré5 puis Ré♭5) ; sommet Do6 une fois. Pas de `key=`.

```pattern notes "Chant P" bars=8 grid=12 octave=5 role=melody
F5 - - C5 - Ab4 C5 - - F5 - G5 | Ab5 - - - - - Eb5 - C5 Eb5 - - |
G5 - - Eb5 - Bb4 Eb5 - - G5 - Bb5 | F5 - - D5 - - Db5 - - - - . |
F5 - - C5 - Ab4 C5 - - F5 - G5 | Ab5 - - - - - C6 - - Ab5 - - |
Bb5 - - G5 - Eb5 G5 - - Bb5 - G5 | F5 - - D5 - - Db5 - - - - . |
```

- **Beat A** (gén. 13, rythme) : demi-temps, grosse caisse sur 1 et 4, clap sur 3.

```pattern drums "Beat A" bars=1 grid=16
Kick |x... .... .... x...|
Clap |.... .... x... ....|
```

- **Beat P** (gén. 14, rythme) : le même avec une grosse caisse sur le deuxième temps.

```pattern drums "Beat P" bars=1 grid=16
Kick |x... x... .... x...|
Clap |.... .... x... ....|
```

- **Hat P** (gén. 15, son) : le charley balancé, temps accentués, un charley ouvert sur le dernier contretemps.

```pattern drums "Hat P" bars=1 grid=20
CHat |x..o. x..o. x..o. x..o.|
OHat |..... ..... ..... ...x.|
```

- **Nappe fin** (gén. 16, forme) : Fa mineur add9 tenu huit mesures.

```pattern notes "Nappe fin" bars=8 grid=4 octave=3 key="F minor" role=pad
F3+G3+Ab3+C4 - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - |
```

- **Basse fin** (gén. 17, rôle) : la basse reprend les deux premières mesures de l'ostinato, deux octaves plus bas.

```pattern notes "Basse fin" bars=2 grid=4 octave=1 key="F minor" role=bass
F1 C2 Ab1 C2 | F1 C2 G1 C2 |
```

Dispositif structurel : l'échange de rôles de la fin (la basse joue l'ostinato de l'arpège), et le charley à cinq pas par temps contre tout le reste à quatre.

## Arrangement

Form: F3 Crescendo unique

```arrangement tempo=84
section Graine1  1-8   : Arp S
section Graine2  9-16  : Arp S, Basse S, Hat
section Graine3  17-32 : Arp S8, Basse S, Nappe S, Hat [to=32.3], Kick S [to=32.3]
section Montee1  33-48 : Arp A, Basse A, Nappe A, Chant A, Hat, Beat A
section Montee2  49-64 : Arp A16, Basse A8 [mute=64], Nappe A, Chant B, Hat, Beat A [mute=64]
section Sommet   65-88 : Arp P, Basse A8, Nappe P, Chant P, Hat P, Beat P
section Fin      89-96 : Nappe fin, Basse fin [to=95]
```

Cycles d'accords par section :

- Graine (1–32) : Fam7 – Ré♭ add9/Fa, deux mesures par accord (éolien).
- Montée (33–64) : Fam7 – La♭ – Mi♭ – Si♭, une mesure par accord (dorien) : le rythme harmonique double.
- Sommet (65–88) : Fam7 – La♭ – Mi♭ – Si♭ → Si♭m (deux temps chacun dans la quatrième mesure), six tours.
- Fin (89–96) : Fam add9 tenu.

Coutures :

- 8 → 9 : la basse et le charley entrent ensemble, très bas ; rien d'autre ne bouge.
- 16 → 17 : l'arpège passe à la croche, la nappe et la grosse caisse entrent.
- 32 → 33 : le charley et la grosse caisse se taisent deux temps (32.3) ; sur 33.1 le cycle double, le Ré naturel remplace le Ré♭, le chant commence.
- 48 → 49 : l'écho du chant est lancé sur 47–48 puis repris ; l'arpège passe à la double croche, la basse à la croche.
- 63 → 64 → 65 : la mesure 64 est un souffle : ni basse, ni grosse caisse, ni clap ; l'arpège, la nappe, le chant et le charley continuent, la résonance monte ; tout revient sur 65.1 une octave plus haut.
- 88 → 89 : coupe franche sur l'accord tenu ; la basse reprend l'ostinato du début, puis s'arrête à 95.

Événements uniques :

1. 32.3 : le charley et la grosse caisse se taisent deux temps.
2. 33.1 : le Ré naturel (dorien), le rythme harmonique double, le chant entre.
3. 47.1 – 48.4 : l'écho du chant lancé, repris sur 49.1.
4. 64 : une mesure sans grave (structurel).
5. 68.3 : la première bascule Si♭ → Si♭ mineur.
6. 78.3 : le Do6 du chant, la note la plus haute (une fois par passage de huit mesures, donc aussi à 70.3 et 86.3 : la plus haute du morceau, pas unique ; écrit tel quel).
7. 89.1 : la basse prend l'ostinato de l'arpège sous l'accord tenu (échange de rôles, structurel).

## Automation

La coupure du filtre de l'arpège : elle s'ouvre lentement puis vite sur la graine, en ligne droite sur la montée, lentement puis vite vers le souffle de 64, et saute au sommet.

```automation "Coupure arp" part="Arp S" param=cutoff curve=linear
1.1 25 ease-in, 33.1 55 linear, 49.1 70 ease-in, 64.4 105 step, 65.1 115
```

La résonance du même filtre : elle ne bouge qu'à partir de la double croche, monte vers le souffle, retombe en S au sommet, puis repart pour les huit dernières mesures.

```automation "Resonance arp" part="Arp A16" param=resonance curve=linear
49.1 20 linear, 64.4 60 step, 65.1 30 step, 81.1 30 ease-in, 88.4 70
```

La coupure du filtre de la basse : elle suit la vague, puis se referme vite puis lentement sous l'accord tenu.

```automation "Coupure basse" part="Basse S" param=cutoff curve=linear
9.1 30 linear, 33.1 45 ease-in, 65.1 80 step, 89.1 50 ease-out, 96.4 25
```

Le mélange de l'écho du chant : lancé deux fois (47–48, puis 85–88), repris d'un coup.

```automation "Echo chant" part="Chant A" param=delay curve=step
33.1 15 step, 47.1 15 linear, 48.4 60 step, 49.1 15 step, 85.1 15 ease-in, 88.4 70
```

Le volume de la nappe : elle gonfle en S, tient le sommet, et s'éteint vite puis lentement à la fin.

```automation "Volume nappe" part="Nappe S" param=volume curve=linear
17.1 50 smooth, 33.1 80 linear, 65.1 100 step, 89.1 100 ease-out, 96.4 40
```

Dans Faulk : « Coupure arp » et « Resonance arp » = Fréquence de coupure et Résonance du Filter de la piste Arp ; « Coupure basse » = Fréquence de coupure du Filter de la piste Basse ; « Echo chant » = Mélange de l'Echo de la piste Chant ; « Volume nappe » = Volume de la piste Nappe.

## Notes de finition

Sons : Arp = Oscillator carré, déclin 150 ms, maintien 40 %, relâchement 120 ms, Filter passe-bas automatisé (≈ 300 Hz à 5 kHz) et sa résonance, Echo 1/8. mélange 15 %. Basse = dent de scie, relâchement 100 ms, Filter passe-bas automatisé (≈ 150 à 700 Hz), aucun autre effet. Nappe = dent de scie, attaque 500 ms, relâchement 1 s, Filter passe-bas 1,2 kHz, Bloom Ensemble, Reverb taille 70 % mélange 35 %, volume automatisé. Chant = Oscillator sinus (triangle si disponible), attaque 10 ms, relâchement 250 ms, Echo 1/4 au tempo, mélange automatisé (15 % → 55 %), Reverb mélange 20 %. Batterie = le kit de Drums tel quel. Charley = Drums, bas dans le mix. Master = Compressor doux (−12 dB, ratio 2) puis Ceiling −0,3 dB.

Mix: Batterie: C, front (no Reverb), no width, kick 50–100 Hz, clap 1–3 kHz
Mix: Charley: R15, front (no effect), no width, above 5 kHz
Mix: Basse: C, front (no Reverb, Filter lowpass 150–700 Hz automated), no width, 35–210 Hz (Db1–Ab2)
Mix: Arp: L15, middle (Echo eighth_dotted mix 0.15, Filter lowpass 300 Hz–5 kHz automated), no width, 150 Hz–2 kHz (D3–C6)
Mix: Nappe: C, back (Reverb size 0.7 mix 0.35, Filter lowpass 1.2 kHz), Bloom ensemble, 150–600 Hz (D3–Eb4)
Mix: Chant: C, front to middle (Echo quarter mix 0.15–0.55 automated, Reverb mix 0.2), no width, 300 Hz–2 kHz (D4–C6)
Mono check: 1, 3 and 4 by reading (kick, bass and lead at C; Bloom ensemble only on the pad; arp at L15 and hat at R15 are not the same sound mirrored and nothing is hard-panned); 2 does not apply; the rest is left to the ear.

Humanisation : le charley balancé est la seule ; aucune dérive écrite. Laissé à l'oreille : le niveau de la basse contre la grosse caisse, la résonance de l'arpège au souffle (64) et à la fin du sommet, la longueur de l'écho lancé. Une seconde version pourrait essayer : la grille descendante au sommet, la basse balancée avec le charley, le chant en canon avec lui-même deux mesures plus tard.

## Check

```

[notes] 'Arp S'  bars=4 grid=4 notes=16
  OK     all 16 notes are in F minor
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 0 / leaps 15, up 50 / down 40 semitones, 4.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse S'  bars=4 grid=8 notes=6
  OK     all 6 notes are in F minor
  INFO   contour: range 4 semitones, highest note occurs 3x, steps 1 / leaps 1, up 2 / down 4 semitones, 1.5 notes per bar

[notes] 'Nappe S'  bars=4 grid=4 notes=8
  OK     all 8 notes are in F minor

[drums] 'Hat'  bars=1 grid=20 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[drums] 'Kick S'  bars=1 grid=16 notes=1

[notes] 'Arp S8'  bars=4 grid=8 notes=32
  OK     all 32 notes are in F minor
  INFO   contour: range 12 semitones, highest note occurs 4x, steps 0 / leaps 31, up 87 / down 77 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Arp A'  bars=4 grid=8 notes=32
  OK     all 32 notes are in F dorian
  INFO   contour: range 15 semitones, highest note occurs 1x, steps 0 / leaps 31, up 80 / down 75 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Arp A16'  bars=4 grid=16 notes=64
  OK     all 64 notes are in F dorian
  INFO   contour: range 22 semitones, highest note occurs 2x, steps 0 / leaps 63, up 142 / down 142 semitones, 16.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Arp P'  bars=4 grid=16 notes=64
  INFO   contour: range 23 semitones, highest note occurs 2x, steps 0 / leaps 63, up 143 / down 143 semitones, 16.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse A'  bars=4 grid=8 notes=17
  OK     all 17 notes are in F dorian
  INFO   contour: range 14 semitones, highest note occurs 1x, steps 0 / leaps 7, up 28 / down 16 semitones, 4.2 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse A8'  bars=4 grid=8 notes=32
  OK     all 32 notes are in F dorian
  INFO   contour: range 19 semitones, highest note occurs 2x, steps 0 / leaps 18, up 96 / down 84 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Nappe A'  bars=4 grid=4 notes=16
  OK     all 16 notes are in F dorian

[notes] 'Nappe P'  bars=4 grid=4 notes=20

[notes] 'Chant A'  bars=8 grid=8 notes=22
  OK     all 22 notes are in F dorian
  INFO   contour: range 13 semitones, highest note occurs 1x, steps 5 / leaps 16, up 35 / down 42 semitones, 2.8 notes per bar

[notes] 'Chant B'  bars=8 grid=8 notes=34
  OK     all 34 notes are in F dorian
  INFO   contour: range 14 semitones, highest note occurs 1x, steps 6 / leaps 27, up 57 / down 64 semitones, 4.2 notes per bar

[notes] 'Chant P'  bars=8 grid=12 notes=37
  INFO   contour: range 16 semitones, highest note occurs 1x, steps 8 / leaps 28, up 60 / down 64 semitones, 4.6 notes per bar

[drums] 'Beat A'  bars=1 grid=16 notes=3

[drums] 'Beat P'  bars=1 grid=16 notes=4

[drums] 'Hat P'  bars=1 grid=20 notes=9
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Nappe fin'  bars=8 grid=4 notes=4
  OK     all 4 notes are in F minor

[notes] 'Basse fin'  bars=2 grid=4 notes=8
  OK     all 8 notes are in F minor
  INFO   contour: range 7 semitones, highest note occurs 4x, steps 0 / leaps 7, up 23 / down 16 semitones, 4.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[arrangement] tempo=84
  Graine1        bars   1-8   ( 8) 1 parts
  Graine2        bars   9-16  ( 8) 3 parts
  Graine3        bars  17-32  (16) 5 parts
                 edits: Hat [to=32.3]; Kick S [to=32.3]
  Montee1        bars  33-48  (16) 6 parts
  Montee2        bars  49-64  (16) 6 parts
                 edits: Basse A8 [mute=64]; Beat A [mute=64]
  Sommet         bars  65-88  (24) 6 parts
  Fin            bars  89-96  ( 8) 2 parts
                 edits: Basse fin [to=95]
  total 96 bars

[automation] 'Coupure arp'  part='Arp S' cc=74 (cutoff) curve=linear points=5

[automation] 'Resonance arp'  part='Arp A16' cc=71 (resonance) curve=linear points=5

[automation] 'Coupure basse'  part='Basse S' cc=74 (cutoff) curve=linear points=5

[automation] 'Echo chant'  part='Chant A' cc=94 (delay) curve=step points=6

[automation] 'Volume nappe'  part='Nappe S' cc=7 (volume) curve=linear points=5

RESULT ok
```
