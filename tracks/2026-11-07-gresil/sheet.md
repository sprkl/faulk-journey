# Grésil

Instrumental électronique à mi-tempo, 100 bpm, **Ré dorien**, écrit pour les nouveaux outils du jour : des accords **empilés par un effet MIDI** à partir d'une seule note, un **hoquet** (bégaiement audio) comme événement unique à chaque couture, un **filtre qui bouge tout seul au tempo** sur l'arpège, et trois couloirs d'automation **tapés au clavier**. Aucun profil de style demandé : le cadre est le mien. Le titre vient de la texture : une pluie de petites notes aiguës et aléatoires (le « grésil ») qui va et vient autour d'un cycle de quatre accords, pendant qu'une basse en noires pointées et un arpège à trois notes (une figure de trois doubles-croches sur une grille de quatre) portent le morceau. 72 mesures (2 min 53), forme en arc : intro, premier palier, montée, sommet à 33–48 (46 à 67 % du morceau), break sur l'harmonie déplacée, sortie par retrait en seize mesures.

## Brief et contraintes

- **Profil de style** : aucun (choix du passage). Mi-tempo, mineur modal, texture plutôt que puissance.
- **Tempo** : 100 bpm.
- **Tonalité** : Ré dorien (D E F G A B C). Cycle de **quatre accords d'une mesure** : **Dm7 – G7 – Dm7 – Am7** (i – IV – i – v, le Si naturel de la quarte majeure dorienne dans G7), tenu 64 mesures sur 72. Break (49–56), la seule excursion : **Fmaj7 – G7 – Fmaj7 – Em7** (III – IV – III – ii), tout en Ré dorien, sans basse ni kick.
- **Palette par rôle** (sept pistes + master) :
  - pulsation : Drums, kick sur 1, le « a » de 2 et le « et » de 3 (une figure cassée, pas quatre à la suite), clap sur 2 et 4, charley fermé en contretemps à 60 (« Beat A », « Beat lite » sans kick) ;
  - charleys : une seconde piste Drums, doubles-croches de charley fermé à 60 avec un charley ouvert sur le dernier « a » (« Hats B ») : l'élément de 3–8 kHz qui dure ;
  - basse : Oscillator en dents de scie, Filter passe-bas 300 Hz, mono (« Bass A » en noires pointées et relance, « Bass B » en croches avec saut d'octave au sommet) ;
  - nappe : Oscillator en triangle, **une note par accord** dans le clip et **Stack en mode gamme** (+2, +4, +6 degrés) qui construit l'accord de septième, strum 40 ms, Reverb 35 %, à −10 dB (« Pad A », « Pad B ») ; la fiche écrit les accords complets (ce que l'oreille doit entendre), Faulk les empile ;
  - arpège : Oscillator en carré, Filter passe-bas dont la coupure est **automatisée** (couloir 1) et dont le **LFO au tempo** (triangle, 1/8, profondeur 1) fait bouger le timbre à l'intérieur de chaque croche, Echo 1/8 à 15 %, à −5 dB (« Arp A », « Arp B ») ;
  - lead : Oscillator en triangle, Echo 1/8 dont le mix est **automatisé** (couloir 2), à −6 dB (« Lead A », « Lead thin ») ;
  - texture : Oscillator en sinus, notes courtes (release 0,15 s), **Scatter** 30 % en mode gamme (choix 3, intervalle 4 degrés, autour) pour que la pluie change à chaque passage, Reverb 50 %, à −12 dB (« Grésil ») ;
  - master : Compressor 2:1 seuil −18 dB, relâchement auto ; **Ceiling** à −0,3 dB ; master à −2 dB.
- **Longueur cible** : 72 mesures : Intro 8 / A 16 / Build 8 / Peak 16 / Break 8 / Exit 16.
- **Contraintes arbitraires** (trois, à moi) :
  1. **l'arpège est une figure de trois notes sur une grille de quatre** (3 doubles-croches, relancée à chaque mesure) : l'accent tourne, l'arpège ne « tombe » sur le temps qu'une fois par mesure ;
  2. **chaque couture est un hoquet** : pas de roulement de caisse claire écrit, la fin de chaque section (24.4, 32.4, 48.3, 64.4) est un bégaiement du beat par l'effet Hiccup, dont le mix est automatisé en paliers (couloir 3) ;
  3. **la nappe ne bouge que par le bas** : l'accord change de basse (D, D, D, C) sous des notes communes, et dans le break c'est la même chose un ton plus haut (C, D, C, B).
