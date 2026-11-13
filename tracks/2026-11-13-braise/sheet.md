# Braise

Instrumental électronique sombre et chaud, 112 bpm, **La dorien**, 96 mesures (3 min 26). Le titre : une braise sur laquelle on souffle. Une seule figure d'arpège, d'abord à la noire et presque éteinte, que l'on fait grossir sans rien empiler de plus que nécessaire : le filtre s'ouvre, la figure se subdivise (noires, croches, doubles croches), la basse se met à marcher, puis la grille de deux accords s'ouvre en une descente de quatre pour le sommet. Tout à la fin du sommet, l'accord de Ré bascule de majeur à mineur, une seule fois, et il ne reste qu'un accord tenu.

## Brief et contraintes

- **Profil : morzak** (imposé par le brief ; rotation morzak → drifting-cycles → aucun).

Profil : morzak

- **Tempo** : 112 bpm (famille « groove moyen » 112–123 du profil, lecture directe, pas de demi-temps).
- **Tonalité** : La dorien (La Si Do Ré Mi Fa# Sol) : mineur avec le IV majeur. Quatre images d'accords :
  - **cycle A** (1–64) : **Am7 – D** (i – IV dorien), une mesure par accord ;
  - **grille du sommet** (65–84) : **Am7 – G – F – Em** (i – ♭VII – ♭VI – v), une mesure par accord, la basse descend d'un degré par mesure ; le Fa naturel sort du dorien (couleur éolienne, voulue) ;
  - **bascule** (85–88) : **Am7 – G – D – Dm** : le IV dorien revient majeur une mesure, puis sa tierce bascule ;
  - **fin** (89–96) : **Am add9** tenu, puis La et Mi seuls.
- **Palette par rôle** (cinq pistes, master) :
  - arpège (l'ostinato, rôle à part entière) : Oscillator en carré, relâchement court, Filter passe-bas dont la coupure et la résonance sont automatisées, Echo 1/8. léger ;
  - basse : Oscillator en dents de scie, mono, Filter passe-bas 400 Hz, pas de Reverb ; pédale, puis croches, puis la descente ;
  - nappe : Oscillator en dents de scie, attaque lente, Filter passe-bas 2 kHz, Bloom en ensemble, Reverb ; elle gonfle (volume automatisé), elle ne brille pas ;
  - chant : Oscillator en carré adouci (Filter passe-bas 3 kHz), Echo au tempo dont le mélange est lancé une fois ; la ligne qui se développe ;
  - pulsation : Drums ; un charley fermé discret du début à la fin du sommet, un kick qui ne devient régulier qu'au sommet ;
  - master : Compressor léger, Ceiling ; pas d'écrasement.
- **Longueur cible** : 96 mesures.
- **Contraintes** (trois, dont deux gestes du profil) :
  1. *(profil, « Où va le style » 2)* **une grille plus riche et plus rapide pour le sommet seulement** : les deux accords tenus 64 mesures s'ouvrent en i – ♭VII – ♭VI – v, la basse descendant d'un degré par mesure ;
  2. *(profil, « Gestes à essayer » 2)* **la bascule de tierce est un événement unique** : Ré reste majeur tout le morceau et ne devient mineur qu'une fois, à la mesure 88, au moment le plus dense ;
  3. *(la mienne)* **pas de kick sur chaque temps avant la mesure 65** : la pulsation régulière est réservée au sommet.
- **Hypothèses** : pas de voix, aucun fichier audio ; tout vient des instruments et des effets de Faulk.
- **Forme** : `Form: F3 Crescendo unique` (les deux passages précédents sont F2 « Apnée » et F4 « Marée », exclus ; le profil nomme F3 et F6 ; F6 a servi au dernier passage morzak : F3). Écart assumé à la carte F3 : la graine n'est pas un ostinato tout seul pendant 32 mesures (la basse entre à 9, le kick à 17, tous deux très bas), et la fin n'est pas une coupure sèche mais un accord tenu de huit mesures (geste 3 du profil : « une fin qui prend son temps »).

## Catalogue d'attributs

- Tempo : 112 bpm, doubles croches droites, pas de swing.
- Mode et harmonie : mineur modal, cycle de deux accords tenu 64 mesures, IV majeur dorien ; ♭VII et ♭VI de passage au sommet ; la signature (un accord qui change de tierce : D puis Dm) placée une fois, mesures 87–88.
- Son : peu de couches (cinq rôles), sons simples, un arpège comme rôle à part entière, basse mono dominante, très peu de réverbération en bas.
- Rythme : densité modérée, aucun roulement, aucun break de batterie toutes les quatre mesures.
- Mélodie : une ligne qui chante et se développe (énoncée, variée, étendue au sommet, amincie à la sortie) au-dessus d'un arpège en cascade.
- Forme : arc, le moment le plus dense tard (68–92 %), fin de huit mesures.
- Mix : le bas domine ; présence et air discrets mais jamais absents (le charley fermé joue de la mesure 1 à la mesure 88) ; pas de master écrasé.

## Boucle de départ

L'ostinato d'abord (c'est lui la pulsation), puis la basse, puis le reste.

```pattern notes "Arp A" bars=2 grid=4 octave=4 key="A dorian" role=arp
A3 E C E | A3 F# D F# |
```

La figure à la noire : fondamentale, quinte, tierce, quinte. Am puis D : seules deux notes bougent (Mi → Fa#, Do → Ré).

```pattern drums "Beat graine" bars=1 grid=16
CHat  |..o...o...o...o.|
```

Le charley fermé, doux (60), sur les contretemps : l'élément entre 3 et 8 kHz qui ne s'arrête pas avant la fin du sommet.

```pattern notes "Basse pédale" bars=2 grid=4 octave=1 key="A dorian" role=bass
A - - - | D2 - - - |
```

Les deux fondamentales en rondes.

```pattern drums "Beat A" bars=1 grid=16
Kick  |x...............|
CHat  |..o...o...o...o.|
```

Un seul kick par mesure : un battement de cœur, pas encore une pulsation (contrainte 3).

## Variations

```pattern drums "Beat A clap" bars=1 grid=16
Kick  |x...............|
Clap  |..............x.|
CHat  |..o...o...o...o.|
```

Génération 1 (forme) : la même mesure avec un clap seul sur le « et » du temps 4 ; elle ne joue qu'une fois, mesure 32, avant tout motif de clap.

```pattern notes "Arp B" bars=2 grid=8 octave=4 key="A dorian" role=arp
A3 E C E A E C E | A3 F# D F# A F# D F# |
```

Génération 2 (rythme) : la figure à la croche ; sa seconde moitié part de l'octave du haut.

```pattern notes "Basse croches" bars=2 grid=8 octave=1 key="A dorian" role=bass
A . A A . A . A | D2 . D2 D2 . D2 . D2 |
```

Génération 3 (rythme) : la basse se met à marcher, en croches trouées, sur la seule fondamentale.

```pattern drums "Beat B" bars=1 grid=16
Kick  |x.....x...x.....|
Clap  |....x.......x...|
CHat  |o.o.o.o.o.o.o.o.|
```

Génération 4 (rythme) : kick brisé (1, le « et » de 2, le « et » de 3), clap sur 2 et 4, le charley passe à la croche.

```pattern notes "Nappe A" bars=2 grid=4 octave=4 key="A dorian" role=pad
A3+C+E+G - - - | A3+D+F# - - - |
```

Génération 5 (son) : la nappe, Am7 puis D sur La ; la note commune La reste en bas.

```pattern notes "Chant A" bars=4 grid=8 octave=5 key="A dorian" role=melody
E - - D C - A4 - | F#4 - - A4 D - - - | E - - D C - E - | F# - - - . . . . |
```

Génération 6 (mélodie) : le chant énoncé. Deux phrases de deux mesures ; la seconde répond en montant jusqu'au Fa#5, sommet, une fois.

```pattern notes "Arp C" bars=2 grid=16 octave=4 key="A dorian" role=arp
A3 C E A A3 C E A A3 C E A A3 C E A | A3 D F# A A3 D F# A A3 D F# A A3 D F# A |
```

Génération 7 (rythme et contour) : la figure en doubles croches, en cascade montante ; le La4 revient à chaque temps (c'est un arpège : décision).

```pattern notes "Chant B" bars=4 grid=8 octave=5 key="A dorian" role=melody
E - - D C - A4 - | D - - A4 F#4 - - - | E - - D C - E - | G - - F# E - - - |
```

Génération 8 (mélodie) : le chant varié : la réponse de la mesure 2 est renversée (elle descend), et la fin monte jusqu'au Sol5 puis redescend par degrés.

```pattern notes "Arp grille" bars=4 grid=16 octave=4 key="A minor" role=arp
A3 E A E A3 E A E A3 E A E A3 E A E | G3 D G D G3 D G D G3 D G D G3 D G D | F3 C F C F3 C F C F3 C F C F3 C F C | E3 B3 E B3 E3 B3 E B3 E3 B3 E B3 E3 B3 E B3 |
```

Génération 9 (harmonie, contrainte 1) : au sommet l'arpège perd sa tierce (fondamentale, quinte, octave, quinte) et descend d'un degré par mesure : La, Sol, Fa, Mi. Vérifié en La mineur naturel, à cause du Fa.

```pattern notes "Basse grille" bars=4 grid=8 octave=1 key="A minor" role=bass
A . A A . A . A | G . G G . G . G | F . F F . F . F | E . E E . E . E |
```

La basse garde son rythme et descend avec la grille.

```pattern notes "Nappe grille" bars=4 grid=4 octave=4 key="A minor" role=pad
A3+C+E+G - - - | G3+B3+D+G - - - | A3+C+F - - - | G3+B3+E - - - |
```

Am7, G, F sur La, Em sur Sol : les voix bougent peu, le Sol4 du haut tient deux mesures puis descend Fa, Mi.

```pattern notes "Chant grille" bars=4 grid=8 octave=5 key="A minor" role=melody
E - - D C - A4 - | B4 - - D G - - - | A - - G F - C - | B4 - - - E - - - |
```

Génération 10 (mélodie) : le chant étendu : il part comme avant puis monte au La5, sommet du morceau, une fois, sur l'accord de Fa.

```pattern drums "Beat C" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |oooooooooooooooo|
OHat  |..o...o...o...o.|
```

Génération 11 (rythme) : le kick sur chaque temps, enfin (contrainte 3) ; charley fermé en doubles croches douces, charley ouvert doux à contretemps.

```pattern notes "Arp bascule" bars=4 grid=16 octave=4 role=arp
A3 E A E A3 E A E A3 E A E A3 E A E | G3 D G D G3 D G D G3 D G D G3 D G D | D3 A3 D A3 D3 A3 D A3 D3 A3 D A3 D3 A3 D A3 | D3 A3 D A3 D3 A3 D A3 D3 A3 D A3 D3 A3 D A3 |
```

Génération 12 (harmonie, contrainte 2) : les quatre dernières mesures du sommet : La, Sol, puis Ré deux fois. L'arpège n'a pas de tierce : il laisse la nappe et le chant dire la bascule. Sans `key=` (voir « Nappe bascule »).

```pattern notes "Basse bascule" bars=4 grid=8 octave=1 role=bass
A . A A . A . A | G . G G . G . G | D2 . D2 D2 . D2 . D2 | D2 . D2 D2 . D2 . D2 |
```

La basse de la bascule : La, Sol, puis Ré deux fois.

```pattern notes "Nappe bascule" bars=4 grid=4 octave=4 role=pad
A3+C+E+G - - - | G3+B3+D+G - - - | A3+D+F# - - - | A3+D+F - - - |
```

La signature : D sur La (Fa#) puis Dm sur La (Fa naturel). Sans `key=` : le motif contient exprès Fa# et Fa.

```pattern notes "Chant bascule" bars=4 grid=8 octave=5 role=melody
E - - D C - A4 - | B4 - - D G - - - | F# - - - - - - - | F - - - - - - - |
```

Le chant tient la tierce elle-même : Fa#5 une mesure, Fa5 une mesure. Sommet Sol5 une fois.

```pattern notes "Nappe fin" bars=8 grid=4 octave=4 key="A dorian" role=pad
A3+B3+C+E - - - | - - - - | - - - - | - - - - | A3+E - - - | - - - - | - - - - | - - - - |
```

Génération 13 (forme) : Am add9 tenu quatre mesures, puis la quinte à vide quatre mesures : la tierce s'efface, on ne sait plus si c'est majeur ou mineur.

```pattern notes "Basse fin" bars=4 grid=4 octave=1 key="A dorian" role=bass
A - - - | - - - - | - - - - | - - - - |
```

La basse tient La quatre mesures et s'arrête.

```pattern notes "Chant fin" bars=4 grid=4 octave=5 key="A dorian" role=melody
E - - - | - - - - | A4 - - - | - - - - |
```

Génération 14 (mélodie) : le chant aminci : ses deux notes d'appui, Mi puis La, en notes longues.

## Arrangement

Form: F3 Crescendo unique

```arrangement tempo=112
section Graine      1-16  : Arp A, Beat graine, Basse pédale [from=9]
section Graine2    17-32  : Arp A, Beat A [mute=32], Beat A clap [from=32], Basse pédale
section Accretion  33-48  : Arp B, Beat B, Basse croches, Nappe A, Chant A
section Accretion2 49-64  : Arp C, Beat B [mute=64], Basse croches, Nappe A, Chant B
section Plateau    65-84  : Arp grille, Beat C, Basse grille, Nappe grille, Chant grille [mute=73-76]
section Bascule    85-88  : Arp bascule, Beat C [to=88.4], Basse bascule, Nappe bascule, Chant bascule
section Fin        89-96  : Nappe fin, Basse fin [to=93], Chant fin [to=93]
```

Longueurs : 16, 16, 16, 16, 20, 4, 8. Le plateau fait vingt mesures (cinq tours de grille) et la bascule quatre : ensemble les vingt-quatre mesures du sommet de la carte F3.

Cycles par section : Graine, Graine 2, Accrétion, Accrétion 2 : cycle A (Am7 – D) ; Plateau : Am7 – G – F – Em ; Bascule : Am7 – G – D – Dm ; Fin : Am add9, puis La et Mi seuls.

Coutures :
- 16 → 17 : la basse est déjà là depuis 9 (elle passe la ligne), seul le kick entre ;
- 32 → 33 : anticipation : un clap seul sur le « et » du temps 4 de 32, puis tout change ;
- 48 → 49 : le chant et la nappe continuent, seul l'arpège change de vitesse ;
- 64 → 65 : la batterie se tait toute la mesure 64 (`mute=64`), l'arpège en doubles croches tient la pulsation seul, le sommet entre plein ;
- 72 → 77 : le chant se tait un tour (73–76) : l'arpège répond dans son silence ;
- 88 → 89 : le kick manque au temps 4 de 88 (`to=88.4`), la dernière note du chant est jetée dans l'écho, puis tout s'arrête sauf l'accord tenu.

Événements uniques :
1. **mesure 64 : la batterie se tait une mesure, l'arpège tient seul la pulsation** (structurel) ;
2. mesures 87–88 : D puis Dm, la bascule de tierce, une seule fois ;
3. mesure 32, « et » du temps 4 : un clap seul, aucun autre avant la mesure 33 ;
4. mesure 88, temps 4 : le kick manque et le Fa5 du chant part dans l'écho ;
5. **mesure 89 : tout se coupe sur un accord tenu** (structurel : la coupure de la forme F3).

Arc : montée continue de 1 à 64 par le timbre et la subdivision, sommet 65–88 (68 à 92 % du morceau), bascule à 88, huit mesures de braise.

## Automation

```automation "Arp ouverture" part="Arp A" param=cutoff curve=ease-in
1.1 25, 64.4 95, 65.1 115 step, 89.1 60
```

La coupure du Filter de l'arpège : 300 Hz à la mesure 1, environ 4 kHz à la fin de 64 (`ease-in` : lente puis rapide), grande ouverte au sommet, et refermée d'un coup quand tout se coupe (il ne joue plus : c'est sa queue d'écho qui s'assombrit). Le couloir vise « Arp A » dans la notation, mais il court sur la piste de l'arpège entière.

```automation "Arp résonance" part="Arp C" param=resonance curve=linear
49.1 25, 64.4 80, 65.1 30
```

La résonance du même Filter monte pendant les doubles croches (49–64) et retombe au sommet : la tension vient du son, pas d'une couche.

```automation "Nappe gonfle" part="Nappe A" param=volume curve=smooth
33.1 35, 64.4 100
```

Le volume de la nappe : elle entre presque inaudible et gonfle sur 32 mesures.

```automation "Chant écho" part="Chant bascule" cc=94 curve=step
85.1 30, 88.4 115
```

Le mélange de l'Echo du chant saute de 25 % à 90 % au temps 4 de 88 : le Fa5 est jeté dans la fin.

## Notes de finition

- Sons : voir la palette. Arpège : carré, attaque 2 ms, relâchement 120 ms. Basse : dents de scie, relâchement 100 ms. Nappe : dents de scie, attaque 500 ms, relâchement 1,2 s. Chant : carré, attaque 20 ms, relâchement 250 ms.
- Mix: Pulsation : C, devant (ni Reverb ni Echo), sans largeur, kick 50–100 Hz, clap 1–4 kHz, charleys au-dessus de 5 kHz
- Mix: Basse : C, devant (pas de Reverb, Filter passe-bas 400 Hz), sans largeur, 40–250 Hz
- Mix: Arpège : L30, milieu (Echo 1/8. retour 30 % mélange 15 %, Filter passe-bas 300 Hz → 6 kHz automatisé), sans largeur, 200 Hz–4 kHz
- Mix: Nappe : C, fond (Reverb taille 0,7 amortissement 0,7 mélange 40 %, Filter passe-bas 2 kHz), Bloom ensemble phase stéréo 150 mélange 45 % tonalité 300 Hz, 200 Hz–2 kHz
- Mix: Chant : R15, devant puis fond à 88.4 (Echo 1/4 retour 35 % mélange 25 % → 90 %, Filter passe-bas 3 kHz), sans largeur, 400 Hz–3 kHz
- Mono check : 1, 3 et 4 à la lecture (kick et basse à C et sans Bloom ; le chant est à R15, écart voulu à la règle « lead à C » pour répondre à l'arpège à gauche ; Bloom de la nappe à 45 % avec tonalité à 300 Hz ; aucune partie en pan dur) ; 2 sans objet (pas de paire en miroir).
- Humanisation : rien d'écrit ; la vélocité du charley fermé (60) est la seule nuance. À l'oreille : le niveau de la basse contre le kick, la résonance maximale supportable à 64.
- Laissé à l'oreille : le niveau du charley (il doit rester présent sans briller), la taille de la Reverb de la fin.
- Version suivante : swing des contretemps du charley seul (geste 5), un arpège polymétrique de trois pas au plateau (geste 7), une vallée et un second sommet.

Ce qui vient du profil : tempo, mode mineur dorien avec IV majeur, cycle court tenu, cinq rôles, arpège comme rôle, basse dominante, la signature (D → Dm), la grille descendante du dernier sommet, des couloirs de timbre, la fin de huit mesures, le chant qui se développe. Plié : la forme F3 (graine pas seule, fin tenue au lieu d'une coupure). Laissé : le swing, la tonalité de Fa mineur (déjà prise au passage morzak précédent), la forme à deux sommets.

## Check

```
[notes] 'Arp A'  bars=2 grid=4 notes=8
  OK     all 8 notes are in A dorian
  INFO   contour: range 9 semitones, highest note occurs 2x, steps 0 / leaps 7, up 24 / down 15 semitones, 4.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[drums] 'Beat graine'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Basse pédale'  bars=2 grid=4 notes=2
  OK     all 2 notes are in A dorian

[drums] 'Beat A'  bars=1 grid=16 notes=5

[drums] 'Beat A clap'  bars=1 grid=16 notes=6

[notes] 'Arp B'  bars=2 grid=8 notes=16
  OK     all 16 notes are in A dorian
  INFO   contour: range 12 semitones, highest note occurs 2x, steps 0 / leaps 15, up 40 / down 31 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse croches'  bars=2 grid=8 notes=10
  OK     all 10 notes are in A dorian
  INFO   contour: range 5 semitones, highest note occurs 5x, steps 0 / leaps 1, up 5 / down 0 semitones, 5.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[drums] 'Beat B'  bars=1 grid=16 notes=13

[notes] 'Nappe A'  bars=2 grid=4 notes=7
  OK     all 7 notes are in A dorian

[notes] 'Chant A'  bars=4 grid=8 notes=12
  OK     all 12 notes are in A dorian
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 6 / leaps 5, up 16 / down 14 semitones, 3.0 notes per bar

[notes] 'Arp C'  bars=2 grid=16 notes=32
  OK     all 32 notes are in A dorian
  INFO   contour: range 12 semitones, highest note occurs 8x, steps 0 / leaps 31, up 96 / down 84 semitones, 16.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Chant B'  bars=4 grid=8 notes=14
  OK     all 14 notes are in A dorian
  INFO   contour: range 13 semitones, highest note occurs 1x, steps 6 / leaps 7, up 22 / down 22 semitones, 3.5 notes per bar

[notes] 'Arp grille'  bars=4 grid=16 notes=64
  OK     all 64 notes are in A minor
  INFO   contour: range 17 semitones, highest note occurs 4x, steps 0 / leaps 63, up 192 / down 190 semitones, 16.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse grille'  bars=4 grid=8 notes=20
  OK     all 20 notes are in A minor
  INFO   contour: range 5 semitones, highest note occurs 5x, steps 3 / leaps 0, up 0 / down 5 semitones, 5.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Nappe grille'  bars=4 grid=4 notes=14
  OK     all 14 notes are in A minor

[notes] 'Chant grille'  bars=4 grid=8 notes=13
  OK     all 13 notes are in A minor
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 7 / leaps 5, up 17 / down 17 semitones, 3.2 notes per bar

[drums] 'Beat C'  bars=1 grid=16 notes=26

[notes] 'Arp bascule'  bars=4 grid=16 notes=64
  INFO   contour: range 19 semitones, highest note occurs 4x, steps 0 / leaps 63, up 192 / down 192 semitones, 16.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse bascule'  bars=4 grid=8 notes=20
  INFO   contour: range 7 semitones, highest note occurs 10x, steps 1 / leaps 1, up 7 / down 2 semitones, 5.0 notes per bar

[notes] 'Nappe bascule'  bars=4 grid=4 notes=14

[notes] 'Chant bascule'  bars=4 grid=8 notes=9
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 5 / leaps 3, up 10 / down 9 semitones, 2.2 notes per bar

[notes] 'Nappe fin'  bars=8 grid=4 notes=6
  OK     all 6 notes are in A dorian

[notes] 'Basse fin'  bars=4 grid=4 notes=1
  OK     all 1 notes are in A dorian

[notes] 'Chant fin'  bars=4 grid=4 notes=2
  OK     all 2 notes are in A dorian

[arrangement] tempo=112
  Graine         bars   1-16  (16) 3 parts
                 edits: Basse pédale [from=9]
  Graine2        bars  17-32  (16) 4 parts
                 edits: Beat A [mute=32]; Beat A clap [from=32]
  Accretion      bars  33-48  (16) 5 parts
  Accretion2     bars  49-64  (16) 5 parts
                 edits: Beat B [mute=64]
  Plateau        bars  65-84  (20) 5 parts
                 edits: Chant grille [mute=73-76]
  Bascule        bars  85-88  ( 4) 5 parts
                 edits: Beat C [to=88.4]
  Fin            bars  89-96  ( 8) 3 parts
                 edits: Basse fin [to=93]; Chant fin [to=93]
  total 96 bars

[automation] 'Arp ouverture'  part='Arp A' cc=74 (cutoff) curve=ease-in points=4

[automation] 'Arp résonance'  part='Arp C' cc=71 (resonance) curve=linear points=3

[automation] 'Nappe gonfle'  part='Nappe A' cc=7 (volume) curve=smooth points=2

[automation] 'Chant écho'  part='Chant bascule' cc=94 (cc94) curve=step points=2

RESULT ok
```
