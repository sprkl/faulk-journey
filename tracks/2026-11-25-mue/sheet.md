# Mue

## Brief et contraintes

Form: F11 Morphose composée d'un trait

Profil : aucun

Brief du passage : pas de profil de style (rotation morzak → drifting-cycles → aucun), mes propres choix ; règles du lead de `references/mix.md` ; essayer Cascade et Sluice s'ils servent le morceau. Aucune humeur imposée : je vise un morceau qui dérive, calme au début, tendu au milieu, dépouillé à la fin.

- **Tempo** : 96 bpm, 4/4. Assez lent pour que la cellule rythmique du début se lise, assez vif pour que les doubles croches de l'arpège avancent.
- **Tonalité** : Do mineur (naturel) de 1 à 48, puis **Fa mineur** à la mesure 49 (une quarte au-dessus, une seule note change : Ré devient Ré♭). Le Do tenu à travers la coupure est la tonique de l'une et la quinte de l'autre.
- **Palette** (rôles, familles de sons) : pouls = Drums (kick, clap) et un charley sur sa propre piste ; basse = sinus ; harmonie = un clavier en dent de scie filtrée (S1), puis un arpège carré pincé fait par **Cascade** à partir d'accords tenus (S3, S4) ; lead = un chant sinus (S2), puis une cellule carrée derrière un passe-bas (S4, S5) ; texture = une nappe en dent de scie hachée par **Sluice**, qui écoute le charley (S5).
- **Longueur** : 96 mesures (4 min).
- **Forme** : F11. Les deux fiches précédentes sont F9 « Rappel » et F6 « Court-circuit » (exclues) ; les cinq dernières : F9, F6, F5, F4, F3. Pas de profil, pas d'humeur imposée, F0 écartée (le brief ne dit rien de la forme). Restent F1, F2, F7, F8, F10, F11 : F11 et F8 n'ont jamais servi ; F11 sert le mieux le matériau, parce que ses deux articulations (« la mélodie devient l'harmonie », « le rythme du début revient comme texture ») sont exactement ce que font un arpégiateur nourri d'accords tenus et une porte commandée par une autre piste.

Trois contraintes :

1. **Rien ne revient, tout descend de ce qui précède.** Chaque section naît d'un fragment de la précédente : le rythme des accords de S1 devient la cellule de basse de S2 ; les notes du chant de S2 deviennent les accords de S3 ; le groupement par trois doubles croches de l'arpège de S3 devient la cellule de S4 ; le rythme de S1 revient en S5, non comme partie mais comme découpe d'une nappe.
2. **Aucun arpège écrit.** Les arpèges ne sont que des accords tenus de quatre notes ; c'est Cascade qui les égrène.
3. **Une seule cellule rythmique syncopée**, 3 + 3 + 4 + 6 doubles croches (attaques aux pas 1, 4, 7, 11), d'où viennent le clavier, la basse A, le kick de S2 et le charley de S5.

Hypothèses : sons d'usine de Faulk (Oscillator, Drums) ; pas de voix ; rien n'est écouté par un humain pendant le passage, tout est mesuré sur l'export.

## Boucle de départ

Le porteur du pouls d'abord : un kick lent, sur le premier et le dernier appui de la cellule.

```pattern drums "Beat S" bars=1 grid=16
Kick |x.........x.....|
```

```pattern drums "Hat S" bars=1 grid=16
CHat |....o.......o...|
```

Le charley ne marque que le contretemps lent, en fantôme : le pouls reste creux.

Puis ce qui définit le morceau : la boucle d'accords, quatre mesures, Do m9 – La♭ maj7 – Fa m7 – Sol m7, jouée sur la cellule 3 + 3 + 4 + 6. La voix du haut descend d'un ton et remonte (Ré, Do, Do, Si♭).

```pattern notes "Clavier A" bars=4 grid=16 octave=4 key="C minor" role=chords
C3+Eb4+G4+D5 - . C3+Eb4+G4+D5 - . C3+Eb4+G4+D5 - - . C3+Eb4+G4+D5 - - - . . |
Ab2+Eb4+G4+C5 - . Ab2+Eb4+G4+C5 - . Ab2+Eb4+G4+C5 - - . Ab2+Eb4+G4+C5 - - - . . |
F2+Eb4+Ab4+C5 - . F2+Eb4+Ab4+C5 - . F2+Eb4+Ab4+C5 - - . F2+Eb4+Ab4+C5 - - - . . |
G2+D4+F4+Bb4 - . G2+D4+F4+Bb4 - . G2+D4+F4+Bb4 - - . G2+D4+F4+Bb4 - - - . . |
```

## Variations

Génération 2 (harmonie → basse) : la boucle rétrécit en une cellule de deux mesures. La basse garde le rythme du clavier et ses fondamentales, deux accords par mesure au lieu d'un. La levée de Si♭ ramène au Do.

```pattern notes "Basse A" bars=2 grid=16 octave=2 key="C minor" role=bass
C - . C - . Eb - . . Ab1 - - - . . |
F1 - . F1 - . Ab1 - . . G1 - - - Bb1 - |
```

Génération 3 (rythme) : la batterie prend la cellule (kick aux pas 1, 7, 11) et le charley passe en doubles croches balancées (le device Swing en 1/16 retarde la quatrième double de chaque temps).

```pattern drums "Beat W" bars=1 grid=16
Kick |x.....x...x.....|
Clap |....x.......x...|
```

```pattern drums "Hat W" bars=1 grid=16
CHat |x.oxx.oxx.oxx.ox|
```

Génération 4 (mélodie) : le chant, seize mesures. La première phrase pose une question (elle finit sur Ré, loin de la tonique) ; la seconde reprend le début, monte à son seul sommet (Sol5, mesure 15) et répond sur Do.

```pattern notes "Chant" bars=16 grid=8 octave=4 key="C minor" role=melody
G - - Bb - - C5 - | D5 - - C5 - - Bb - | C5 - - - - - . . | . . G - Bb - C5 - |
Eb5 - - D5 - - C5 - | D5 - - C5 - - Bb - | C5 - - - D5 - Eb5 - | D5 - - - - - . . |
G - - Bb - - C5 - | D5 - - C5 - - Bb - | C5 - - - - - . . | . . G - Bb - C5 - |
Eb5 - - D5 - - C5 - | F5 - - Eb5 - - D5 - | G5 - - - F5 - Eb5 - | C5 - - - - - - - |
```

Génération 5 (mélodie → harmonie) : les notes du chant, deux mesures par deux mesures, empilées en accords tenus : {Sol, Si♭, Do, Ré}, {Do, Sol, Si♭}, {Mi♭, Ré, Do, Fa}, {Sol, Fa, Mi♭, Do}. Cascade les égrène (montant-descendant, doubles croches, deux octaves). La basse leur donne quatre fondamentales nouvelles : Do, Mi♭, La♭, Si♭.

```pattern notes "Arp C" bars=8 grid=4 octave=4 key="C minor" role=chords
C4+G4+Bb4+D5 - - - | - - - - | G3+C4+G4+Bb4 - - - | - - - - |
C4+Eb4+F4+D5 - - - | - - - - | C4+Eb4+F4+G4 - - - | - - - - |
```

```pattern notes "Basse C" bars=8 grid=8 octave=2 key="C minor" role=bass
C . C . . C . C | C . . C . G . C3 |
Eb . Eb . . Eb . Eb | Eb . . Eb . Bb . Eb3 |
Ab1 . Ab1 . . Ab1 . Ab1 | Ab1 . . Ab1 . Eb . Ab |
Bb1 . Bb1 . . Bb1 . Bb1 | Bb1 . . Bb1 . F . G |
```

Génération 6 (rythme) : la batterie change de pied, du balancé au droit : quatre temps au sol, charley ouvert sur chaque contretemps, plus aucune double croche (le Swing n'a donc plus rien à retarder).

```pattern drums "Beat D" bars=1 grid=16
Kick |x...x...x...x...|
Clap |....x.......x...|
```

```pattern drums "Hat D" bars=1 grid=16
CHat |o...o...o...o...|
OHat |..x...x...x...x.|
```

Échange de rôles (événement structurel, mesures 45–48) : la basse chante les quatre premières mesures du chant, deux octaves plus bas.

```pattern notes "Basse chant" bars=4 grid=8 octave=2 key="C minor" role=bass
G - - Bb - - C3 - | D3 - - C3 - - Bb - | C3 - - - - - . . | . . G - Bb - C3 - |
```

Le Do tenu à travers la coupure (mesures 47–48), par le son du chant :

```pattern notes "Tenue Do" bars=2 grid=4 octave=5 key="C minor" role=pad
C - - - | - - - - |
```

Le roulement de la mesure 48 : il s'arrête avant le quatrième temps, qui reste vide.

```pattern drums "Roulement" bars=1 grid=16
Kick |x...x...........|
Clap |....x.x.oxox....|
```

Génération 7 (harmonie) : l'harmonie se déplace en Fa mineur. Cycle D : Fa m7 – Mi♭ – Ré♭ maj7 – Mi♭ add9, deux mesures par accord.

```pattern notes "Arp D" bars=8 grid=4 octave=3 key="F minor" role=chords
F3+Ab3+C4+Eb4 - - - | - - - - | Eb3+G3+Bb3+Eb4 - - - | - - - - |
Db3+F3+Ab3+C4 - - - | - - - - | Eb3+G3+Bb3+F4 - - - | - - - - |
```

```pattern notes "Basse D" bars=8 grid=8 octave=2 key="F minor" role=bass
F . F F3 . F . F3 | F . F F3 . F C Eb |
Eb . Eb Eb3 . Eb . Eb3 | Eb . Eb Eb3 . Eb Bb1 Eb |
Db . Db Db3 . Db . Db3 | Db . Db Db3 . Db Ab1 Db |
Eb . Eb Eb3 . Eb . Eb3 | Eb . Eb Eb3 . Eb G Bb |
```

Génération 8 (la troisième idée) : la cellule. Elle prend à l'arpège de S3 son groupement par trois doubles croches (3 + 3 + 3 + 3 + 2 + 2) et sa figure montante-descendante ; huit mesures, deux par accord ; un seul sommet, Fa5 à la mesure 7.

```pattern notes "Cellule A" bars=8 grid=16 octave=4 key="F minor" role=lead
C5 - . Ab - . C5 - . Eb5 - . C5 - Ab - | Bb - . Ab - . F - . Ab - . C5 - - - |
Bb - . G - . Bb - . Eb5 - . Bb - G - | Ab - . G - . Eb - . G - . Bb - - - |
Ab - . F - . Ab - . C5 - . Ab - F - | Ab - . F - . Db - . F - . Ab - - - |
Bb - . G - . Bb - . Eb5 - . F5 - Eb5 - | Db5 - . Bb - . G - . Bb - . C5 - - - |
```

```pattern drums "Beat E" bars=1 grid=16
Kick |x...x...x...x.x.|
Clap |....x.......x...|
```

```pattern drums "Hat E" bars=1 grid=16
CHat |x.o.x.o.x.o.x...|
OHat |..............x.|
```

Les huit dernières mesures de S4 accélèrent vers Fa : Ré♭ maj7 – Mi♭7 – Fa m add9 (quatre mesures).

```pattern notes "Arp E" bars=8 grid=4 octave=3 key="F minor" role=chords
Db3+F3+Ab3+C4 - - - | - - - - | Eb3+G3+Bb3+Db4 - - - | - - - - |
F3+Ab3+C4+G4 - - - | - - - - | - - - - | - - - - |
```

```pattern notes "Basse E" bars=8 grid=8 octave=2 key="F minor" role=bass
Db . Db Db3 . Db . Db3 | Db . Db Db3 . Db Ab1 Db |
Eb . Eb Eb3 . Eb . Eb3 | Eb . Eb Eb3 . Eb G Bb |
F . F F3 . F . F3 | F . F F3 . F C Eb |
F . F F3 . F . F3 | F . F F3 . F C Eb |
```

S5 : il ne reste que la cellule, réduite à ses deux premières mesures, puis à ses premières notes, puis à un Do tenu (la quinte : la fin ne se résout pas).

```pattern notes "Cellule F" bars=2 grid=16 octave=4 key="F minor" role=lead
C5 - . Ab - . C5 - . Eb5 - . C5 - Ab - | Bb - . Ab - . F - . Ab - . C5 - - - |
```

```pattern notes "Cellule fin" bars=8 grid=16 octave=4 key="F minor" role=lead
C5 - . Ab - . C5 - . Eb5 - . C5 - Ab - | Bb - . Ab - . F - . Ab - . C5 - - - |
C5 - . Ab - . C5 - . . . . . . . . | . . . . . . . . . . . . . . . . |
C5 - . Ab - . . . . . . . . . . . | . . . . . . . . . . . . . . . . |
C5 - - - - - - - - - - - - - - - | - - - - - - - - . . . . . . . . |
```

La texture : une nappe tenue (Fa m add9, Ré♭ maj7 sur pédale de Fa, Fa m add9), que Sluice n'ouvre que sous le charley ; le charley rejoue la cellule de S1.

```pattern notes "Trame" bars=24 grid=4 octave=3 key="F minor" role=pad
F3+C4+G4+Ab4 - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - |
Db3+Ab3+C4+F4 - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - |
F3+C4+G4+Ab4 - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - |
```

```pattern notes "Trame éclat" bars=1 grid=4 octave=3 key="F minor" role=pad
F3+C4+G4+Ab4 - - - |
```

```pattern drums "Hat R" bars=1 grid=16
CHat |x..x..x...x.....|
```

```pattern notes "Basse P" bars=4 grid=4 octave=1 key="F minor" role=bass
F - - - | - - - - | - - - - | - - - - |
```

```pattern drums "Clap seul" bars=1 grid=16
Clap |........x.......|
```

28 motifs : la forme n'a pas de retour, donc pas de motif qui resserve ; au-delà de vingt, c'est assumé.

## Arrangement

Form: F11 Morphose composée d'un trait

```arrangement tempo=96
section S1 1-12 : Clavier A [to=12.3], Beat S, Hat S, Basse A [from=12.3]
section S2 13-28 : Basse A, Chant, Beat W [mute=28], Hat W [mute=28]
section S3 29-48 : Arp C [to=48.4], Basse C [to=45], Basse chant [from=45 to=48.4], Beat D [to=48], Hat D [to=48], Roulement [from=48], Tenue Do [from=47]
section S4 49-72 : Arp D [to=65], Arp E [from=65 to=72], Basse D [to=65], Basse E [from=65 to=72], Cellule A, Beat E [mute=72], Hat E [mute=64,72], Hat R [from=64 to=65], Trame éclat [from=64 to=65]
section S5 73-96 : Cellule F [to=89], Cellule fin [from=89], Trame, Hat R [to=95], Beat S [from=81 to=89], Basse P [from=81 to=93], Clap seul [from=92 to=93]
```

Longueurs : 12, 16, 20, 24, 24 mesures (la carte F11, 12 – 16 – 20 – 24 – 24).

Cycles par section :

- **S1** (1–12) : Do m9 – La♭ maj7 – Fa m7 – Sol m7, une mesure par accord.
- **S2** (13–28) : pas d'accords ; la basse sous-entend Do m – La♭ | Fa m – Sol m, deux par mesure.
- **S3** (29–48) : Do sus9 – Mi♭6 – La♭ maj7♯11 – Si♭ sus4 add9, deux mesures par accord (les notes du chant sur de nouvelles fondamentales ; La♭ est l'accord commun avec S1).
- **S4** (49–72), en Fa mineur : Fa m7 – Mi♭ – Ré♭ maj7 – Mi♭ add9 (49–64), puis Ré♭ maj7 – Mi♭7 – Fa m add9 (65–71).
- **S5** (73–96) : Fa m add9 (8) – Ré♭ maj7 sur Fa (8) – Fa m add9 (8), pédale de Fa de 81 à 92.

Arc : pas de sommet par empilement ; l'intensité monte par la subdivision (noires pointées, croches, doubles croches) et l'ouverture des filtres jusqu'à 64–71, puis tout est retiré d'un coup à 72.

Coutures :

- **12 → 13** : le clavier se tait à 12.3 (son dernier accord manque), la basse entre à 12.3 par la fin de sa cellule (Sol, levée de Si♭). Anticipation par l'harmonie.
- **28 → 29** : la batterie et le charley se taisent à la mesure 28 ; le chant tient son Do, la basse finit sa cellule. Une partie s'arrête une mesure plus tôt.
- **48 → 49** (le changement de tonalité) : coupure franche. Le roulement s'arrête à 48.3, tout se tait au quatrième temps sauf le Do tenu depuis 47 par le son du chant ; à 49 tout change sur le premier temps.
- **72 → 73** : la mesure 72 ne garde que la cellule ; S5 commence avec elle.

Événements uniques :

1. **45–48, structurel** : échange de rôles, la basse chante le début du chant pendant que l'arpège tient l'harmonie.
2. **47–48** : un Do tenu par le son du chant, qu'on n'a plus entendu depuis 28, à travers le silence de 48.4.
3. **64** : une mesure de la texture de S5 en avance (le charley joue la cellule de S1, la nappe hachée apparaît) ; on ne la comprend qu'à 73.
4. **72, structurel** : toutes les parties s'arrêtent, la cellule dit seule sa huitième mesure.
5. **92.3** : un seul clap, le seul de S5.

## Automation

```automation "Clavier ouverture" part="Clavier A" param=cutoff curve=ease-out
1.1 40, 12.2 85
```

La coupure du Filter du clavier, de 400 Hz à 1,6 kHz : la boucle s'éclaircit vite puis se pose (rapide puis lente).

```automation "Arp ouverture" part="Arp C" param=cutoff curve=smooth
29.1 45, 44.4 100 step
```

La coupure du Filter de l'arpège, de 500 Hz à 3 kHz, en S : l'arpège sort de l'ombre sans à-coup ; elle tient jusqu'à la coupure de 49.

```automation "Arp D coupure" part="Arp D" param=cutoff curve=step
49.1 70, 65.1 70 ease-in, 71.4 110
```

Elle retombe d'un coup à 1,2 kHz au changement de tonalité (palier), puis s'ouvre jusqu'à 4 kHz sur les sept dernières mesures (lente puis rapide : la poussée finale).

```automation "Cellule coupure" part="Cellule A" param=cutoff curve=ease-in
49.1 55, 64.4 92
```

La coupure du Filter de la cellule, de 700 Hz à 2,4 kHz (1,8 octave), lente puis rapide.

```automation "Cellule volume" part="Cellule A" param=volume curve=ease-in
49.1 100, 64.4 92
```

Le volume de la cellule baisse de 2 dB sur les mêmes mesures (−8,5 → −10,5 dB) : la compensation de l'ouverture, règle du lead.

```automation "Cellule fermeture" part="Cellule fin" param=cutoff curve=ease-out
89.1 92, 96.1 50
```

La coupure redescend à 600 Hz sur les huit dernières mesures : la cellule s'éteint en s'assombrissant.

```automation "Trame fondu" part="Trame" param=volume curve=smooth
89.1 95, 96.4 40
```

Le volume de la nappe, de −7 à −30 dB, en S : la fin est une dissolution faite par l'arrangement et par ce seul fondu. (Premier rendu à −12 dB : la nappe hachée se lisait 10 dB sous la cellule en 73–80 ; remontée à −7 dB.)

## Notes de finition

Sons (Faulk) :

- **Batterie** : Drums d'usine.
- **Charley** : Drums, **Swing** (grille 1/16, quantité 62 %) avant l'instrument, Filter passe-haut 6 kHz.
- **Basse** : Oscillator sinus, attaque 5 ms, relâchement 200 ms ; Compressor qui écoute la Batterie (seuil −24 dB, ratio 4).
- **Clavier** : Oscillator dent de scie, relâchement 250 ms ; Filter passe-bas automatisé ; Bloom Ensemble ; Reverb.
- **Arp** : **Cascade** (Montant-descendant, 1/16, 2 octaves, durée 60 %) avant un Oscillator carré pincé (déclin 150 ms, maintien bas) ; Filter passe-bas automatisé ; Echo 1/8 pointé ; Reverb.
- **Chant** : Oscillator sinus, attaque 20 ms, relâchement 400 ms ; Echo noire ; Reverb (la pièce du plan du milieu).
- **Cellule** : Oscillator carré ; Filter passe-bas automatisé ; Bloom Chorus ; Echo et Reverb du Chant (presets du projet).
- **Trame** : Oscillator dent de scie, attaque 50 ms ; Filter passe-bas 2 kHz ; **Sluice** qui écoute le Charley (profondeur 18 dB : porte fermée, la nappe reste un lit lointain) ; Bloom Ensemble ; Reverb longue.
- **Master** : Compressor (seuil −12 dB, ratio 2), Ceiling −0,3 dB.

Mix: Batterie: −10 dB, C, front (no Reverb), no width, 40–100 Hz and click above 2 kHz
Mix: Charley: −18 dB, L25 (own Drums track), middle (no Reverb, Filter highpass 6 kHz), no width, above 6 kHz
Mix: Basse: −6 dB, C, front (no Reverb, Compressor keyed by Batterie), no width, 40–250 Hz
Mix: Clavier: −12 dB, C, middle (Reverb size 0.4 damping 0.5 mix 0.25, Filter lowpass 400 Hz to 1.6 kHz bars 1–12), Bloom ensemble stereo_phase 150 depth 40 % tone 300 Hz mix 0.45, 100 Hz–2 kHz
Mix: Arp: −13 dB, R35, middle (Reverb size 0.4 damping 0.5 mix 0.2, Echo eighth_dotted feedback 0.3 mix 0.2, Filter lowpass 500 Hz to 4 kHz automated), no width, 150 Hz–4 kHz
Mix: Chant: −7 dB, C, front edge of the room (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo quarter feedback 0.25 mix 0.2, no Filter), no width, 400 Hz–1.6 kHz
Mix: Cellule: −8.5 dB, C, front edge of the room (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo quarter feedback 0.25 mix 0.2, Filter lowpass), Bloom chorus stereo_phase 90 mix 0.25, 350 Hz–2.5 kHz ; cutoff 700 Hz to 2.4 kHz bars 49–64, volume −2 dB over the same bars (−8.5 to −10.5 dB)
Mix: Trame: −7 dB, C, back (Reverb size 0.8 damping 0.7 mix 0.45, Filter lowpass 2 kHz, Sluice keyed by Charley depth 18 dB), Bloom ensemble stereo_phase 150 depth 40 % tone 300 Hz mix 0.45, 170 Hz–2 kHz
Mono check: 1, 3 and 4 by reading (kick, bass and leads at C; Bloom on the Clavier and the Trame with tone 300 Hz and mix 0.45, on the Cellule with mix 0.25; no hard pan); 2 does not apply (no mirrored pair); the pads with Bloom off are left to the ear
Lead check: Chant, bars 13–28, −16.8 dBFS RMS, −19.2 without the lead: 2.4 dB (second phrase, bars 21–28: −16.8 and −19.1, 2.4 dB; held C, bars 47–48: −16.3 and −18.8, 2.6 dB)
Lead check: Cellule, bars 61–64 (end of the opening), −15.6 dBFS RMS, −17.1 without the lead: 1.4 dB (filter closed, bars 49–52: −14.8 and −17.1, 2.3 dB; bars 53–60: −15.2 and −17.2, 2.0 dB; open, bars 65–71: −15.9 and −17.2, 1.4 dB; S5 with drums and bass, bars 81–88: −16.0 and −17.5, 1.5 dB; S5 where the form leaves it alone over the gated pad, bars 73–80: −20.1 and −26.3, 6.3 dB, by design and left to the ear)

Humanisation : le Swing du charley (S2, et de nouveau S5 par la cellule) ; les fantômes à 60 ; rien d'autre.

Laissé à l'oreille : le niveau de la nappe hachée face à la cellule en S5 ; la dureté du carré de l'arpège filtre ouvert (65–71) ; le seuil de Sluice.

Une seconde version pourrait : moduler la division de Cascade (1/8 en S3, 1/16 en S4) ; faire écouter à Sluice une piste muette plutôt que le charley audible ; passer S5 en 6/8.

## Vérification

`python sheet_tool.py check fiche-mue.md` :

```

[drums] 'Beat S'  bars=1 grid=16 notes=2

[drums] 'Hat S'  bars=1 grid=16 notes=2
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Clavier A'  bars=4 grid=16 notes=64
  OK     all 64 notes are in C minor

[notes] 'Basse A'  bars=2 grid=16 notes=9
  OK     all 9 notes are in C minor
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 1 / leaps 5, up 9 / down 11 semitones, 4.5 notes per bar

[drums] 'Beat W'  bars=1 grid=16 notes=5

[drums] 'Hat W'  bars=1 grid=16 notes=12
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Chant'  bars=16 grid=8 notes=40
  OK     all 40 notes are in C minor
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 27 / leaps 12, up 51 / down 46 semitones, 2.5 notes per bar

[notes] 'Arp C'  bars=8 grid=4 notes=16
  OK     all 16 notes are in C minor

[notes] 'Basse C'  bars=8 grid=8 notes=32
  OK     all 32 notes are in C minor
  INFO   contour: range 19 semitones, highest note occurs 1x, steps 1 / leaps 10, up 45 / down 38 semitones, 4.0 notes per bar

[drums] 'Beat D'  bars=1 grid=16 notes=6

[drums] 'Hat D'  bars=1 grid=16 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Basse chant'  bars=4 grid=8 notes=10
  OK     all 10 notes are in C minor
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 6 / leaps 3, up 14 / down 9 semitones, 2.5 notes per bar

[notes] 'Tenue Do'  bars=2 grid=4 notes=1
  OK     all 1 notes are in C minor

[drums] 'Roulement'  bars=1 grid=16 notes=8

[notes] 'Arp D'  bars=8 grid=4 notes=16
  OK     all 16 notes are in F minor

[notes] 'Basse D'  bars=8 grid=8 notes=44
  OK     all 44 notes are in F minor
  INFO   contour: range 21 semitones, highest note occurs 3x, steps 2 / leaps 32, up 166 / down 161 semitones, 5.5 notes per bar

[notes] 'Cellule A'  bars=8 grid=16 notes=44
  OK     all 44 notes are in F minor
  INFO   contour: range 16 semitones, highest note occurs 1x, steps 11 / leaps 32, up 66 / down 66 semitones, 5.5 notes per bar

[drums] 'Beat E'  bars=1 grid=16 notes=7

[drums] 'Hat E'  bars=1 grid=16 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Arp E'  bars=8 grid=4 notes=12
  OK     all 12 notes are in F minor

[notes] 'Basse E'  bars=8 grid=8 notes=44
  OK     all 44 notes are in F minor
  INFO   contour: range 21 semitones, highest note occurs 6x, steps 2 / leaps 33, up 166 / down 164 semitones, 5.5 notes per bar

[notes] 'Cellule F'  bars=2 grid=16 notes=11
  OK     all 11 notes are in F minor
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 2 / leaps 8, up 16 / down 16 semitones, 5.5 notes per bar

[notes] 'Cellule fin'  bars=8 grid=16 notes=17
  OK     all 17 notes are in F minor
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 2 / leaps 12, up 24 / down 24 semitones, 2.1 notes per bar

[notes] 'Trame'  bars=24 grid=4 notes=12
  OK     all 12 notes are in F minor

[notes] 'Trame éclat'  bars=1 grid=4 notes=4
  OK     all 4 notes are in F minor

[drums] 'Hat R'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Basse P'  bars=4 grid=4 notes=1
  OK     all 1 notes are in F minor

[drums] 'Clap seul'  bars=1 grid=16 notes=1
  NOTE   no kick in this pattern: fine if another part carries the pulse

[arrangement] tempo=96
  S1             bars   1-12  (12) 4 parts
                 edits: Clavier A [to=12.3]; Basse A [from=12.3]
  S2             bars  13-28  (16) 4 parts
                 edits: Beat W [mute=28]; Hat W [mute=28]
  S3             bars  29-48  (20) 7 parts
                 edits: Arp C [to=48.4]; Basse C [to=45]; Basse chant [from=45 to=48.4]; Beat D [to=48]; Hat D [to=48]; Roulement [from=48]; Tenue Do [from=47]
  S4             bars  49-72  (24) 9 parts
                 edits: Arp D [to=65]; Arp E [from=65 to=72]; Basse D [to=65]; Basse E [from=65 to=72]; Beat E [mute=72]; Hat E [mute=64,72]; Hat R [from=64 to=65]; Trame éclat [from=64 to=65]
  S5             bars  73-96  (24) 7 parts
                 edits: Cellule F [to=89]; Cellule fin [from=89]; Hat R [to=95]; Beat S [from=81 to=89]; Basse P [from=81 to=93]; Clap seul [from=92 to=93]
  total 96 bars

[automation] 'Clavier ouverture'  part='Clavier A' cc=74 (cutoff) curve=ease-out points=2

[automation] 'Arp ouverture'  part='Arp C' cc=74 (cutoff) curve=smooth points=2

[automation] 'Arp D coupure'  part='Arp D' cc=74 (cutoff) curve=step points=3

[automation] 'Cellule coupure'  part='Cellule A' cc=74 (cutoff) curve=ease-in points=2

[automation] 'Cellule volume'  part='Cellule A' cc=7 (volume) curve=ease-in points=2

[automation] 'Cellule fermeture'  part='Cellule fin' cc=74 (cutoff) curve=ease-out points=2

[automation] 'Trame fondu'  part='Trame' cc=7 (volume) curve=smooth points=2

RESULT ok
```

`python sheet_tool.py render fiche-mue.md --out mue.mid` : 28 pistes de motifs, 96 mesures à 96 bpm, 7 couloirs en contrôleurs.

Vérifié : la notation (RESULT ok, toutes les notes dans leur tonalité) ; les notes du projet Faulk contre la fiche, clip par clip (`verification-notes.txt`, RESULT ok) ; les niveaux et les deux lead checks sur l'export (`analyse-wav.txt`) ; la découpe de la nappe par Sluice sur l'export (crêtes aux pas 1, 4, 7, 11 de la mesure 73). Non vérifié : rien n'a été écouté ; le balancement du charley n'a pas été mesuré à ce passage.