- **Signature** : la texture « Grésil » (sinus aigus, aléatoires en gamme) ouvre le morceau avec la nappe, se retire quand l'arpège entre (17), revient au milieu du sommet (41) et reste seule avec la nappe à la fin.
- **Hypothèses** : pas de voix, pas de sample ; tout vient des instruments de Faulk (Oscillator, Drums), de ses effets MIDI (Stack, Scatter) et audio (Filter, Echo, Reverb, Compressor, Ceiling, Hiccup).

## Boucle de départ

La pulsation d'abord, puis la basse, puis la nappe (une note par accord), l'arpège, le lead, la texture.

```pattern drums "Beat A" bars=1 grid=16
Kick |x......x..x.....|
Clap |....x.......x...|
CHat |..o...o...o...o.|
```
Kick sur 1, sur le « a » de 2 et sur le « et » de 3 : une figure cassée qui laisse le temps 4 vide pour la relance de la basse. Clap sur 2 et 4, charley fermé en contretemps à 60.

```pattern drums "Hats B" bars=1 grid=16
CHat |oooooooooooooooo|
OHat |..............x.|
```
Doubles-croches de charley fermé à 60, un charley ouvert sur le dernier « a » de la mesure : l'élément aigu qui tient du début à la fin (3–8 kHz).

```pattern notes "Bass A" bars=4 grid=16 octave=1 key="D dorian" role=bass
D2 - - - - - . . D2 - - . . . A1 - | G1 - - - - - . . G1 - - . . . D2 - | D2 - - - - - . . D2 - - . . . C2 - | A1 - - - - - . . A1 - - . . . C2 - |
```
Fondamentale tenue une noire pointée, relance d'une croche pointée sur le temps 3, puis une croche d'approche sur le « a » de 4 (quinte, puis fondamentale suivante, puis septième). Trois notes par mesure, la basse respire.

```pattern notes "Pad A" bars=4 grid=4 octave=3 key="D dorian" role=pad
D3+F3+A3+C4 - - - | D3+F3+G3+B3 - - - | D3+F3+A3+C4 - - - | C3+E3+G3+A3 - - - |
```
Dm7, G7 (renversé sur Ré : Ré et Fa restent), Dm7, Am7 (renversé sur Do). Les notes communes tiennent, seule la basse de l'accord bouge (contrainte 3). Dans Faulk, le clip porte une note par accord (D3, G3, D3, A3) et Stack empile +2, +4, +6 degrés de la gamme : les mêmes accords en position fondamentale, ce que la fiche accepte.

```pattern notes "Arp A" bars=4 grid=16 octave=4 key="D dorian" role=arp
D4 F4 A4 D4 F4 A4 D4 F4 A4 D4 F4 A4 D4 F4 A4 D4 | G4 B4 D5 G4 B4 D5 G4 B4 D5 G4 B4 D5 G4 B4 D5 G4 | D4 F4 A4 D4 F4 A4 D4 F4 A4 D4 F4 A4 D4 F4 A4 D4 | A4 C5 E5 A4 C5 E5 A4 C5 E5 A4 C5 E5 A4 C5 E5 A4 |
```
Une figure de **trois** doubles-croches (fondamentale, tierce, quinte) sur une grille de seize : l'accent du 1 revient tous les trois pas, cinq fois et un tiers par mesure, et la figure repart avec l'accord à chaque mesure (contrainte 1). Le sommet répété est attendu sur un arpège.

```pattern notes "Lead A" bars=8 grid=16 octave=4 key="D dorian" role=lead
A4 - - - - - - - C5 - - - D5 - - - | E5 - - - - - - - D5 - - - - - - - | C5 - - - - - D5 - - - A4 - - - - - | - - - - - - - - . . . . . . . . | A4 - - - - - - - C5 - - - D5 - - - | G5 - - - - - - - F5 - - - E5 - - - | D5 - - - - - C5 - - - A4 - - - - - | - - - - - - - - . . . . . . . . |
```
Deux phrases de quatre mesures, question (sommet Mi5) et réponse (sommet **Sol5**, une fois, mesure 6, une blanche). Blanches, noires, noires pointées : la mélodie chante au-dessus de l'arpège en doubles, et la quatrième mesure de chaque phrase est une tenue puis un silence, pour laisser l'arpège tourner seul.

