# Col

## Brief et contraintes

Instrumental électronique sombre et chaud, porté par le grave, 120 bpm, **Sol mineur** (dorien, puis éolien), 96 mesures (3 min 12). Le titre : un col, le passage bas entre deux sommets. On monte vite au premier, on traverse une longue vallée sans grosse caisse où seule la nappe bat (le LFO de son filtre, calé sur le tempo), puis on atteint le second sommet, plus haut que le premier parce que sa grille est plus riche et plus rapide : la basse descend d'un degré par mesure. Au dernier tour de ce sommet, l'accord de Ré bascule sa tierce, une seule fois. La descente prend son temps.

Form: F12 Deux sommets et une longue vallée

Profil : morzak

Profil de style : **morzak** (demandé par le brief ; rotation morzak → drifting-cycles → aucun).

- **Tempo** : 120 bpm, 4/4, la famille « groove médian » du profil (112–123), lue telle quelle. Les contretemps du charley et de la basse tombent à 0,6 du temps.
- **Tonalité** : Sol mineur. Cycle A dans le mode dorien : Sol m7 – Do (i – IV majeur), deux mesures chacun. Vallée : Sol m add9 – Mi♭ maj7 (i – ♭VI, éolien), quatre mesures chacun. Second sommet : Sol m – Fa – Mi♭ – Ré m (i – ♭VII – ♭VI – v), une mesure chacun ; au dernier tour, Ré majeur.
- **Palette par rôles** (six pistes) : pouls = batterie (grosse caisse, clap) et un charley sur sa propre piste ; basse = dent de scie mono filtrée, dominante ; arpège = carré pincé, un rôle à part, égrené par l'arpégiateur à partir d'accords tenus ; harmonie et texture = nappe en dent de scie lente dont le filtre bat ; chant = carré doux derrière un passe-bas, avec écho.
- **Longueur** : 96 mesures (3 min 12). Le profil va de 3 min 30 à 7 min : un peu court, assumé (la carte tient en 96 mesures et la construction par l'interface reste dans le temps du passage).
- **Forme** : la forme à deux sommets du profil (« Où va le style », 3). Les deux fiches précédentes sont F11 « Mue » et F9 « Rappel » (exclues) ; les cinq dernières : F11, F9, F6, F5, F4. Le profil nomme F3, F6 et la forme à deux sommets : F6 a servi au dernier passage morzak (le 23), F3 aux deux d'avant (le 19 et le 13), la forme à deux sommets jamais. Elle n'a pas de numéro dans `forms.md` : je la note **F12** pour que la rotation la lise (à ajouter à `forms.md`, ou à renuméroter). Carte : montée 1–16, premier sommet 17–28 (18 à 29 % du morceau), vallée 29–56 (28 mesures, 29 % du morceau), second sommet 57–80 (59 à 83 %) sur la grille riche, descente 81–96.

Trois contraintes (deux gestes du profil, une de moi) :

1. *(profil, « Où va le style » 2 et 3)* **Deux sommets, une longue vallée, et la grille riche pour le second seulement** : le cycle de deux accords tient tout le morceau sauf le second sommet, où la basse descend d'un degré par mesure (Sol, Fa, Mi♭, Ré).
2. *(profil, « Gestes à essayer » 6)* **L'arpège évolue section par section sans que ses notes soient réécrites** : les clips de l'arpège ne contiennent que des accords tenus ; la densité (croches, doubles croches, triolets de doubles), le registre (une octave, puis deux) et l'ouverture du filtre changent par les réglages de l'arpégiateur et du filtre.
3. *(la mienne)* **Dans la vallée, le pouls vient d'un filtre, pas de la batterie** : pas de grosse caisse de 29 à 48 ; la nappe bat à la noire par le LFO de son filtre calé sur le tempo, de plus en plus profond.

Signature du profil : la bascule de tierce est un événement unique (geste 2) : Ré mineur pendant cinq tours, **Ré majeur** au sixième et dernier (mesure 80), le Fa♯ dit par le chant, la nappe, l'arpège et la basse.

Ce que je garde du profil : mineur modal, IV majeur dorien, cycles courts, basse dominante, six rôles, charley discret du début à la fin (mesure 9 à 92), balancement sur le charley et la basse ensemble (« Où va le style » 5), chant qui se développe (énoncé, aminci, étendu, aminci), couloirs d'automation, fin qui prend seize mesures. Ce que je plie : la longueur (3 min 12). Ce que je laisse : les deux cycles qui alternent par section (ici trois images d'accords se suivent sans alterner).

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Cascade, Swing, Filter, Echo, Reverb, Bloom, Compressor, Ceiling).

