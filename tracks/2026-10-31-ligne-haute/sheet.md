# Ligne haute

Instrumental club, 122 bpm, La mineur, 64 mesures (environ 2 min 06), forme par densité, écrit pour être construit dans Faulk avec les devices de `develop` à `8c9191c` : Drums, Oscillator, Echo, Reverb et le nouveau **Filter** (#401). Le morceau est pensé pour que les coutures viennent du **filtre**, pas des cymbales : le passage au break est un balayage passe-haut du **master** (#378), l'ouverture du sommet est un couloir de cutoff sur la basse.

## Brief et contraintes

- **Tempo** : 122 bpm (cœur de la fourchette club ; les stabs en contretemps gardent de l'air).
- **Tonalité** : La mineur (A B C D E F G) ; deux accords seulement, Am7 et Fmaj7 (i7 – VI maj7), deux mesures chacun.
- **Palette par rôle** :
  - pulsation : Drums (kick aux quatre temps, clap sur 2 et 4, charleys en contretemps) ;
  - basse : Oscillator en dents de scie + **Filter passe-bas** (cutoff 450 Hz, résonance 25 %), croches en contretemps (« Bass ») ;
  - harmonie : Oscillator en carré, enveloppe courte, Echo discret, stabs en contretemps (« Stabs ») ;
  - lead : Oscillator en triangle + Echo (« Hook ») ;
  - texture : Oscillator en sinus, quinte tenue, Reverb longue (« Pad »).
  - master : **Filter passe-haut** (cutoff au repos à 20 Hz), piloté par un couloir d'automation du master.
- **Longueur cible** : 64 mesures, forme par densité : Intro 8 / Montée 8 / Groove 16 / Break 8 / Sommet 16 / Sortie 8. Le sommet commence mesure 41 (62 % du morceau) et est la section la plus dense.
- **Contraintes arbitraires** :
  1. deux accords, Am7 et Fmaj7, jamais autre chose ;
  2. le hook n'utilise que quatre hauteurs : A C D E ;
  3. **aucune cymbale de transition** (pas de crash, l'open hat ne marque jamais une couture) : chaque couture est un geste de filtre ou un temps de silence.
- **Hypothèses** : l'édition des couloirs du master dans la timeline n'existe pas encore (#407) : le couloir du master passe par les commandes ; pas de swing (#168).

## Boucle de départ

Pulsation d'abord, puis la basse (c'est elle qui définit le genre ici), puis les stabs, puis le hook.

```pattern drums "Beat A" bars=2 grid=16
Kick |X...x...x...x...|X...x...x...x...|
Clap |....x.......x...|....x.......x...|
CHat |..x...o...X...x.|..o...x...x...X.|
```

Pourquoi : quatre temps au kick, premier temps accentué, clap sur 2 et 4, charleys en contretemps dont la vélocité ne se répète jamais deux fois de suite (fantômes et accents déplacés d'une mesure à l'autre).

```pattern notes "Bass A" bars=4 grid=8 octave=2 key="A minor" role=bass
. A . A . A G A3 | . A . A . A . E | . F . F . F E F3 | . F . F . C . E |
```

Pourquoi : croches en contretemps sous le kick, fondamentale d'abord, l'octave en fin de mesure impaire ; sur Fmaj7, le mi (septième majeure) et le do (quinte) relient les deux accords (contrainte 1).

```pattern notes "Stabs" bars=4 grid=8 octave=3 key="A minor" role=chords
. A+C4+E4+G4 . . . A+C4+E4+G4 . . | . A+C4+E4+G4 . . . . A+C4+E4+G4 . | . A+C4+E4+F4 . . . A+C4+E4+F4 . . | . A+C4+E4+F4 . . . . A+C4+E4+F4 . |
```

Pourquoi : Am7 complet et Fmaj7 sans fondamentale doublée (la basse l'a), conduite de voix minimale : seul sol → fa bouge ; frappes sur les « et », jamais sur le temps (le kick y est déjà).

```pattern notes "Hook A" bars=4 grid=8 octave=4 key="A minor" role=melody
C5 . A . C5 . D5 - | - . A . . . . . | C5 . D5 . E5 - D5 . | C5 - A - . . . . |
```

Pourquoi : quatre hauteurs (contrainte 2), appel d'une mesure, silence, réponse qui monte au sommet E5 une seule fois (mesure 3) et retombe sur la.

```pattern notes "Pad" bars=4 grid=4 octave=3
A+E4 - - - | - - - - | - - - - | - - - - |
```

Pourquoi : fondamentale et quinte sans tierce : la texture ne tranche pas entre Am7 et Fmaj7 (le mi, septième majeure de fa, est la couleur assumée).

## Variations

Une seule chose change par génération, jamais de retour en arrière.

```pattern drums "Hats push" bars=2 grid=16
CHat   |..x...o...X...x.|..o...x...X...x.|
Shaker |x.o.x.o.x.o.x.o.|x.o.x.o.x.o.x.o.|
```

Gen 1 (rythme) : « Beat A » sans kick ni clap, un shaker en doubles alternées fort / fantôme ; pour l'intro.

```pattern drums "Kick hats" bars=2 grid=16
Kick |X...x...x...x...|X...x...x...x...|
CHat |..x...o...X...x.|..o...x...x...X.|
```

Gen 2 (rythme) : « Beat A » sans le clap ; pour la montée (le clap n'arrive qu'avec le groove).

```pattern notes "Bass B" bars=4 grid=8 octave=2 key="A minor" role=bass
. A . A3 . A G A3 | . A . A3 . A . E | . F . F3 . F E F3 | . F . F3 . C E G |
```

Gen 3 (basse) : « Bass A » dont un contretemps sur deux saute à l'octave ; la dernière croche (mi sol) remonte vers la ; pour le sommet.

```pattern notes "Stabs held" bars=4 grid=4 octave=3 key="A minor" role=chords
A+C4+E4+G4 - - - | - - - - | A+C4+E4+F4 - - - | - - - - |
```

Gen 4 (harmonie) : les mêmes voicings tenus deux mesures chacun ; pour le break, où rien ne frappe.

```pattern notes "Hook B" bars=4 grid=8 octave=4 key="A minor" role=melody
. C5 . A . C5 D5 - | - . A - . . . . | . C5 D5 . E5 - . D5 | C5 - A - . . . . |
```

Gen 5 (rythme de la mélodie) : mêmes hauteurs, même sommet unique, toutes les attaques en retard d'une croche : la réponse hésite, l'Echo comble.

```pattern drums "Beat B" bars=2 grid=16
Kick |X...x...x...x...|X...x...x...x..o|
Clap |....x.......x...|....x.......x..o|
CHat |..x...o...X...x.|..o...x...X...xo|
Perc |......x.......x.|......x....x....|
```

Gen 6 (rythme) : « Beat A » avec un fantôme de kick et de clap sur la dernière double, une percussion rare ; pour le sommet.

## Arrangement

```arrangement tempo=122
section Intro   1-8   : Hats push, Pad [from=5]
section Montee  9-16  : Kick hats [mute=16.4], Bass A [from=13], Pad
section Groove  17-32 : Beat A, Bass A [to=31], Stabs, Pad [to=25]
section Break   33-40 : Stabs held, Pad, Hook A [from=35], Bass B [from=40.4]
section Sommet  41-56 : Beat B [mute=56.4], Bass B, Stabs, Hook A [to=49], Hook B [from=49], Pad [from=53]
section Sortie  57-64 : Beat A [to=61], Bass A [to=63], Pad
```

Coutures et événements uniques, par mesure :

- **16.4** : la batterie se tait un temps (`mute=16.4`), le clap arrive avec le groove à 17 : couture par silence (contrainte 3).
- **23.3 → 24.3** : le feedback de l'Echo des Stabs monte à 0,8 pendant deux temps puis retombe (événement unique 1, en marches dans le couloir).
- **31.1 → 33.1** : **balayage passe-haut du master** de 20 Hz à 400 Hz sur deux mesures (la basse est déjà sortie, `to=31`), retour sec à 20 Hz à 33.1 : la couture vers le break est un geste de filtre, pas une cymbale (événement unique 2, couloir du master, #378).
- **39.1 → 41.1** : le mélange de la Reverb du Pad gonfle de 0,35 à 0,9 puis revient (événement unique 3).
- **40.4** : la basse anticipe le sommet d'un temps (`Bass B [from=40.4]`, les croches mi–sol remontent vers la) : couture par harmonie.
- **41.1 → 56.4** : le cutoff du Filter de la basse ouvre lentement de 450 Hz à 1,2 kHz sur tout le sommet (le substitut statique du climax : un seul geste continu).
- **56.4** : un temps de silence de la batterie avant la sortie.
- **64** : fin par coupe : le Pad s'arrête à la barre, la queue de Reverb finit seule.

## Notes de finition

- **Basse** : dents de scie, declin 180 ms, sustain 40 % ; Filter passe-bas 450 Hz, résonance 25 %. Le couloir de cutoff fait le sommet ; ne pas toucher au gain.
- **Stabs** : carré, declin 120 ms, sustain 0 ; Echo mix 0,22, feedback 0,35 (sauf l'événement de 23.3).
- **Hook** : triangle, declin 300 ms ; Echo mix 0,3 : avec « Hook B » décalé d'une croche, l'Echo tisse le hoquet.
- **Pad** : sinus, attaque 800 ms, release 1 500 ms ; Reverb mix 0,35.
- **Master** : Filter passe-haut à 20 Hz au repos (inaudible) ; volume master à régler après un premier export pour garder la crête sous −1 dBFS.
- **Humain** : les vélocités des charleys sont écrites ; le drift en millisecondes n'est pas tenté (pas d'offset fin à la souris).
- **Laissé à l'oreille** : l'équilibre Stabs / Hook au sommet, la longueur de la queue de Reverb finale.
- **Deuxième version** : un vrai break de 16 mesures avec le hook à nu, et le balayage du master qui redescend en rampe sur 4 mesures au lieu du retour sec.

## Check

```
[drums] 'Beat A'  bars=2 grid=16 notes=20

[notes] 'Bass A'  bars=4 grid=8 notes=18
  OK     all 18 notes are in A minor
  INFO   contour: range 21 semitones, highest note occurs 1x, steps 3 / leaps 7, up 32 / down 37 semitones, 4.5 notes per bar

[notes] 'Stabs'  bars=4 grid=8 notes=32
  OK     all 32 notes are in A minor

[notes] 'Hook A'  bars=4 grid=8 notes=11
  OK     all 11 notes are in A minor
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 5 / leaps 5, up 12 / down 15 semitones, 2.8 notes per bar

[notes] 'Pad'  bars=4 grid=4 notes=2

[drums] 'Hats push'  bars=2 grid=16 notes=24
  NOTE   no kick in this pattern: fine if another part carries the pulse

[drums] 'Kick hats'  bars=2 grid=16 notes=16

[notes] 'Bass B'  bars=4 grid=8 notes=19
  OK     all 19 notes are in A minor
  INFO   contour: range 21 semitones, highest note occurs 3x, steps 3 / leaps 15, up 83 / down 85 semitones, 4.8 notes per bar

[notes] 'Stabs held'  bars=4 grid=4 notes=8
  OK     all 8 notes are in A minor

[notes] 'Hook B'  bars=4 grid=8 notes=11
  OK     all 11 notes are in A minor
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 5 / leaps 5, up 12 / down 15 semitones, 2.8 notes per bar

[drums] 'Beat B'  bars=2 grid=16 notes=27

[arrangement] tempo=122
  Intro          bars   1-8   ( 8) 2 parts
                 edits: Pad [from=5]
  Montee         bars   9-16  ( 8) 3 parts
                 edits: Kick hats [mute=16.4]; Bass A [from=13]
  Groove         bars  17-32  (16) 4 parts
                 edits: Bass A [to=31]; Pad [to=25]
  Break          bars  33-40  ( 8) 4 parts
                 edits: Hook A [from=35]; Bass B [from=40.4]
  Sommet         bars  41-56  (16) 6 parts
                 edits: Beat B [mute=56.4]; Hook A [to=49]; Hook B [from=49]; Pad [from=53]
  Sortie         bars  57-64  ( 8) 3 parts
                 edits: Beat A [to=61]; Bass A [to=63]
  total 64 bars

RESULT ok
```
