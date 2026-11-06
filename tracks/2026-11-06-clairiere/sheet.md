# Clairière

Instrumental électronique clair et aéré, 120 bpm, **Do lydien** : après la série sombre et modale mineure des cinq derniers passages, un morceau en majeur augmenté (le Fa♯ lydien), à tempo plein, dont tout le matériau tient sur **deux accords** (I – II : Cmaj7 – D) et une **pulsation euclidienne** qui traverse le morceau. Aucun profil de style demandé : le cadre est le mien. 96 mesures (3 min 12), forme par densité en deux montées : intro, premier palier, drop, une section B de huit mesures sur quatre accords (la seule fois où l'harmonie bouge), break, second drop avec l'arpège en triolets, sortie par retrait. La fiche est écrite pour ce que je veux entendre : des tenues longues (nappe de deux mesures, basse en noires pointées), des triolets dans le lead et dans l'arpège, un motif euclidien E(5,16), et trois couloirs d'automation.

## Brief et contraintes

- **Profil de style** : aucun (choix du passage : le cycle morzak est terminé). Tempo plein, majeur, lumière.
- **Tempo** : 120 bpm.
- **Tonalité** : Do lydien (C D E F♯ G A B). Cycle de **deux accords de deux mesures** : **Cmaj7 – D** (I – II, la quarte augmentée dans l'accord de II), tenu 88 mesures sur 96. Section B (49–56), la seule excursion : **Em7 – D – Em7 – D – Am7 – G – D – D**, tout en Do lydien.
- **Palette par rôle** (cinq pistes + master) :
  - pulsation : Drums, kick sur les quatre temps, clap sur 2 et 4, charley fermé en contretemps à vélocité 60 (« Beat A » et ses variantes), plus une **percussion euclidienne** E(5,16) sur la ligne Snare à vélocité 60 (« Perc E5 »), de la mesure 17 à la 84 ;
  - basse : Oscillator en dents de scie, Filter passe-bas 350 Hz, mono (« Bass A », « Bass B ») : noire pointée tenue, relance, quinte ;
  - nappe : Oscillator en triangle, un accord de quatre sons **tenu deux mesures** (« Pad A », « Pad B »), Reverb 35 %, à −9 dB ;
  - arpège : Oscillator en carré, Filter passe-bas **automatisé** (couloir 1), Echo 1/8 à 20 % (« Arp A » en doubles-croches, « Arp triplets » en triolets de croches), à −4 dB ;
  - lead : Oscillator en triangle, Echo 1/8 dont le mix est **automatisé** (couloir 2), à −6 dB (« Lead A », « Lead thin ») ;
  - master : Compressor 2:1, master à −3 dB.
- **Longueur cible** : 96 mesures : Intro 8 / A 16 / Build 8 / Drop 16 / B 8 / Break 8 / Drop 2 16 / Exit 16.
- **Contraintes arbitraires** (trois, à moi) :
  1. **deux accords** (I – II lydien) portent 88 mesures ; l'harmonie ne bouge que dans la section B, une fois ;
  2. **la pulsation euclidienne E(5,16)** est un élément du morceau du premier palier jusqu'à la sortie : la basse en reprend les accents dans la section B (sa relance tombe sur un coup du motif) ;
  3. **chaque phrase du lead finit par un triolet de croches** : la mélodie en a quatre, un par phrase, et l'arpège prend les triolets au second drop.
- **Signature** : la nappe tient chaque accord deux mesures entières (ronde liée) pendant que l'arpège change de densité dessous : croches de la basse, doubles de l'arpège, triolets du lead ; la lumière vient du Fa♯ de l'accord de II répété toutes les quatre mesures.
- **Hypothèses** : pas de voix, pas de sample ; tout vient des deux instruments de Faulk (Oscillator, Drums) et de ses effets (Filter, Echo, Reverb, Compressor).

## Boucle de départ

La pulsation d'abord, puis la basse, puis la nappe (c'est elle qui fait la couleur ici), l'arpège, le lead.

```pattern drums "Beat A" bars=1 grid=16
Kick |x...x...x...x...|
Clap |....x.......x...|
CHat |..o...o...o...o.|
```
Quatre kicks, clap sur 2 et 4, charley fermé en contretemps de croches à 60. Le socle, pas de fill.

```pattern drums "Perc E5" bars=1 grid=16
Snare |o..o..o..o..o...|
```
E(5,16), rotation 0 : cinq coups répartis sur seize pas (3-3-3-3-4). Ligne Snare à vélocité 60 : une percussion sèche qui tourne autour du kick sans jamais tomber dessus sauf sur le 1.

```pattern notes "Bass A" bars=4 grid=16 octave=1 key="C lydian" role=bass
C2 - - - - - . C2 - - . . C2 - - . | C2 - - - - - . C2 - - . . G1 - - . | D2 - - - - - . D2 - - . . D2 - - . | D2 - - - - - . D2 - - . . A1 - - . |
```
Fondamentale tenue une noire pointée, relance d'une croche pointée sur le « a » de 2, fondamentale ou quinte sur le 4. Les tenues sont écrites exprès : la basse respire, elle n'est pas en doubles-croches staccato.

```pattern notes "Pad A" bars=4 grid=4 octave=3 key="C lydian" role=pad
C3+E3+G3+B3 - - - | - - - - | D3+F#3+A3+C4 - - - | - - - - |
```
Cmaj7 puis D7 (le Do naturel sous le Ré : la septième de II, qui garde le pied en Do), chacun tenu **deux mesures** entières. Voicings serrés entre Do3 et Do4.

```pattern notes "Arp A" bars=4 grid=16 octave=4 key="C lydian" role=arp
E4 G4 B4 D5 E4 G4 B4 D5 E4 G4 B4 D5 E4 G4 B4 D5 | E4 G4 B4 D5 E4 G4 B4 D5 E4 G4 B4 D5 E4 G4 B4 D5 | F#4 A4 C5 D5 F#4 A4 C5 D5 F#4 A4 C5 D5 F#4 A4 C5 D5 | F#4 A4 C5 D5 F#4 A4 C5 D5 F#4 A4 C5 D5 F#4 A4 C5 D5 |
```
Doubles-croches, une figure montante de quatre notes répétée quatre fois par mesure : Em7 sur Cmaj7 (la neuvième Ré5 au sommet), D7 sur D. Le Ré5 au sommet reste le même sur les deux accords : le point fixe.

```pattern notes "Lead A" bars=8 grid=24 octave=4 key="C lydian" role=lead
G4 - - - - - B4 - - D5 - - - - - - - - . . . . . . | . . . E5 - - - - - D5 - - B4 - - - - - - - - . . . | A4 - - - - - B4 - - A4 - - - - - - - - G4 - - - - - | - - - - - - . . . . . . E5 - D5 - B4 - G4 - - - - - | G4 - - - - - B4 - - D5 - - - - - - - - E5 - - - - - | F#5 - - - - - - - - E5 - - D5 - - - - - - - - . . . | B4 - - - - - D5 - - B4 - - - - - - - - A4 - - - - - | - - - - - - . . . . . . D5 - B4 - A4 - G4 - - - - - |
```
Grille 24 par mesure (une croche = 3 pas, un triolet de croche = 2 pas, une noire = 6). Deux phrases de quatre mesures, question et réponse ; chacune se termine par un **triolet de croches** descendant (mesure 4 : Mi5 Ré5 Si4 ; mesure 8 : Ré5 Si4 La4) sur le temps 3, puis une note tenue. Un sommet unique, **Fa♯5** (mesure 6, la quarte lydienne, noire pointée). Les notes longues (noires, noires pointées, blanches) sont écrites comme telles.

## Variations

Une génération, un seul changement.

```pattern drums "Hats" bars=1 grid=16
CHat |..o...o...o...o.|
```
Gén. 1 (forme) : le charley seul, l'intro et le break.

```pattern drums "Beat A open" bars=2 grid=16
Kick |x...x...x...x...|x...x...x...x...|
Clap |....x.......x...|....x.......x...|
CHat |..o...o...o...o.|..o...o...o...o.|
OHat |................|..............x.|
```
Gén. 2 (rythme) : un charley ouvert sur le « a » de 4 toutes les deux mesures : les drops.

```pattern drums "Beat A no kick" bars=1 grid=16
Clap |....x.......x...|
CHat |..o...o...o...o.|
```
Gén. 3 (forme) : sans kick : le build (la tension vient de l'absence) et le début de la sortie.

```pattern notes "Bass B" bars=8 grid=16 octave=1 key="C lydian" role=bass
E2 - - - - - . E2 - - . . E2 - - . | D2 - - - - - . D2 - - . . D2 - - . | E2 - - - - - . E2 - - . . E2 - - . | D2 - - - - - . D2 - - . . A1 - - . | A1 - - - - - . A1 - - . . A1 - - . | G1 - - - - - . G1 - - . . G1 - - . | D2 - - - - - . D2 - - . . D2 - - . | D2 - - - - - . D2 - - . . A1 - - . |
```
Gén. 4 (harmonie) : la figure de Bass A sur les huit accords de la section B. Sa relance tombe sur le « a » de 2 = pas 7 : le troisième coup de E(5,16) (contrainte 2).

```pattern notes "Pad B" bars=8 grid=4 octave=3 key="C lydian" role=pad
E3+G3+B3+D4 - - - | D3+F#3+A3 - - - | E3+G3+B3+D4 - - - | D3+F#3+A3 - - - | A3+C4+E4 - - - | G3+B3+D4 - - - | D3+F#3+A3 - - - | - - - - |
```
Gén. 5 (harmonie) : Em7 – D – Em7 – D – Am7 (sans septième, voicing serré) – G – D tenu deux mesures : la seule excursion harmonique, huit mesures, une fois.

```pattern notes "Arp triplets" bars=4 grid=12 octave=4 key="C lydian" role=arp
E4 G4 B4 E4 G4 B4 D5 B4 G4 D5 B4 G4 | E4 G4 B4 E4 G4 B4 D5 B4 G4 D5 B4 G4 | F#4 A4 C5 F#4 A4 C5 D5 C5 A4 D5 C5 A4 | F#4 A4 C5 F#4 A4 C5 D5 C5 A4 D5 C5 A4 |
```
Gén. 6 (rythme) : triolets de croches (12 pas par mesure), deux figures montantes puis deux descendantes : la vague du second drop.

```pattern notes "Lead thin" bars=4 grid=24 octave=4 key="C lydian" role=lead
G4 - - - - - B4 - - D5 - - - - - - - - . . . . . . | . . . . . . . . . . . . . . . . . . . . . . . . | A4 - - - - - B4 - - A4 - - - - - - - - G4 - - - - - | - - - - - - . . . . . . . . . . . . . . . . . . |
```
Gén. 7 (mélodie, amincie) : les deux appels de Lead A, sans leurs triolets, une mesure sur deux : le build et le break.

## Arrangement

```arrangement tempo=120
section Intro   1-8    : Pad A, Hats, Arp A [from=5]
section A       9-24   : Beat A, Bass A [from=13], Pad A, Arp A, Perc E5 [from=17]
section Build   25-32  : Beat A no kick, Bass A, Pad A, Arp A, Perc E5, Lead thin
section Drop    33-48  : Beat A open, Bass A [from=33.2], Pad A, Arp A, Perc E5, Lead A
section B       49-56  : Beat A, Bass B, Pad B, Perc E5
section Break   57-64  : Hats, Pad A, Lead thin, Arp A [from=61]
section Drop2   65-80  : Beat A open [from=65.2], Bass A, Pad A, Arp triplets, Perc E5, Lead A
section Exit    81-96  : Beat A no kick [to=89], Hats [from=89], Bass A [to=89], Pad A, Arp A [to=93], Perc E5 [to=85]
```

Coutures et événements uniques, par mesure :

- **5** : l'arpège entre sous la nappe, filtre presque fermé (couloir 1) ; **13** : la basse entre quatre mesures après le beat (couture grossière : le beat seul d'abord) ; **17** : **événement 1**, la percussion euclidienne entre et ne partira qu'à la mesure 85.
- **25** : Build : le kick tombe, le lead aminci entre ; rien d'autre ne change.
- **33** : Drop : le kick et le charley ouvert reviennent sur le 1, **la basse sur le temps 2** (`[from=33.2]`, anticipation inversée : un trou dans le grave sur le 1).
- **38.2** : **événement 2** : le Fa♯5 de Lead A, sommet de la mélodie, entendu la première fois (puis à 46.2 et deux fois au second drop).
- **49–56** : **événement 3**, la section B : l'harmonie bouge pour la seule fois, sans arpège ni lead ; la basse reprend les accents euclidiens.
- **57** : Break : tout tombe sauf la nappe et le charley ; le mix de l'Echo du lead monte (couloir 2) ; l'arpège revient à **61** avec son filtre qui remonte.
- **65** : Drop 2 : le beat revient **sur le temps 2** (`[from=65.2]`), la basse et les triolets de l'arpège sur le 1 : la vague.
- **81–96** : Exit, retrait dans l'ordre inverse des arrivées : kick (81), percussion (85), clap et basse (89), arpège (93) ; la nappe et le charley vont au bout.
- **96** : fin sur D tenu (la nappe) : la queue de la Reverb ferme sur la quarte augmentée.

## Automation

```automation "Arp ouverture" part="Arp A" param=cutoff curve=ease-in
5.1 20, 24.4 55, 25.1 45 linear, 32.4 90 step, 33.1 110, 48.4 110 step, 61.1 25, 64.4 80 step, 65.1 115, 80.4 115, 92.4 15
```
Couloir 1, la coupure du Filter de la piste Arp (0 = 200 Hz, 127 = 8 kHz) : fermé à l'entrée (5), s'ouvre lentement puis vite (ease-in) jusqu'au build, saute à ouvert au drop, se referme pour le retour de l'arpège au break (61 → 64, ease-in), s'ouvre à fond sur le second drop, se referme sur toute la sortie (81 → 92, linéaire). La courbe ease-in dans les montées : l'oreille entend l'ouverture surtout dans les dernières mesures, là où la couture arrive.

```automation "Lead échos" part="Lead A" param=delay curve=linear
33.1 25, 56.4 25 step, 57.1 40, 64.4 85, 65.1 25 step, 88.4 25, 95.4 100
```
Couloir 2, le mix de l'Echo de la piste Lead (0 = 0 %, 127 = 100 %) : 20 % pendant les drops, monte de 30 à 65 % sur le break (la mélodie amincie se dissout en échos), retombe au second drop, remonte jusqu'à 80 % sur les huit dernières mesures.

```automation "Nappe entrée" part="Pad A" param=volume curve=ease-out
1.1 50, 8.4 100, 56.4 100 step, 57.1 70, 60.1 100
```
Couloir 3, le volume de la piste Pad : fondu d'entrée sur l'intro (ease-out : vite d'abord, puis se pose), et un creux de trois mesures au début du break, pour que le retour à pleine voix se sente avant l'arpège.

## Notes de finition

- **Sons** : Drums (kick, clap, charley, snare à 60 pour la percussion) ; basse Oscillator **dents de scie**, Filter passe-bas 350 Hz, résonance 0,3, mono ; nappe Oscillator **triangle**, Reverb 35 %, −9 dB ; arpège Oscillator **carré**, Filter passe-bas automatisé, Echo 1/8 à 20 %, −4 dB ; lead Oscillator **triangle**, Echo 1/8 automatisé, −6 dB ; master Compressor 2:1, master −3 dB.
- **Couloir 1 — Arp, Filter, coupure** : 400 Hz à 5 → 1,5 kHz à 24 ; 1,2 kHz à 25 → 3,5 kHz à 32 ; 5 kHz de 33 à 48 ; 500 Hz à 61 → 3 kHz à 64 ; 6 kHz de 65 à 80 ; 6 kHz → 300 Hz de 81 à 92.
- **Couloir 2 — Lead, Echo, mix** : 20 % de 33 à 56 ; 30 → 65 % de 57 à 64 ; 20 % de 65 à 88 ; 20 → 80 % de 89 à 96.
- **Couloir 3 — Pad, volume** : −12 dB à 1 → 0 dB à 8 ; −6 dB à 57 → 0 dB à 60.
- **Humanisation** : charley à 60, percussion euclidienne à 60, clap et kick à 100 ; basse à 100 ; arpège à 90 ; lead à 95 ; nappe à 80. Pas de dérive de temps.
- **Laissé à l'oreille** : la résonance du Filter de l'arpège (0,3 à 0,5) ; le niveau de l'arpège en triolets face au lead ; la durée de la Reverb de la nappe.
- **Version 2** : un contre-chant de la nappe en blanches dans la section B, et un troisième accord (Bm7) pour un pont de quatre mesures avant la sortie.

## Vérification

Sortie de `sheet_tool.py check` : voir `check.txt` à côté de cette fiche.