## Catalogue d'attributs (profil morzak, adapté)

- **Son** : six rôles, sons simples ; un arpège pincé qui est un rôle à lui seul ; une basse mono qui domine ; peu de réverbération dans le grave.
- **Harmonie** : Sol mineur ; dorien (Do majeur) aux sommets d'entrée et de sortie, éolien (Mi♭) dans la vallée et au second sommet ; une bascule de tierce (Ré m → Ré) entendue une fois.
- **Mélodie** : un chant qui se développe sur le cycle court ; un seul sommet par phrase.
- **Rythme** : doubles croches droites à l'arpège ; contretemps balancés à 0,6 du temps sur le charley et la basse ; batterie peu chargée, deux relances seulement (28 et 80).
- **Forme** : deux sommets, le second plus haut et plus tardif, une vallée d'un tiers du morceau, une descente lente.
- **Tempo** : 120 bpm.

## Boucle de départ

Le porteur du pouls d'abord : quatre temps au sol, clap sur deux et quatre, charley en contretemps (fantôme sur le temps).

```pattern drums "Beat A" bars=1 grid=16
Kick |x...x...x...x...|
Clap |....x.......x...|
```

```pattern drums "Hat A" bars=1 grid=16
CHat |o.x.o.x.o.x.o.x.|
```

Puis ce qui définit le morceau : la basse, sur Sol m7 – Do, deux mesures par accord. Fondamentale, octave, et une levée qui ramène à l'accord suivant. Ses croches de contretemps sont balancées par le device Swing (les notes restent droites dans le clip).

```pattern notes "Basse A" bars=4 grid=8 octave=2 key="G dorian" role=bass
G . G G3 . G . Bb | G . G G3 . G D F |
C . C C3 . C . E | C . C C3 . C G Bb |
```

L'arpège : deux accords tenus ; l'arpégiateur les égrène en montant (Sol Si♭ Ré Fa, puis Sol Do Mi Sol).

```pattern notes "Arp A" bars=4 grid=4 octave=3 key="G dorian" role=chords
G3+Bb3+D4+F4 - - - | - - - - | G3+C4+E4+G4 - - - | - - - - |
```

## Variations

Génération 2 (harmonie) : la basse en pédale, pour la montée et pour la fin.

```pattern notes "Basse P" bars=4 grid=4 octave=1 key="G minor" role=bass
G - - - | - - - - | - - - - | - - - - |
```

Génération 3 (mélodie) : le chant, énoncé au premier sommet. Deux phrases de quatre mesures ; un seul sommet, Sol5 à la mesure 7 ; il finit sur Do, loin de la tonique : la question reste ouverte avant la vallée.

```pattern notes "Chant A" bars=8 grid=8 octave=4 key="G dorian" role=melody
D5 - - - Bb - C5 - | D5 - - - - - . . | E5 - - - C5 - D5 - | E5 - - - - - G - |
D5 - - - Bb - C5 - | D5 - - F5 - - D5 - | G5 - - - E5 - D5 - | C5 - - - - - . . |
```

Génération 4 (rythme) : la relance, deux fois seulement dans le morceau (28 et 80) : la grosse caisse lâche le quatrième temps, le clap le remplit.

```pattern drums "Beat F" bars=1 grid=16
Kick |x...x...x.......|
Clap |....x.......x.x.|
```

