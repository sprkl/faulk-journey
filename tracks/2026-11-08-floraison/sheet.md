# Floraison

Instrumental électronique à mi-tempo, 108 bpm, **Mi mineur**, écrit pour mettre à l'épreuve l'effet **Bloom** (chorus, ensemble, vibrato) arrivé la veille, et les parties de la boîte à outils que le passage précédent n'avait pas touchées : **Trim** (longueur des notes au tempo), **Lattice** (notes ramenées dans la gamme), le **suiveur d'enveloppe** et la **saturation** du Filter, l'**anticipation**, le **genou** et le **mélange** du Compressor. Le titre vient de l'idée du morceau : une nappe qui s'épanouit, de sèche et étroite au départ à large et désaccordée (Bloom en Ensemble, mélange automatisé), pendant qu'un lead vibré répond à lui-même une quarte plus haut, ramené dans la gamme par Lattice. Pas de profil de style : le cadre est le mien. 64 mesures (2 min 22), forme en arc : intro, premier palier, break court, sommet à 33–48 (50 à 75 % du morceau), sortie par retrait en seize mesures.

## Brief et contraintes

- **Profil de style** : aucun (choix du passage). Mi-tempo, mineur naturel, du large et du chaud plutôt que du puissant.
- **Tempo** : 108 bpm.
- **Tonalité** : Mi mineur (E F# G A B C D). Cycle de **quatre accords d'une mesure** : **Em – C – G – D** (i – VI – III – VII), tenu d'un bout à l'autre : le morceau ne module pas, c'est le son qui bouge.
- **Palette par rôle** (sept pistes + master) :
  - pulsation : Drums, kick sur 1, le « et » de 2 et le « et » de 3, caisse claire sur 2 et 4, charley fermé en croches à 60 (« Beat A », « Beat lite » sans kick) ;
  - charleys : une seconde piste Drums, doubles-croches de charley fermé à 60 avec un charley ouvert sur le dernier « a » (« Hats B ») ; une mesure de relance en doubles accentuées avec quatre charleys ouverts (« Hats fill »), une fois ;
  - basse : Oscillator en dents de scie, **Trim au tempo 1/8** (les noires écrites deviennent des croches : le pied est court), Filter passe-bas 250 Hz dont la coupure **suit l'enveloppe** du signal (quantité d'enveloppe 2 oct, attaque 5 ms, relâchement 120 ms : chaque note ouvre le filtre et le referme) et dont la **saturation** est automatisée (couloir 2), à −3 dB (« Bass A » en tresillo 3-3-2) ;
  - nappe : Oscillator en dents de scie, attaque 300 ms, release 600 ms, **une note par accord** dans le clip et **Stack « Dans la gamme »** (+2, +4 degrés) qui construit la triade, **Bloom en mode Ensemble** (profondeur 50 %, vitesse libre 0,8 Hz, phase stéréo 90°), mélange de Bloom automatisé de 20 à 100 % (couloir 1), Reverb 35 %, à −10 dB (« Pad A ») ;
  - arpège : Oscillator en carré, release 100 ms, Filter passe-bas 1,5 kHz résonance 25 %, Echo 1/8 à 15 %, à −6 dB (« Arp A », quatre doubles-croches par temps : fondamentale, tierce, quinte, octave) ;
  - lead : Oscillator en triangle, attaque 20 ms, release 400 ms, **Bloom en mode Vibrato** (au tempo 1/8, profondeur 30 %), Echo 1/8 à 20 %, à −6 dB (« Lead A ») ;
  - réponse : une seconde piste lead, même son plus **Lattice** (« Gamme du projet », notes hors gamme « Vers le haut ») : le clip porte **Lead A transposé de cinq demi-tons** (une quarte) au chromatique, et Lattice ramène le Fa qui en sort sur Fa# ; Echo 1/8 dont le mélange est automatisé (couloir 3), à −7 dB (« Lead B » écrit tel que l'oreille doit l'entendre, « Lead tail » une note tenue) ;
  - master : Compressor seuil −16 dB, ratio 3, **genou 6 dB**, **anticipation Oui**, détection RMS, **mélange 70 %** (compression parallèle), compensation +2 dB ; Ceiling à −0,3 dB ; master à −2 dB.