```pattern notes "Grésil" bars=2 grid=16 octave=5 vel=60 key="D dorian" role=texture
D5 . A5 . . E5 . . D5 . G5 . . F5 . . | . E5 . . A5 . D6 . . G5 . . E5 . A5 . |
```
Douze petites notes de sinus sur deux mesures, jamais deux sur des pas voisins, dans la gamme : la pluie. Dans Faulk, Scatter à 30 % déplace une note sur trois vers une voisine de la gamme à chaque passage ; la fiche écrit la pluie « moyenne ».

## Variations

```pattern drums "Beat lite" bars=1 grid=16
Clap |....x.......x...|
CHat |..o...o...o...o.|
```
Génération 1 (rythme) : Beat A sans kick, pour la montée et le dernier palier de la sortie.

```pattern notes "Bass B" bars=4 grid=8 octave=1 key="D dorian" role=bass
D2 D2 D3 D2 D2 D2 A2 D2 | G1 G1 G2 G1 G1 G1 D2 G1 | D2 D2 D3 D2 D2 D2 A2 D2 | A1 A1 A2 A1 A1 A1 E2 A1 |
```
Génération 2 (rythme) : la basse passe en croches au sommet, avec un saut d'octave sur le temps 2 et la quinte sur le « et » de 3 : même harmonie, deux fois plus d'énergie.

```pattern notes "Pad B" bars=4 grid=4 octave=3 key="D dorian" role=pad
C3+E3+F3+A3 - - - | D3+F3+G3+B3 - - - | C3+E3+F3+A3 - - - | B2+D3+E3+G3 - - - |
```
Génération 3 (harmonie) : le break monte d'un ton : Fmaj7 – G7 – Fmaj7 – Em7, la basse d'accord fait C, D, C, B (contrainte 3). Dans Faulk : F3, G3, F3, E3 sous Stack.

```pattern notes "Arp B" bars=4 grid=16 octave=4 key="D dorian" role=arp
F4 A4 C5 F4 A4 C5 F4 A4 C5 F4 A4 C5 F4 A4 C5 F4 | G4 B4 D5 G4 B4 D5 G4 B4 D5 G4 B4 D5 G4 B4 D5 G4 | F4 A4 C5 F4 A4 C5 F4 A4 C5 F4 A4 C5 F4 A4 C5 F4 | E4 G4 B4 E4 G4 B4 E4 G4 B4 E4 G4 B4 E4 G4 B4 E4 |
```
Génération 4 (harmonie) : l'arpège suit le break, même figure de trois.

```pattern notes "Lead thin" bars=4 grid=16 octave=4 key="D dorian" role=lead
A4 - - - - - - - . . . . D5 - - - | E5 - - - - - - - - - - - - - - - | - - - - - - - - C5 - - - A4 - - - | - - - - - - - - . . . . . . . . |
```
Génération 5 (mélodie) : la première phrase amincie à cinq notes, pour la montée et la seconde moitié du break : annoncée avant d'être chantée.

Génération 6 (son) : au sommet, l'arpège garde ses notes mais son filtre s'ouvre (couloir 1) et son LFO au tempo rend chaque croche vivante ; la montée vient du son, pas d'une couche de plus.

Génération 7 (forme) : le kick saute le temps 1 du sommet (`Beat A [from=33.2]`) juste après le hoquet de 32.4 : le trou de temps 1.

## Arrangement

```arrangement tempo=100
section Intro   1-8    : Pad A, Hats B [from=5], Grésil [from=5]
section A       9-24   : Beat A, Bass A, Pad A, Arp A [from=17], Grésil [to=17]
section Build   25-32  : Beat lite, Bass A, Pad A, Arp A, Lead thin, Hats B [from=29]
section Peak    33-48  : Beat A [from=33.2], Bass B, Pad A, Arp A, Lead A, Hats B, Grésil [from=41]
section Break   49-56  : Pad B, Arp B, Lead thin [from=53], Grésil
section Exit    57-72  : Beat A [to=65], Beat lite [from=65 to=69], Bass A [to=65], Pad A, Arp A [to=69], Lead A [to=65], Hats B [to=69], Grésil [from=65]
```