Génération 5 (harmonie, la vallée) : le Mi naturel devient Mi♭. Sol m add9 – Mi♭ maj7, quatre mesures chacun ; deux voix sur quatre ne bougent pas.

```pattern notes "Arp V" bars=8 grid=4 octave=3 key="G minor" role=chords
G3+A3+Bb3+D4 - - - | - - - - | - - - - | - - - - |
G3+Bb3+D4+Eb4 - - - | - - - - | - - - - | - - - - |
```

```pattern notes "Nappe V" bars=8 grid=4 octave=3 key="G minor" role=pad
G3+D4+A4+Bb4 - - - | - - - - | - - - - | - - - - |
G3+D4+Eb4+Bb4 - - - | - - - - | - - - - | - - - - |
```

```pattern drums "Hat V" bars=1 grid=16
CHat |..o...o...o...o.|
```

Le chant aminci : de longues notes, de l'espace ; un seul sommet, Mi♭5 (la note de la vallée).

```pattern notes "Chant B" bars=8 grid=8 octave=4 key="G minor" role=melody
D5 - - - - - - - | . . . . Bb - A - | Bb - - - - - - - | . . . . . . . . |
D5 - - - - - - - | . . . . Eb5 - D5 - | Bb - - - - - - - | - - - - . . . . |
```

La basse revient en pédale sous la vallée, et une grosse caisse seule, sur le premier temps, annonce le retour.

```pattern notes "Basse V" bars=8 grid=4 octave=1 key="G minor" role=bass
G1 - - - | - - - - | - - - - | - - - - | Eb2 - - - | - - - - | - - - - | - - - - |
```

```pattern drums "Beat V" bars=1 grid=16
Kick |x...............|
```

Génération 6 (harmonie, la grille riche) : un accord par mesure, la basse descend d'un degré par mesure.

```pattern notes "Arp P" bars=4 grid=4 octave=3 key="G minor" role=chords
G3+Bb3+D4+G4 - - - | F3+A3+C4+F4 - - - | Eb3+G3+Bb3+Eb4 - - - | D3+F3+A3+D4 - - - |
```

```pattern notes "Nappe P" bars=4 grid=4 octave=3 key="G minor" role=pad
G3+D4+Bb4 - - - | F3+C4+A4 - - - | Eb3+Bb3+G4 - - - | D3+A3+F4 - - - |
```

```pattern notes "Basse D" bars=4 grid=8 octave=2 key="G minor" role=bass
G . G G3 . G . G3 | F . F F3 . F . F3 | Eb . Eb Eb3 . Eb . Eb3 | D . D D3 . D F A |
```

Génération 7 (mélodie) : le chant étendu, seize mesures sur quatre tours de la grille. Chaque mesure pose une note de l'accord sur son premier temps ; un seul sommet, Si♭5 à la mesure 13.

```pattern notes "Chant C" bars=16 grid=8 octave=4 key="G minor" role=melody
D5 - - - Bb - C5 - | C5 - - - A - . . | Bb - - - G - Bb - | A - - - - - F - |
D5 - - - Bb - C5 - | C5 - - F5 - - C5 - | Eb5 - - - D5 - Bb - | D5 - - - - - . . |
G5 - - - D5 - F5 - | F5 - - - C5 - A - | G5 - - Eb5 - - G5 - | A5 - - - F5 - D5 - |
Bb5 - - - G5 - D5 - | A5 - - F5 - - C5 - | G5 - - Eb5 - - Bb - | D5 - - - - - - - |
```

Génération 8 (harmonie, la bascule) : le dernier tour. Ré mineur devient Ré majeur ; le Fa♯ est hors de la gamme, c'est l'idée (pas de `key=`). Le chant redescend et dit lui-même le Fa♯.

```pattern notes "Arp P bascule" bars=4 grid=4 octave=3 role=chords
G3+Bb3+D4+G4 - - - | F3+A3+C4+F4 - - - | Eb3+G3+Bb3+Eb4 - - - | D3+F#3+A3+D4 - - - |
```