- **Longueur cible** : 64 mesures : Intro 8 / A 16 / Break 8 / Peak 16 / Exit 16.
- **Contraintes arbitraires** (trois, à moi) :
  1. **un seul cycle d'accords** du début à la fin : ce qui change, c'est le son (Bloom, saturation, échos) et la densité ;
  2. **la basse est un tresillo** (3-3-2 en croches) et rien d'autre : fondamentale, fondamentale, quinte ;
  3. **la réponse du lead est une transposition mécanique** (cinq demi-tons) corrigée par Lattice, jamais réécrite à la main : si la machine se trompe, c'est l'effet MIDI qui rattrape.
- **Signature** : la nappe en Ensemble qui s'élargit (couloir 1) jusqu'au sommet, puis se referme ; le lead vibré qui se répond une quarte plus haut.
- **Hypothèses** : pas de voix, pas de sample dans le morceau (une piste audio sera essayée à part, comme fonction, puis retirée) ; tout vient des instruments de Faulk (Oscillator, Drums), de ses effets MIDI (Stack, Trim, Lattice) et audio (Bloom, Filter, Echo, Reverb, Compressor, Ceiling).

## Boucle de départ

La pulsation d'abord, puis la basse (c'est elle qui fait le genre ici), puis la nappe (une note par accord), l'arpège, le lead.

```pattern drums "Beat A" bars=1 grid=16
Kick  |x.....x...x.....|
Snare |....x.......x...|
CHat  |o.o.o.o.o.o.o.o.|
```
Kick sur 1, sur le « et » de 2 et sur le « et » de 3 : une figure qui pousse, et le temps 4 vide. Caisse claire sur 2 et 4, charley fermé en croches à 60.

```pattern drums "Hats B" bars=1 grid=16
CHat |oooooooooooooooo|
OHat |..............x.|
```
Doubles-croches de charley fermé à 60, un charley ouvert sur le dernier « a » : l'élément aigu qui tient du début à la fin.

```pattern notes "Bass A" bars=4 grid=8 octave=1 key="E minor" role=bass
E2 - . E2 - . B1 - | C2 - . C2 - . G1 - | G1 - . G1 - . D2 - | D2 - . D2 - . A1 - |
```
Tresillo : fondamentale sur 1 et sur le « et » de 2, quinte sur le temps 4, en noires que Trim raccourcit en croches (contrainte 2). Fondamentale et quinte de chaque accord : la basse et les accords sont d'accord à chaque changement.

```pattern notes "Pad A" bars=4 grid=4 octave=3 key="E minor" role=pad
E3+G3+B3 - - - | C3+E3+G3 - - - | G3+B3+D4 - - - | D3+F#3+A3 - - - |
```
Em, C, G, D en position fondamentale, une ronde par accord. Dans Faulk, le clip porte une note par accord (E3, C3, G3, D3) et Stack empile +2 et +4 degrés de la gamme : les mêmes triades.

```pattern notes "Arp A" bars=4 grid=16 octave=4 key="E minor" role=arp
E4 G4 B4 E5 E4 G4 B4 E5 E4 G4 B4 E5 E4 G4 B4 E5 | C4 E4 G4 C5 C4 E4 G4 C5 C4 E4 G4 C5 C4 E4 G4 C5 | G4 B4 D5 G5 G4 B4 D5 G5 G4 B4 D5 G5 G4 B4 D5 G5 | D4 F#4 A4 D5 D4 F#4 A4 D5 D4 F#4 A4 D5 D4 F#4 A4 D5 |
```
Quatre doubles-croches par temps (fondamentale, tierce, quinte, octave), la figure repart avec l'accord à chaque mesure : l'arpège le plus droit possible, pour que le mouvement vienne d'ailleurs (Bloom, couloirs). Dans Faulk : la mesure 1 écrite et répétée, puis copiée et transposée (−4, +3, −2) pour les trois autres.