Coutures et événements uniques :
- **5.1** : les charleys et la pluie entrent ensemble sur la nappe ;
- **9.1** : beat et basse ensemble, sans annonce (la pluie continue jusqu'à 17) ;
- **17.1** : l'arpège entre et la pluie se tait : un élément pour un autre, pas une couche de plus ;
- **24.4** : hoquet (Hiccup mix 100 % sur un temps), puis **25.1** le kick disparaît (Build) ;
- **32.4** : hoquet, puis **33.1 sans kick** (`[from=33.2]`) : le trou de temps 1 avant Bass B en croches et le lead entier ;
- **41.1** : la pluie revient au milieu du sommet, sur l'arpège ouvert ;
- **48.3** : hoquet d'une demi-mesure, puis le break : plus de basse, plus de batterie, harmonie un ton plus haut ;
- **53.1** : Lead thin au milieu du break (annonce du retour) ;
- **57.1** : tout revient, le filtre de l'arpège rouvert d'un coup ;
- **64.4** : dernier hoquet, puis **65** : plus de kick, plus de basse, plus de lead ; **69** : plus de charleys ni d'arpège ; **69–72** : nappe et pluie seules, le filtre fermé, fin sur la dernière note tenue de la nappe à 72.

## Automation

```automation "Arp ouverture" part="Arp A" param=cutoff curve=ease-in
17.1 30, 32.4 70, 33.1 95 step, 48.4 95, 49.1 40 linear, 56.4 70, 57.1 95 step, 64.4 95, 68.4 20
```
Coupure du Filter de l'arpège (30 ≈ 400 Hz, 95 ≈ 4 kHz, 20 ≈ 250 Hz) : fermé à l'entrée, ouverture lente puis rapide (ease-in) sur les seize mesures jusqu'au sommet, saut à 95 à 33.1, tenue ; retombée à 40 au break puis remontée linéaire ; rouvert d'un coup à 57 ; fermeture finale 64.4 → 68.4 pour la sortie.

```automation "Lead échos" part="Lead A" param=delay curve=linear
25.1 15, 32.4 60 ease-in, 33.1 20 step, 56.4 20, 57.1 30, 64.4 85
```
Mix de l'Echo du lead : sec pendant la montée (15 → 60 : le lead aminci se noie progressivement avant le sommet), net au sommet (20), puis la sortie se dissout dans les échos (30 → 85).

```automation "Hoquet" part="Beat A" cc=12 curve=step
24.4 127, 25.1 0, 32.4 127, 33.1 0, 48.3 127, 49.1 0, 64.4 127, 65.1 0
```
Mix de Hiccup sur la piste Drums (cc 12 = le mix, 127 = 100 %) : quatre paliers d'un temps (une demi-mesure à 48.3), un à chaque couture, en marches (step). Hiccup en mode insert, intervalle 1/4, taille 1/16, gate 60 %, variation « plus court » : le beat bégaie puis la section suivante reprend sur un silence.

```automation "Nappe entrée" part="Pad A" param=volume curve=ease-out
1.1 40, 8.4 100, 48.4 100 step, 49.1 75, 56.4 100
```
Volume de la nappe : fondu d'entrée sur huit mesures (rapide puis lent), retrait de 25 % au break pour laisser la place à Pad B et à la pluie, retour avant 57.

## Notes de finition

- **Sons** : Bass saw, attaque 5 ms, release 0,2 s, Filter 300 Hz résonance 20 % ; Pad triangle, attaque 0,4 s, release 0,8 s, Stack mode gamme (+2 / +4 / +6 degrés, strum 40 ms, direction montante), Reverb 35 % ; Arp carré, release 0,1 s, Filter passe-bas (coupure automatisée, résonance 30 %, LFO triangle synchronisé 1/8 profondeur 1, redémarrage à la note), Echo 1/8 retour 30 % mix 15 % ; Lead triangle, attaque 20 ms, release 0,4 s, Echo 1/8 mix automatisé ; Grésil sinus, attaque 2 ms, decay 0,1 s, sustain 0, Scatter 30 % (choix 3, intervalle 4, autour, gamme), Reverb 50 % ; Drums par défaut, Hiccup sur la piste Drums ; master Compressor 2:1 −18 dB auto, Ceiling −0,3 dB.
- **Niveaux** : Drums 0, Hats −8, Bass −3, Pad −10, Arp −5, Lead −6, Grésil −12, master −2 dB.
- **Humaniser** : Scatter fait déjà bouger la pluie ; le strum de Stack décale les voix de la nappe ; rien d'autre, les machines restent droites.
- **Laissé à l'oreille** : la quantité de hoquet (gate, taille) à 48.3 ; si la pluie masque le lead à 41–48, la baisser à −14 dB ; la résonance du filtre de l'arpège au sommet.
- **Version 2** : un contre-chant répondant à l'arpège dans ses trous (interlock), une sortie plus longue sur la nappe seule, un second cycle d'accords pour une section C.

## Vérification

Sortie de `sheet_tool.py check`, copiée telle quelle dans `check.txt` (à côté de cette fiche) ; le rendu MIDI est `gresil.mid`, livré et jamais importé dans Faulk.