```pattern notes "Nappe P bascule" bars=4 grid=4 octave=3 role=pad
G3+D4+Bb4 - - - | F3+C4+A4 - - - | Eb3+Bb3+G4 - - - | D3+A3+F#4 - - - |
```

```pattern notes "Basse D bascule" bars=4 grid=8 octave=2 role=bass
G . G G3 . G . G3 | F . F F3 . F . F3 | Eb . Eb Eb3 . Eb . Eb3 | D . D D3 . D F# A |
```

```pattern notes "Chant D" bars=4 grid=8 octave=4 role=melody
G5 - - - D5 - Bb - | A - - - C5 - F5 - | Eb5 - - - D5 - Bb - | A - F# - A - D5 - |
```

Génération 9 (forme, la descente) : le chant aminci une seconde fois, des fragments de son énoncé ; la nappe reprend le cycle du début, puis tient un Sol sans tierce : après la bascule, ni majeur ni mineur.

```pattern notes "Chant E" bars=8 grid=8 octave=4 key="G dorian" role=melody
D5 - - - Bb - C5 - | D5 - - - - - . . | . . . . . . . . | E5 - - - - - . . |
D5 - - - Bb - . . | . . . . . . . . | . . . . . . . . | G - - - - - - - |
```

```pattern notes "Nappe A" bars=4 grid=4 octave=3 key="G dorian" role=pad
G3+D4+F4+Bb4 - - - | - - - - | G3+C4+E4+G4 - - - | - - - - |
```

```pattern notes "Nappe fin" bars=4 grid=4 octave=3 key="G minor" role=pad
G3+D4+A4 - - - | - - - - | - - - - | - - - - |
```

20 motifs.

## Arrangement

Form: F12 Deux sommets et une longue vallée

```arrangement tempo=120
section Montée 1-16 : Arp A, Basse P [from=9], Hat A [from=9]
section Sommet 1a 17-20 : Arp A, Basse A, Beat A, Hat A
section Sommet 1b 21-28 : Arp A, Basse A, Beat A [mute=28], Beat F [from=28], Hat A, Chant A
section Vallée 29-56 : Arp V, Nappe V, Hat V, Chant B [from=45 to=53], Basse V [from=45], Beat V [from=49]
section Sommet 2a 57-60 : Arp P, Nappe P, Basse D, Beat A, Hat A
section Sommet 2b 61-76 : Arp P, Nappe P, Basse D, Beat A, Hat A, Chant C
section Sommet 2c 77-80 : Arp P bascule, Nappe P bascule, Basse D bascule, Beat A [mute=80], Beat F [from=80], Hat A, Chant D
section Descente 81-96 : Arp A [to=93], Nappe A [to=93], Nappe fin [from=93], Basse A [to=89], Basse P [from=89 to=93], Beat A [to=85], Hat A [to=93], Chant E [to=89]
```

Longueurs : 16, 12 (4 + 8), 28, 24 (4 + 16 + 4), 16 mesures.

Cycles par section :

- **Montée** (1–16) et **premier sommet** (17–28) : Sol m7 – Do, deux mesures par accord.
- **Vallée** (29–56) : Sol m add9 – Mi♭ maj7, quatre mesures par accord ; elle finit sur Sol m add9 (53–56).
- **Second sommet** (57–80) : Sol m – Fa – Mi♭ – Ré m, une mesure par accord ; Ré majeur à la mesure 80.
- **Descente** (81–96) : Sol m7 – Do (81–92), puis Sol sans tierce (93–96).

Arc d'énergie : arpège seul et sourd (1–8) → basse en pédale et charley (9–16) → premier sommet, cinq parties puis le chant (17–28) → vallée, à moins de la moitié de l'énergie du sommet : arpège en croches, nappe, charley fantôme (29–44), puis le chant aminci et la pédale (45), la grosse caisse seule (49) → second sommet, six parties, grille riche, arpège sur deux octaves (57), triolets (73), la bascule (80) → descente : la grosse caisse part (85), la basse revient en pédale et le chant se tait (89), tout s'arrête sauf la nappe (93).