```pattern notes "Lead A" bars=8 grid=16 octave=4 key="E minor" role=lead
B4 - - - G4 - - - A4 - - - B4 - - - | E5 - - - - - - - D5 - - - B4 - - - | C5 - - - B4 - - - A4 - - - G4 - - - | F#4 - - - - - - - - - - - . . . . | B4 - - - G4 - - - A4 - - - B4 - - - | E5 - - - - - - - F#5 - - - G5 - - - | E5 - - - - - - - D5 - - - B4 - - - | E4 - - - - - - - - - - - - - - - |
```
Deux phrases de quatre mesures en noires et blanches : la question monte à Mi5 et retombe sur Fa#4 (une noire pointée puis un silence), la réponse monte jusqu'au **Sol5**, une fois, mesure 6, et se pose sur un Mi4 tenu une mesure. Le Do5 de la mesure 3 est là exprès : c'est lui qui sortira de la gamme une fois transposé (voir Lead B).

## Variations

```pattern drums "Beat lite" bars=1 grid=16
Snare |....x.......x...|
CHat  |o.o.o.o.o.o.o.o.|
```
Génération 1 (rythme) : Beat A sans kick, pour le break et la fin de la sortie.

```pattern drums "Hats fill" bars=1 grid=16
CHat |XxXxXxXxXxXxXxXx|
OHat |....x...x...x.x.|
```
Génération 2 (rythme) : une mesure de relance, doubles accentuées et quatre charleys ouverts qui se resserrent (2, 3, 4, « et » de 4), jouée une seule fois (mesure 8).

```pattern notes "Lead B" bars=8 grid=16 octave=5 key="E minor" role=lead
E5 - - - C5 - - - D5 - - - E5 - - - | A5 - - - - - - - G5 - - - E5 - - - | F#5 - - - E5 - - - D5 - - - C5 - - - | B4 - - - - - - - - - - - . . . . | E5 - - - C5 - - - D5 - - - E5 - - - | A5 - - - - - - - B5 - - - C6 - - - | A5 - - - - - - - G5 - - - E5 - - - | A4 - - - - - - - - - - - - - - - |
```
Génération 3 (mélodie, par la machine) : Lead A transposé de cinq demi-tons (une quarte) ; le Do5 devient un Fa5, hors de Mi mineur, et **Lattice** (« Vers le haut ») le pousse sur **Fa#5** : c'est ce que la fiche écrit, puisque c'est ce que l'oreille entend (contrainte 3). Sommet Do6, une fois, mesure 6.

```pattern notes "Lead tail" bars=1 grid=4 octave=5 key="E minor" role=lead
E5 - - - |
```
Génération 4 (forme) : la dernière note du morceau, un Mi5 tenu une mesure sur la nappe seule, avec le vibrato de Bloom et les échos ouverts.

Génération 5 (son) : la nappe ne change pas de notes de tout le morceau ; c'est le mélange de Bloom (couloir 1) qui l'ouvre : sèche à l'intro, large au sommet, refermée dans la sortie.

Génération 6 (son) : la saturation du Filter de la basse monte sur le palier A et saute au sommet (couloir 2) : la même ligne de basse, de plus en plus mordante.

Génération 7 (forme) : le kick saute le temps 1 du sommet (`Beat A [from=33.2]`) et le temps 1 de la sortie (`Beat A [from=49.2]`) : deux trous de temps 1, après un silence d'un temps à 32.4.

## Arrangement

```arrangement tempo=108
section Intro  1-8   : Pad A, Hats B [from=5 to=8], Hats fill [from=8]
section A      9-24  : Beat A [mute=24.4], Bass A [mute=24.4], Pad A, Arp A [from=17], Hats B
section Break  25-32 : Beat lite, Bass A [to=32.4], Pad A, Arp A [to=32.4], Lead A [to=32.4]
section Peak   33-48 : Beat A [from=33.2], Bass A, Pad A, Arp A, Lead A [to=41], Lead B [from=41], Hats B
section Exit   49-64 : Beat A [from=49.2 to=57], Bass A [to=57], Pad A, Arp A [to=61], Lead B [to=53], Hats B [to=57], Lead tail [from=61 to=62]
```

