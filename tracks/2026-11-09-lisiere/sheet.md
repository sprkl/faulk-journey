# Lisière

Instrumental électronique nocturne, 116 bpm, **Fa mineur** (maison) avec la couleur dorienne du **IV majeur** dans la première boucle, écrit sur le **profil de style morzak** (`.claude/skills/music-producer/references/styles/morzak.md`). Le titre : la lisière, le bord du bois la nuit, là où la même boucle tourne et où l'on n'entend changer que la lumière. Le morceau est une boucle tenue pendant trente-deux mesures et qui ne change que de timbre, coupée net au milieu d'une mesure, reprise sur un **second cycle** où l'accord de tonique **bascule de majeur à mineur**, puis ouverte pour le dernier sommet sur une **grille plus riche dont la basse descend d'un degré par mesure**. 80 mesures (2 min 46), forme **F6 Boucle à une interruption** mise à l'échelle de 64 à 80 mesures.

## Brief et contraintes

- **Profil de style** : **morzak**. Gardé : tempo de la famille médiane (116 dans 112–123), Fa mineur comme maison, couleur modale (IV dorien, v mineur, ♭VI et ♭VII), cycles de 2 à 4 accords tenus par section, cinq rôles plus un bruit, synthés simples et basse dominante, arpège qui évolue (croches puis doubles : move 6), mélodie qui se développe (énoncée, variée, étendue : move 9), au moins deux couloirs (move 8), la **signature** (un accord qui bascule sa tierce : Fa majeur puis Fa mineur dans le cycle B, et le IV majeur dorien à la place d'un V). Les deux moves pris comme contraintes viennent de « Where the style is going » (voir ci-dessous). Bendu : la bascule de tierce est dans le cycle B à chaque passage, pas un événement unique (move 2 non pris) ; la fin est une coupure, pas une dissolution (move 3 non pris : F6 finit au milieu d'une phrase, et la coupure rime avec la rupture) ; 2 min 46 au lieu des 3½–7 minutes mesurées (budget de construction par l'interface) ; F6 veut une boucle qui ne change que de timbre, et le lead entre tout de même à la mesure 17 (une seule partie ajoutée, nommée ici).
- **Tempo** : 116 bpm.
- **Tonalité** : Fa mineur. Quatre images d'accords, une par section :
  - **cycle A** (Boucle A, 1–32) : **Fm – Fm – B♭ – B♭** (i – IV dorien), une mesure par accord ;
  - **rupture** (33–36) : silence, puis **D♭** (♭VI) tenu trois mesures ;
  - **cycle B** (Boucle B, 37–60) : **F – Fm – D♭ – E♭** (I – i – ♭VI – ♭VII : la tonique bascule sa tierce, la couleur empruntée de « Where the style is going » 1) ;
  - **grille du sommet** (61–80) : **Fm – E♭ – D♭ – Cm** (i – ♭VII – ♭VI – v), la basse descend Fa, Mi♭, Ré♭, Do (« Where the style is going » 2).
- **Palette par rôle** (cinq pistes, une piste audio, master) :
  - pulsation : Drums, kick sur chaque temps, clap sur 2 et 4, charley fermé sur les contretemps à 60, un charley ouvert sur le dernier « a » (« Beat A », le même groove d'un bout à l'autre : les sections viennent de l'harmonie, pas des parties) ;
  - basse : Oscillator en dents de scie, release 120 ms, Filter passe-bas 300 Hz résonance 15 %, à −2 dB (« Bass A / B / C ») ;
  - nappe : Oscillator en dents de scie, attaque 200 ms, release 500 ms, Filter passe-bas 900 Hz, Reverb 30 %, à −12 dB (« Pad A / B / C / D♭ », triades écrites) ;
  - arpège : Oscillator en carré, release 80 ms, **Filter passe-bas automatisé** (couloirs 1–3) résonance 30 %, Echo 1/8 à 20 %, **Hiccup** (mélange automatisé, couloir 4 : à 0 sauf deux temps), à −8 dB (« Arp A » en croches, « Arp B » et « Arp C » en doubles) ;
  - lead : Oscillator en triangle, attaque 10 ms, release 350 ms, Bloom en Vibrato au tempo 1/8 profondeur 25 %, Echo 1/8 dont le mélange est automatisé (couloir 5), à −6 dB (« Lead A », « Lead libre », « Lead B », « Lead C ») ;
  - traîne : une **piste audio** avec un fichier WAV importé (`tail.wav`, deux secondes de bruit sombre qui décroît), posé une fois à 33.1, à −10 dB (« Tail » dans la fiche, lane Noise) ;
  - master : Compressor seuil −14 dB, ratio 3, détection RMS, mélange 80 % ; Ceiling −0,5 dB ; master à −1 dB. Cible de mix du profil : la basse domine, peu de présence.
- **Longueur cible** : 80 mesures : Boucle A 32 / Rupture 4 / Boucle B 24 / Sommet 20.
- **Contraintes** (trois : deux du profil, une à moi) :
  1. **deux cycles qui alternent par section sur un groove constant** (« Where the style is going » 1) : Beat A ne change jamais ; cycle A dans le mode, cycle B avec la tonique qui bascule majeur → mineur ;
  2. **une grille plus riche pour le dernier sommet seulement** (« Where the style is going » 2) : i – ♭VII – ♭VI – v, la basse descend d'un degré par mesure, et c'est ce qui rend le dernier sommet plus grand que la boucle ;
  3. **la basse est une seule figure rythmique** (fondamentale tenue un temps, fondamentale sur le « et » de 2, quinte sur 4) du début à la fin : seules les hauteurs suivent les accords.
- **Hypothèses** : pas de voix ; un seul fichier audio (la traîne), tout le reste vient des instruments et des effets de Faulk.
- **Forme** : `Form: F6 Boucle à une interruption` (les cinq fiches précédentes n'ont pas de ligne Form et comptent F0 ; le profil classe F3, F6 et la forme à deux sommets ; F6 est la plus proche du plateau du style et sa reprise « réharmonisée » est exactement le cycle B).

## Catalogue d'attributs (profil morzak)

- Son : un lead triangle vibré, un arpège carré filtré (le rôle d'arpège à part entière), une basse mono en dents de scie, une boîte à rythmes simple, cinq rôles, peu de réverbération sur le grave.
- Harmonie : Fa mineur, cycles de 2 à 4 accords d'une mesure, IV dorien, ♭VI et ♭VII, v mineur ; la tonique bascule sa tierce (signature).
- Mélodie : arpège en cascade descendante, mélodie qui chante sur le cycle court et se développe (énoncée, variée, étendue).
- Rythme : doubles-croches droites, densité d'attaques modérée (≈ 5 par seconde avec la batterie seule).
- Forme : plateau hypnotique (F6), une seule interruption, le dernier sommet plus riche en harmonie qu'en parties.
- Tempo : 116.
- Mix : basse et sub dominants, présence basse, master dynamique (mélange du Compressor à 80 %, pas de limiteur serré).

## Boucle de départ

La pulsation d'abord, puis la basse (c'est elle qui porte), la nappe, l'arpège ; le lead vient plus tard.

```pattern drums "Beat A" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |..o...o...o...o.|
OHat  |..............o.|
```
Kick sur les quatre temps, clap sur 2 et 4, charley fermé sur les contretemps à 60 (l'élément aigu qui tient tout le morceau), un charley ouvert doux sur le dernier « a ». Onze attaques par mesure : jamais chargé.

```pattern notes "Bass A" bars=4 grid=8 octave=1 key="F dorian" role=bass
F1 - . F1 . . C2 . | F1 - . F1 . . C2 . | Bb1 - . Bb1 . . F2 . | Bb1 - . Bb1 . . F2 . |
```
La figure de la contrainte 3 : fondamentale tenue un temps, fondamentale sur le « et » de 2, quinte sur le temps 4. Fa puis Si♭ : i et IV dorien.

```pattern notes "Pad A" bars=4 grid=4 octave=3 key="F dorian" role=pad
F3+Ab3+C4 - - - | F3+Ab3+C4 - - - | F3+Bb3+D4 - - - | F3+Bb3+D4 - - - |
```
Fm en position fondamentale, B♭ en second renversement : le Fa3 reste en bas, deux voix bougent d'un ton.

```pattern notes "Arp A" bars=4 grid=8 octave=4 key="F dorian" role=arp
C5 Ab4 F4 C4 C5 Ab4 F4 C4 | C5 Ab4 F4 C4 C5 Ab4 F4 C4 | D5 Bb4 F4 D4 D5 Bb4 F4 D4 | D5 Bb4 F4 D4 D5 Bb4 F4 D4 |
```
Cascade descendante en croches, deux fois par mesure, de la quinte à la quinte basse : la note la plus haute revient à chaque cascade, c'est un arpège (le rappel du check est attendu).

```pattern notes "Lead A" bars=8 grid=8 octave=4 key="F dorian" role=lead
C5 - - - Ab4 - Bb4 - | C5 - - - - - . . | D5 - - - F5 - - - | Eb5 - D5 - Bb4 - . . | C5 - - - Ab4 - Bb4 - | C5 - - - Eb5 - F5 - | G5 - - - F5 - D5 - | C5 - - - - - - . |
```
Énoncé (move 9) : deux phrases de quatre mesures. La première tourne autour de Do5 et monte à Fa5 sur le Si♭ ; la seconde reprend le même départ et monte une fois à **Sol5** (mesure 7), puis se pose sur Do5. Dix-neuf notes.

## Variations

```pattern notes "Bass B" bars=4 grid=8 octave=1 role=bass
F1 - . F1 . . C2 . | F1 - . F1 . . C2 . | Db2 - . Db2 . . Ab1 . | Eb2 - . Eb2 . . Bb1 . |
```
Génération 1 (harmonie) : la même figure sur le cycle B : Fa, Fa, Ré♭, Mi♭. Pas de `key=` : le cycle B mélange Fa majeur et Fa mineur exprès.

```pattern notes "Pad B" bars=4 grid=4 octave=3 role=pad
F3+A3+C4 - - - | F3+Ab3+C4 - - - | F3+Ab3+Db4 - - - | G3+Bb3+Eb4 - - - |
```
Génération 2 (harmonie, signature) : **Fa majeur puis Fa mineur** (La3 → La♭3 : la tierce bascule), puis D♭ avec le Fa en bas, puis E♭ en premier renversement. Une voix bouge d'un demi-ton à chaque accord. Pas de `key=` (La♮ et Ré♭ sortent de Fa mineur exprès).

```pattern notes "Arp B" bars=4 grid=16 octave=4 role=arp
F5 C5 A4 F4 F5 C5 A4 F4 F5 C5 A4 F4 F5 C5 A4 F4 | F5 C5 Ab4 F4 F5 C5 Ab4 F4 F5 C5 Ab4 F4 F5 C5 Ab4 F4 | F5 Db5 Ab4 F4 F5 Db5 Ab4 F4 F5 Db5 Ab4 F4 F5 Db5 Ab4 F4 | Eb5 Bb4 G4 Eb4 Eb5 Bb4 G4 Eb4 Eb5 Bb4 G4 Eb4 Eb5 Bb4 G4 Eb4 |
```
Génération 3 (rythme, move 6) : l'arpège passe en doubles-croches, quatre cascades par mesure, de l'octave à la fondamentale ; la tierce bascule avec la nappe (La4 → La♭4). Pas de `key=` (cycle B).

```pattern notes "Lead B" bars=8 grid=8 octave=4 role=lead
C5 - - - A4 - Bb4 - | C5 - - - Ab4 - . . | Db5 - - - F5 - - - | Eb5 - Bb4 - G4 - . . | C5 - - - A4 - Bb4 - | C5 - - - Eb5 - F5 - | Ab5 - - - F5 - Db5 - | Bb4 - - - - - - . |
```
Génération 4 (mélodie, move 9) : Lead A varié sur le cycle B : le même départ, La♮ sur Fa majeur puis La♭ sur Fa mineur (la mélodie dit la bascule), la montée va à **La♭5** (mesure 7), une fois, et la phrase se pose sur Si♭4 (la quinte de E♭). Vingt notes. Pas de `key=` (cycle B).

```pattern notes "Bass C" bars=4 grid=8 octave=1 key="F minor" role=bass
F2 - . F2 . . C2 . | Eb2 - . Eb2 . . Bb1 . | Db2 - . Db2 . . Ab1 . | C2 - . C2 . . G1 . |
```
Génération 5 (harmonie, contrainte 2) : la grille du sommet, la basse descend Fa2, Mi♭2, Ré♭2, Do2, un degré par mesure, toujours la même figure.

```pattern notes "Pad C" bars=4 grid=4 octave=3 key="F minor" role=pad
F3+Ab3+C4 - - - | G3+Bb3+Eb4 - - - | F3+Ab3+Db4 - - - | Eb3+G3+C4 - - - |
```
Génération 6 (harmonie) : Fm, E♭ (premier renversement), D♭ (Fa en bas), Cm (premier renversement) : la nappe reste serrée entre Mi♭3 et Mi♭4 pendant que la basse descend.

```pattern notes "Arp C" bars=4 grid=16 octave=4 key="F minor" role=arp
F5 C5 Ab4 F4 F5 C5 Ab4 F4 F5 C5 Ab4 F4 F5 C5 Ab4 F4 | Eb5 Bb4 G4 Eb4 Eb5 Bb4 G4 Eb4 Eb5 Bb4 G4 Eb4 Eb5 Bb4 G4 Eb4 | Db5 Ab4 F4 Db4 Db5 Ab4 F4 Db4 Db5 Ab4 F4 Db4 Db5 Ab4 F4 Db4 | C5 G4 Eb4 C4 C5 G4 Eb4 C4 C5 G4 Eb4 C4 C5 G4 Eb4 C4 |
```
Génération 7 (harmonie + registre) : les cascades de doubles descendent avec la basse, une par accord, du Fa5 au Do4 : l'arpège lui-même dessine la grille.

```pattern notes "Lead C" bars=8 grid=8 octave=5 key="F minor" role=lead
F5 - Ab5 - C6 - - - | Bb5 - - - G5 - Eb5 - | F5 - - - Ab5 - - - | G5 - Eb5 - C5 - - - | F5 - Ab5 - Bb5 - - - | Bb5 - - - G5 - Eb5 - | Db5 - F5 - Ab5 - - - | G5 - - - - - - - |
```
Génération 8 (mélodie, move 9 : étendue) : au sommet la mélodie monte d'une octave et s'étire : elle atteint **Do6** dès la mesure 1, une seule fois (la seconde phrase s'arrête à Si♭5), et finit sur un Sol5 tenu sur le Cm. Vingt et une notes.

```pattern notes "Pad Db" bars=4 grid=4 octave=3 role=pad
. . . . | F3+Ab3+Db4 - - - | - - - - | - - - - |
```
Génération 9 (forme) : l'accord de la rupture : une mesure de rien, puis D♭ (♭VI) tenu trois mesures, seul avec le lead. Pas de `key=` (Ré♭ hors de Fa dorien).

```pattern notes "Lead libre" bars=4 grid=8 octave=4 role=lead
. . . . . . . . | Ab4 - - - - - - - | F5 - - - - - Eb5 - | Db5 - - - - - - - |
```
Génération 10 (forme) : la phrase libre de la rupture, en notes longues sur le D♭ : La♭4, Fa5 (sommet, une fois), Mi♭5 de passage, Ré♭5. Quatre notes, le vibrato et les échos ouverts. Pas de `key=`.

```pattern drums "Tail" bars=1 grid=16
Noise |x...............|
```
Génération 11 (son) : la traîne de bruit, une fois, à 33.1 : dans Faulk c'est un clip **audio** (`tail.wav` importé sur une piste audio) ; dans le rendu MIDI, une lane Noise.

## Arrangement

Form: F6 Boucle à une interruption

```arrangement tempo=116
section BoucleA   1-32  : Beat A [to=32.3], Bass A [to=32.3], Pad A [to=32.3], Arp A [to=32.3], Lead A [from=17 to=32.3]
section Rupture  33-36  : Tail [to=34], Pad Db, Lead libre
section BoucleB  37-60  : Beat A, Bass B [mute=60.4], Pad B, Arp B, Lead B [to=53]
section Sommet   61-80  : Beat A [to=80.3], Bass C [to=80.3], Pad C [to=80.3], Arp C [to=80.3], Lead C [to=77]
```

Cycles par section : **Boucle A** Fm – Fm – B♭ – B♭ ; **Rupture** D♭ ; **Boucle B** F – Fm – D♭ – E♭ ; **Sommet** Fm – E♭ – D♭ – Cm. Quatre images différentes.

Coutures et événements uniques :
- **1.1** : tout entre d'un coup sauf le lead : beat, basse, nappe, arpège (le plateau du style) ; l'arpège est fermé (couloir 1) ;
- **17.1** : le lead énonce sa mélodie ; rien d'autre ne change (la seule partie ajoutée du morceau) ;
- **32.1–32.3** : **Hiccup** jeté sur l'arpège pendant deux temps (événement unique 1, couloir 4) ;
- **32.3** : **tout est coupé au milieu de la mesure** (événement unique 2, structurel), 33 : rien que la **traîne de bruit** (événement 3, le seul son audio du morceau) ;
- **34–36** : D♭ tenu et la phrase libre du lead, sans batterie : la chose « sans rapport » de F6 (fait partie de l'événement structurel) ;
- **37.1** : la boucle revient sur le cycle B sans annonce, l'arpège en doubles et un peu plus ouvert, le lead varié ;
- **52.3** : les échos du lead sont jetés (couloir 5) sur sa dernière note, puis plus de lead de 53 à 60 : la vallée, où l'arpège finit de s'ouvrir ;
- **60.4** : **la basse se tait un temps** avant la grille (événement unique 4) ;
- **61.1** : la grille riche, la basse descend, le lead une octave plus haut, l'arpège grand ouvert : le vrai sommet ;
- **77** : plus de lead, la grille tourne une dernière fois ;
- **80.3** : **coupure au milieu de la mesure** (événement unique 5, structurel), qui rime avec 32.3 ; la réverbération de la nappe et l'écho de l'arpège font la fin.

Longueurs : 32, 4, 24, 20 : toutes multiples de 4 ; la rupture de 4 mesures est irrégulière par rapport aux sections de 16–40 du style, c'est l'interruption.

## Automation

```automation "Arpège s'ouvre" part="Arp A" param=cutoff curve=ease-in
1.1 20, 32.2 100
```
Coupure du Filter de l'arpège (20 ≈ 400 Hz, 100 ≈ 4 kHz) : fermée au départ, elle s'ouvre lentement puis vite (ease-in) sur toute la boucle A : c'est le seul mouvement de ces trente-deux mesures avec l'entrée du lead.

```automation "Arpège B s'ouvre" part="Arp B" param=cutoff curve=ease-in
37.1 50, 60.3 105
```
La même coupure sur la boucle B, repartie à mi-chemin (50 ≈ 1 kHz) et montée jusqu'à 105 (≈ 5 kHz) au bout de la vallée : le sommet se prépare par le son, pas par des parties.

```automation "Arpège C plein" part="Arp C" param=cutoff curve=linear
61.1 110, 80.2 127
```
Grand ouvert sur la grille, jusqu'au bout.

```automation "Hoquet" part="Arp A" cc=17 curve=step
1.1 0, 32.1 127, 32.3 0
```
Mélange de Hiccup sur l'arpège (cc 17 : 0 = sec, 127 = 100 %), à zéro tout le morceau sauf deux temps avant la coupure : l'arpège bégaie puis tout s'arrête.

```automation "Échos jetés" part="Lead B" param=delay curve=step
37.1 25, 52.3 100, 60.4 25
```
Mélange de l'Echo du lead (25 ≈ 20 %, 100 ≈ 80 %) : jeté sur la dernière note de Lead B, tenu dans la vallée, ramené juste avant la grille. Dans Faulk, un seul couloir sur la piste lead (le même paramètre) porte aussi 17.1 à 25.

## Notes de finition

- **Sons** : Bass saw, release 120 ms, Filter passe-bas 300 Hz résonance 15 % ; Pad saw, attaque 200 ms, release 500 ms, Filter 900 Hz, Reverb 30 % ; Arp carré, release 80 ms, Filter automatisé résonance 30 %, Echo 1/8 retour 30 % mélange 20 %, Hiccup intervalle 1 mesure taille 1/16 mélange automatisé ; Lead triangle, attaque 10 ms, release 350 ms, Bloom Vibrato au tempo 1/8 profondeur 25 %, Echo 1/8 mélange automatisé ; Drums par défaut ; piste audio pour la traîne ; master Compressor −14 dB 3:1 RMS mélange 80 %, Ceiling −0,5 dB.
- **Niveaux** : Drums 0, Bass −2, Pad −12, Arp −8, Lead −6, Tail −10, master −1 dB : la basse devant, comme le profil le mesure.
- **Humaniser** : rien : le style est fait de machines droites ; le vibrato de Bloom et l'ouverture du filtre font le vivant.
- **Laissé à l'oreille** : la résonance de l'arpège au sommet (si elle siffle, 20 %) ; le niveau de la traîne ; la profondeur du vibrato.
- **Version 2** : une dissolution de huit mesures après 80 (move 3 du profil) ; le swing des contretemps du charley seul (move 5) ; un contre-chant qui répond à l'arpège dans ses trous (move 7).

## Vérification

Sortie de `sheet_tool.py check`, copiée telle quelle dans `check.txt` (à côté de cette fiche) ; le rendu MIDI est `lisiere.mid`, livré et jamais importé dans Faulk.