Coutures :

- **16 → 17** : l'arpège double sa vitesse sur le premier temps de 17, avec l'entrée de la batterie ; le filtre a fini d'ouvrir sa première marche une mesure plus tôt.
- **28 → 29** : la relance (le clap remplit le quatrième temps laissé par la grosse caisse), puis la batterie et la basse disparaissent d'un coup ; le charley ne s'arrête pas, il passe en fantôme : c'est lui qui relie.
- **44 → 45** et **48 → 49** : la vallée se repeuple par étapes (chant et pédale, puis une grosse caisse seule) : le retour est annoncé huit mesures avant.
- **56 → 57** : la vallée finit sur Sol m add9, l'accord sur lequel la grille riche commence ; la profondeur du LFO de la nappe retombe d'un coup.
- **80 → 81** : la relance sur Ré majeur, puis le retour de Sol m7 – Do : le Fa♯ se résout en Sol.

Événements uniques :

1. **29–48, structurel** : vingt mesures sans grosse caisse, où le pouls est le battement du filtre de la nappe.
2. **73–80** : l'arpège passe en triolets de doubles croches, la seule fois.
3. **80, structurel** : Ré majeur, la bascule de tierce, une seule mesure dans tout le morceau.
4. **93–96** : l'accord sans tierce, seul.

## Automation

```automation "Arp coupure A" part="Arp A" param=cutoff curve=ease-in
1.1 40, 16.4 75 linear, 28.4 88 step, 81.1 92 ease-out, 96.1 45
```

La coupure du Filter de l'arpège : de 400 Hz à 1,2 kHz sur la montée (lente puis rapide), jusqu'à 2 kHz au premier sommet (linéaire) ; dans la descente elle retombe de 2,5 kHz à 500 Hz (rapide puis lente : l'arpège s'assombrit vite puis s'éteint doucement).

```automation "Arp coupure V" part="Arp V" param=cutoff curve=smooth
29.1 55, 56.4 70
```

Dans la vallée elle repart de 600 Hz et remonte à 1 kHz, en S.

```automation "Arp coupure P" part="Arp P" param=cutoff curve=ease-in
57.1 70, 76.4 100
```

Au second sommet, de 1 kHz à 3 kHz (lente puis rapide), puis 4 kHz tenus pendant la bascule (un palier à 77).

```automation "Arp coupure bascule" part="Arp P bascule" param=cutoff curve=step
77.1 110
```

```automation "Basse coupure" part="Basse D" param=cutoff curve=linear
57.1 55, 76.4 82
```

La coupure du Filter de la basse, de 500 Hz à 1,4 kHz : le second sommet grossit par le jeu, pas par une partie de plus. Elle retombe à 500 Hz à la descente (palier à 81).

```automation "Nappe battement" part="Nappe V" cc=1 curve=smooth
29.1 8, 44.4 38 linear, 56.4 51 step
```

La profondeur du LFO du Filter de la nappe (LFO calé sur le tempo, à la noire ; le bouton va de 0 à 5 octaves) : 0,3 octave à 29, 1,5 à 44 (en S), 2 à 56 (linéaire) ; elle retombe à 0,4 à 57 (palier) pour laisser la place à la batterie.

```automation "Nappe battement fin" part="Nappe fin" cc=1 curve=linear
93.1 10, 96.4 38
```

Sur le dernier accord le battement revient (0,4 à 1,5 octave) : un souvenir de la vallée.

```automation "Nappe vallée" part="Nappe V" param=volume curve=step
29.1 108
```

```automation "Nappe sommet" part="Nappe P" param=volume curve=step
57.1 100
```

```automation "Nappe fondu" part="Nappe fin" param=volume curve=smooth
93.1 112, 96.4 85
```

Le volume de la nappe : −8 dB dans la vallée, où elle porte le morceau (palier), −12 dB au second sommet et dans la descente, puis −6 dB sur le dernier accord, seule, et un fondu en S jusqu'à −20 dB. (Premier rendu à −12 dB partout : la vallée se lisait à −23,6 dBFS, 8 dB sous le premier sommet, et le dernier accord à −31 dBFS.)

```automation "Basse pédale" part="Basse V" param=volume curve=step
45.1 88
```

Le volume de la basse tombe de −6 à −12 dB pour la pédale de la vallée (paliers à 45 et à 57) : au premier rendu la pédale tenue remontait la vallée au niveau du premier sommet (−15,9 dBFS).

La densité de l'arpège (réglages de l'arpégiateur, pas un contrôleur) : croches sur une octave de 1 à 16 ; doubles croches sur une octave de 17 à 28 ; croches de 29 à 56 ; doubles croches sur deux octaves de 57 à 72 ; triolets de doubles croches sur deux octaves de 73 à 80 ; croches sur une octave de 81 à 92. Dans Faulk : trois couloirs en paliers sur Cascade (Division, Type, Octaves).