Coutures et événements uniques :
- **5.1** : les charleys entrent sur la nappe sèche ;
- **8.1** : la relance de charleys (Hats fill), une fois dans le morceau ;
- **9.1** : beat et basse ensemble, sans annonce ;
- **17.1** : l'arpège entre, la nappe commence à s'ouvrir ;
- **24.4** : le beat et la basse se taisent un temps (trou), puis **25.1** le kick disparaît : break sur caisse claire et charleys, le lead entre en entier ;
- **32.4** : tout se tait un temps sauf la nappe et la caisse claire, puis **33.1 sans kick** (`[from=33.2]`) : le trou de temps 1 avant le sommet, la saturation de la basse saute, la nappe est grande ouverte ;
- **41.1** : le lead passe à sa réponse une quarte plus haut (Lead B, Lattice) ;
- **49.1** : le kick saute encore le temps 1 ; la nappe commence à se refermer ;
- **53** : plus de lead ; **57** : plus de kick, plus de basse, plus de charleys ; **61** : plus d'arpège, un Mi5 tenu (Lead tail) ; **62–64** : nappe seule, Bloom revenu à 20 %, fin sur la ronde de Ré à 64.

## Automation

```automation "Nappe floraison" part="Pad A" param=chorus curve=ease-in
1.1 25, 16.4 25, 32.4 90, 33.1 127 step, 48.4 127, 49.1 90 linear, 60.4 25
```
Mélange de Bloom sur la nappe (25 ≈ 20 %, 127 = 100 %) : sèche pendant l'intro et la première moitié de A, ouverture lente puis rapide (ease-in) de 17 à 32, saut au maximum à 33.1, tenue sur tout le sommet, retrait linéaire de 49 à 61.

```automation "Basse mordant" part="Bass A" cc=16 curve=ease-in
9.1 0, 32.4 50, 33.1 90 step, 56.4 90, 57.1 0
```
Saturation du Filter de la basse (cc 16 : la saturation, 0 = propre, 90 ≈ 70 %) : propre à l'entrée, qui monte lentement puis vite jusqu'au break, saut au sommet, tenue, coupée à 57 avec la basse.

```automation "Réponse échos" part="Lead B" param=delay curve=ease-in
41.1 25, 52.4 100, 53.1 100
```
Mélange de l'Echo de la piste de réponse (25 ≈ 20 %, 100 ≈ 80 %) : la réponse se noie dans ses échos jusqu'à sa dernière note, et la traîne continue après 53.

## Notes de finition

- **Sons** : Bass saw, attaque 5 ms, release 150 ms, Trim au tempo 1/8 binaire, Filter passe-bas 250 Hz, résonance 20 %, quantité d'enveloppe 2 oct (attaque 5 ms, relâchement 120 ms), saturation automatisée ; Pad saw, attaque 300 ms, release 600 ms, Stack dans la gamme (+2, +4), Bloom Ensemble (profondeur 50 %, libre 0,8 Hz, phase stéréo 90°, mélange automatisé), Reverb 35 % ; Arp carré, release 100 ms, Filter 1,5 kHz résonance 25 %, Echo 1/8 retour 30 % mélange 15 % ; Lead triangle, attaque 20 ms, release 400 ms, Bloom Vibrato au tempo 1/8 profondeur 30 %, Echo 1/8 20 % ; Lead B même son, Lattice (gamme du projet, vers le haut), Bloom Vibrato, Echo automatisé ; Drums par défaut ; master Compressor −16 dB, 3:1, genou 6 dB, anticipation, RMS, mélange 70 %, compensation +2 dB, Ceiling −0,3 dB.
- **Niveaux** : Drums 0, Hats −8, Bass −3, Pad −10, Arp −6, Lead −6, Lead B −7, master −2 dB.
- **Humaniser** : le désaccord de Bloom et le strum de Stack suffisent ; les machines restent droites.
- **Laissé à l'oreille** : la profondeur de l'Ensemble au sommet (si la nappe tangue trop, 35 %) ; la quantité d'enveloppe de la basse (si elle claque, 1 oct) ; le mélange du Compressor.
- **Version 2** : une section C avec un second cycle (Am – C – Em – D), un contre-chant de l'arpège en triolets, une vraie fin sur un accord de la nappe sans Bloom.

## Vérification

Sortie de `sheet_tool.py check`, copiée telle quelle dans `check.txt` (à côté de cette fiche) ; le rendu MIDI est `floraison.mid`, livré et jamais importé dans Faulk.