## Notes de finition

Sons (Faulk) :

- **Batterie** : Drums d'usine.
- **Charley** : Drums sur sa piste, Swing (grille 1/8, quantité 60 %) avant l'instrument, Filter passe-haut 6 kHz.
- **Basse** : Swing (grille 1/8, 60 %) ; Oscillator dent de scie, attaque 5 ms, relâchement 200 ms ; Filter passe-bas 500 Hz, automatisé ; Compressor qui écoute la Batterie (seuil −24 dB, ratio 4).
- **Arp** : Cascade (Montant, durée 60 %) avant un Oscillator carré pincé (déclin 150 ms, maintien bas) ; Filter passe-bas automatisé ; Echo 1/8 pointé ; Reverb.
- **Nappe** : Oscillator dent de scie, attaque 60 ms, relâchement 500 ms ; Filter passe-bas 1,2 kHz dont le LFO est calé sur le tempo (noire), profondeur automatisée ; Bloom Ensemble ; Reverb longue.
- **Chant** : Oscillator carré, attaque 15 ms, relâchement 300 ms ; Filter passe-bas 900 Hz, fixe (pas d'ouverture) ; Echo noire ; Reverb (la pièce du plan du milieu).
- **Master** : Compressor (seuil −12 dB, ratio 2), Ceiling −0,3 dB.

Mix: Batterie: −10 dB, C, front (no Reverb), no width, 40–100 Hz and click above 2 kHz
Mix: Charley: −18 dB, L25 (own Drums track), middle (no Reverb, Filter highpass 6 kHz), no width, above 6 kHz
Mix: Basse: −6 dB (−12 dB bars 45–56), C, front (no Reverb, Filter lowpass 500 Hz, to 1.4 kHz bars 57–76, Compressor keyed by Batterie), no width, 40–250 Hz
Mix: Arp: −13 dB, R35, middle (Reverb size 0.4 damping 0.5 mix 0.2, Echo eighth_dotted feedback 0.3 mix 0.2, Filter lowpass 400 Hz to 4 kHz automated), no width, 200 Hz–4 kHz
Mix: Nappe: −12 dB (−8 dB bars 29–56, −6 to −20 dB bars 93–96), C, back (Reverb size 0.8 damping 0.7 mix 0.45, Filter lowpass 1.2 kHz with a synced LFO), Bloom ensemble stereo_phase 150 depth 40 % tone 300 Hz mix 0.45, 200 Hz–1.2 kHz
Mix: Chant: −9 dB, C, front edge of the room (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo quarter feedback 0.25 mix 0.2, Filter lowpass 900 Hz, fixed), no width, 400 Hz–1 kHz
Mono check: 1, 3 and 4 by reading (kick, bass and lead at C; Bloom only on the Nappe, tone 300 Hz, mix 0.45; no hard pan); 2 does not apply (no mirrored pair); the pad with Bloom off is left to the ear
Lead check: Chant, bars 61–76 (densest section), −14.6 dBFS RMS, −16.7 without the lead: 2.1 dB (first peak, bars 21–28: −15.2 and −17.3, 2.1 dB; valley, bars 45–52: −16.0 and −18.6, 2.7 dB; triplet bars 73–76: −14.6 and −16.4, 1.8 dB; the flip, bars 77–80: −14.4 and −16.7, 2.2 dB; thinned exit, bars 81–88, half rests: −16.1 and −17.1, 1.0 dB). No filter opening on the lead: nothing to compensate.

Master : Compressor (seuil −12 dB, ratio 2, compensation 10 dB), Ceiling −0,3 dB : crête −0,3 dBFS, −17,2 dBFS RMS, facteur de crête 16,8 dB (le profil : 11 à 16 dB).

Niveaux mesurés sur le rendu (RMS par section) : montée −26,9 puis −19,1 ; premier sommet −17,2 puis −15,2 ; vallée −20,6 (29–44, 29 % de l'énergie du sommet), −16,6 (45–56) ; second sommet −16,7 (57–60), −14,6 (61–76), −14,4 (77–80) ; descente −16,1, −17,7 ; dernier accord −24,5 dBFS. Le second sommet est 0,7 dB au-dessus du premier. La seconde moitié de la vallée (pédale, chant, grosse caisse) remonte plus haut que la fourchette du profil (35 à 50 %) : c'est le retour annoncé.

Humanisation : le Swing du charley et de la basse (grille 1/8, 60 %) ; les fantômes du charley à 60 ; rien d'autre.

Laissé à l'oreille : la profondeur du battement de la nappe (2 octaves à 56) ; la dureté de l'arpège en triolets filtre ouvert à 4 kHz (73–80) ; l'équilibre basse / grosse caisse ; le passage en triolets lui-même, lu dans le couloir et à l'écran mais pas mesuré.

Une seconde version pourrait : alterner vraiment deux cycles par section (« Où va le style » 1) ; lancer l'écho du chant sur ses fins de phrase ; ouvrir le filtre du chant au second sommet, avec la compensation de la règle du lead.

## Vérification

`python sheet_tool.py check fiche-col.md` :

```
[drums] 'Beat A'  bars=1 grid=16 notes=6

[drums] 'Hat A'  bars=1 grid=16 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Basse A'  bars=4 grid=8 notes=22
  OK     all 22 notes are in G dorian
  INFO   contour: range 19 semitones, highest note occurs 2x, steps 0 / leaps 17, up 68 / down 65 semitones, 5.5 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Arp A'  bars=4 grid=4 notes=8
  OK     all 8 notes are in G dorian

[notes] 'Basse P'  bars=4 grid=4 notes=1
  OK     all 1 notes are in G minor

[notes] 'Chant A'  bars=8 grid=8 notes=19
  OK     all 19 notes are in G dorian
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 9 / leaps 9, up 29 / down 31 semitones, 2.4 notes per bar

[drums] 'Beat F'  bars=1 grid=16 notes=6

[notes] 'Arp V'  bars=8 grid=4 notes=8
  OK     all 8 notes are in G minor

[notes] 'Nappe V'  bars=8 grid=4 notes=8
  OK     all 8 notes are in G minor

[drums] 'Hat V'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Chant B'  bars=8 grid=8 notes=8
  OK     all 8 notes are in G minor
  INFO   contour: range 6 semitones, highest note occurs 1x, steps 4 / leaps 3, up 6 / down 10 semitones, 1.0 notes per bar

[notes] 'Basse V'  bars=8 grid=4 notes=2
  OK     all 2 notes are in G minor

[drums] 'Beat V'  bars=1 grid=16 notes=1

[notes] 'Arp P'  bars=4 grid=4 notes=16
  OK     all 16 notes are in G minor

[notes] 'Nappe P'  bars=4 grid=4 notes=12
  OK     all 12 notes are in G minor

[notes] 'Basse D'  bars=4 grid=8 notes=21
  OK     all 21 notes are in G minor
  INFO   contour: range 17 semitones, highest note occurs 2x, steps 0 / leaps 16, up 91 / down 89 semitones, 5.2 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Chant C'  bars=16 grid=8 notes=42
  OK     all 42 notes are in G minor
  INFO   contour: range 17 semitones, highest note occurs 1x, steps 6 / leaps 32, up 79 / down 79 semitones, 2.6 notes per bar

[notes] 'Arp P bascule'  bars=4 grid=4 notes=16

[notes] 'Nappe P bascule'  bars=4 grid=4 notes=12

[notes] 'Basse D bascule'  bars=4 grid=8 notes=21
  INFO   contour: range 17 semitones, highest note occurs 2x, steps 0 / leaps 16, up 91 / down 89 semitones, 5.2 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Chant D'  bars=4 grid=8 notes=13
  INFO   contour: range 13 semitones, highest note occurs 1x, steps 4 / leaps 8, up 16 / down 21 semitones, 3.2 notes per bar

[notes] 'Chant E'  bars=8 grid=8 notes=8
  OK     all 8 notes are in G dorian
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 6 / down 13 semitones, 1.0 notes per bar

[notes] 'Nappe A'  bars=4 grid=4 notes=8
  OK     all 8 notes are in G dorian

[notes] 'Nappe fin'  bars=4 grid=4 notes=3
  OK     all 3 notes are in G minor

[arrangement] tempo=120
  Montée         bars   1-16  (16) 3 parts
                 edits: Basse P [from=9]; Hat A [from=9]
  Sommet 1a      bars  17-20  ( 4) 4 parts
  Sommet 1b      bars  21-28  ( 8) 6 parts
                 edits: Beat A [mute=28]; Beat F [from=28]
  Vallée         bars  29-56  (28) 6 parts
                 edits: Chant B [from=45 to=53]; Basse V [from=45]; Beat V [from=49]
  Sommet 2a      bars  57-60  ( 4) 5 parts
  Sommet 2b      bars  61-76  (16) 6 parts
  Sommet 2c      bars  77-80  ( 4) 7 parts
                 edits: Beat A [mute=80]; Beat F [from=80]
  Descente       bars  81-96  (16) 8 parts
                 edits: Arp A [to=93]; Nappe A [to=93]; Nappe fin [from=93]; Basse A [to=89]; Basse P [from=89 to=93]; Beat A [to=85]; Hat A [to=93]; Chant E [to=89]
  total 96 bars

[automation] 'Arp coupure A'  part='Arp A' cc=74 (cutoff) curve=ease-in points=5

[automation] 'Arp coupure V'  part='Arp V' cc=74 (cutoff) curve=smooth points=2

[automation] 'Arp coupure P'  part='Arp P' cc=74 (cutoff) curve=ease-in points=2

[automation] 'Arp coupure bascule'  part='Arp P bascule' cc=74 (cutoff) curve=step points=1
  NOTE   a single point is a constant value, not a move

[automation] 'Basse coupure'  part='Basse D' cc=74 (cutoff) curve=linear points=2

[automation] 'Nappe battement'  part='Nappe V' cc=1 (cc1) curve=smooth points=3

[automation] 'Nappe battement fin'  part='Nappe fin' cc=1 (cc1) curve=linear points=2

[automation] 'Nappe vallée'  part='Nappe V' cc=7 (volume) curve=step points=1
  NOTE   a single point is a constant value, not a move

[automation] 'Nappe sommet'  part='Nappe P' cc=7 (volume) curve=step points=1
  NOTE   a single point is a constant value, not a move

[automation] 'Nappe fondu'  part='Nappe fin' cc=7 (volume) curve=smooth points=2

[automation] 'Basse pédale'  part='Basse V' cc=7 (volume) curve=step points=1
  NOTE   a single point is a constant value, not a move

RESULT ok
```

Rendu MIDI : `col.mid` (24 pistes de motifs, 96 mesures à 120 bpm, 11 couloirs en contrôleurs).
