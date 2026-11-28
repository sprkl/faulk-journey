# Détour

## Brief et contraintes

Instrumental électronique mélodique, pensif, 108 bpm, **Mi mineur**, 72 mesures écrites en 4/4 (2 min 40). Le titre : un détour par une autre mesure. Le groove de départ (A) est en 4/4, à trois parties ; au milieu, B passe en **6/8** sans que la croche change de vitesse, dans le relatif majeur (Sol), la batterie réduite à un pouls, la mélodie en valeurs longues sur un autre son ; A revient en 4/4, et la cellule de B continue par-dessus, en noires pointées contre le 4/4.

Form: F8 A B A' avec un B dans une autre mesure

Profil : aucun

- **Tempo** : 108 bpm. A et A' en 4/4 ; B en 6/8, la croche constante (une mesure de 6/8 = trois noires de A).
- **Tonalité** : Mi mineur naturel ; B visite le relatif (Sol majeur) sans changer d'armure.
- **Palette par rôles** (sept pistes) : pouls = batterie (grosse caisse, clap) et un charley sur sa propre piste ; basse = triangle rond ; harmonie pincée = accords en dent de scie pincée (touches en A, arpège en B) ; nappe = dent de scie lente derrière un filtre passe-bande qui se déplace (elle n'existe qu'à partir de B) ; chant = carré adouci, le lead de A ; cloche = sinus pincé avec écho, le lead de B, puis le contre-chant de A'.
- **Longueur** : 72 mesures de 4/4 à l'écriture, soit 24 + 32 mesures de 6/8 + 24 (B : 24 mesures de 4/4 = 96 noires = 32 mesures de 6/8).
- **Forme** : F8, la carte de `forms.md` telle quelle (A 1–24, B 25–48, A' 49–72). Les deux fiches précédentes sont F10 (« Ronde ») et la forme à deux sommets de « Col » : exclues. Les cinq dernières : F10, deux sommets, F11, F9, F6 : pas de F0, mais le brief ne dit rien de la forme, donc F0 est écarté. Restent F1, F2, F3, F4, F7, F8 ; le brief ne donne pas d'humeur : je prends F8, la seule forme qui n'a jamais servi, et celle dont l'idée (un second monde par la mesure) met à l'épreuve ce que le produit n'a jamais eu à faire : changer de mesure en cours de morceau.

Trois contraintes :

1. **La croche ne change jamais de vitesse** : pas de changement de tempo ; seul le groupement change (par deux en A, par trois en B).
2. **Une cellule de trois notes (Si, Ré, Mi)** ouvre les deux mélodies : le chant de A la dit en noires, la cloche de B en valeurs pointées ; en A' la cloche la redit en noires pointées par-dessus le 4/4.
3. **A tient en trois parties** (pouls, basse, accords) jusqu'à la mesure 8 ; la nappe n'existe pas avant B, et reste en A' comme trace de la visite.

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Swing, Filter, Echo, Reverb, Bloom, Compressor, Ceiling) et ses presets d'usine. La notation de la fiche ne connaît que le 4/4 : les motifs de B sont écrits en croches (grid=8) dans des mesures de 4/4, par cycles de 3 mesures (quatre mesures de 6/8) ou de 6 mesures (huit mesures de 6/8) ; les mesures irrégulières sont nommées dans l'arrangement.

## Boucle de départ

Le porteur du pouls d'abord : une grosse caisse brisée (1, le « et » du 2, le 3 et demi), le clap sur deux et quatre.

```pattern drums "Beat A" bars=1 grid=16
Kick |x......x..x.....|
Clap |....x.......x...|
```

Le charley en croches, un fantôme sur la dernière double croche de chaque temps (c'est lui que le Swing retarde et humanise).

```pattern drums "Hat A" bars=1 grid=16
CHat |x.xox.xox.xox.xo|
```

Les accords pincés : trois touches par mesure (1, 2, le « et » du 3), un accord par mesure ; deux voix sur quatre ne bougent presque pas (Mi3 et Sol3).

```pattern notes "Accords A" bars=4 grid=8 octave=3 key="E minor" role=chords
E3+G3+B3+D4 . E3+G3+B3+D4 . . E3+G3+B3+D4 . . | E3+G3+B3+C4 . E3+G3+B3+C4 . . E3+G3+B3+C4 . . |
E3+G3+A3+C4 . E3+G3+A3+C4 . . E3+G3+A3+C4 . . | D3+F#3+A3+B3 . D3+F#3+A3+B3 . . D3+F#3+A3+B3 . . |
```

La basse : fondamentale, fondamentale, quinte, en 3 + 3 + 2 ; une levée à la fin du cycle.

```pattern notes "Basse A" bars=4 grid=8 octave=2 key="E minor" role=bass
E2 . . E2 . . B2 . | C2 . . C2 . . G2 . | A1 . . A1 . . E2 . | B1 . . B1 . F#2 B1 . |
```

## Variations

Génération 2, la mélodie : le chant de A, huit mesures (une phrase et sa réponse). La cellule Si – Ré – Mi l'ouvre ; un seul sommet (Sol5, mesure 3) ; la réponse retombe sur Si4.

```pattern notes "Chant A" bars=8 grid=8 octave=4 key="E minor" role=lead
B4 - D5 - E5 - - - | . . E5 - D5 - B4 - | A4 - C5 - E5 - G5 - | F#5 - - D5 - - B4 - |
B4 - D5 - E5 - - - | . . E5 - D5 - B4 - | A4 - C5 - E5 - F#5 - | D5 - - B4 - - - - |
```

Génération 3, la mesure : B en 6/8. Le pouls d'abord, réduit : la grosse caisse sur le premier temps de chaque mesure de 6/8, un clap sur le quatrième temps une mesure sur deux. Trois mesures de 4/4 = quatre mesures de 6/8.

```pattern drums "Beat B" bars=3 grid=8
Kick |x.....x.....x.....x.....|
Clap |.........x...........x..|
```

```pattern drums "Hat B" bars=3 grid=8
CHat |x.ox.ox.ox.ox.ox.ox.ox.o|
```

Génération 4, l'harmonie : le cycle de B, dans le relatif (Sol – Si m – Do – Ré), deux mesures de 6/8 par accord, soit six mesures de 4/4 par cycle. Les accords pincés deviennent un arpège en croches.

```pattern notes "Accords B" bars=6 grid=8 octave=3 key="G major" role=chords
G3 B3 D4 B3 D4 B3 G3 B3 | D4 B3 D4 B3 F#3 B3 D4 B3 | D4 B3 F#3 B3 D4 B3 D4 B3 |
G3 C4 E4 C4 E4 C4 G3 C4 | E4 C4 E4 C4 F#3 A3 D4 A3 | D4 A3 F#3 A3 D4 A3 D4 A3 |
```

La basse de B : la fondamentale sur le premier temps, la quinte en levée puis sur le quatrième temps.

```pattern notes "Basse B" bars=6 grid=8 octave=2 key="G major" role=bass
G2 - - . . D3 G2 - | - D3 - - B1 - - . | . F#2 B1 - - F#2 - - |
C2 - - . . G2 C2 - | - G2 - - D2 - - . | . A2 D2 - - A2 - - |
```

Génération 5, le son : la nappe, qui naît avec B. Un accord par deux mesures de 6/8 (douze croches).

```pattern notes "Nappe B" bars=6 grid=8 octave=3 key="G major" role=pad
B3+D4+G4 - - - - - - - | - - - - B3+D4+F#4 - - - | - - - - - - - - |
C4+E4+G4 - - - - - - - | - - - - A3+D4+F#4 - - - | - - - - - - - - |
```

Génération 6, la mélodie de B : la cloche, en valeurs longues (blanches pointées et noires pointées). La cellule Si – Ré – Mi l'ouvre ; un seul sommet (Sol5).

```pattern notes "Cloche B" bars=6 grid=8 octave=4 key="G major" role=lead
B4 - - - - - D5 - | - E5 - - F#5 - - - | - - D5 - - B4 - - |
E5 - - - - - G5 - | - E5 - - F#5 - - - | - - D5 - - A4 - - |
```

Génération 7, le retour : la nappe reste sous A', sur le cycle de A.

```pattern notes "Nappe A" bars=4 grid=4 octave=3 key="E minor" role=pad
G3+B3+D4 - - - | G3+B3+E4 - - - | G3+C4+E4 - - - | F#3+B3+D4 - - - |
```

La cellule de B par-dessus le 4/4 de A', une octave plus haut que le chant : trois noires pointées, puis la tenue ; elle traverse la barre de mesure.

```pattern notes "Cloche haute" bars=4 grid=8 octave=5 key="E minor" role=melody
B5 - - D6 - - E6 - | - - - - . . . . | E6 - - C6 - - A5 - | - - - - . . . . |
```

Génération 8, la forme : une relance et la fin. Le roulement de la mesure 48 ramène le 4/4 (doubles croches).

```pattern drums "Beat R" bars=1 grid=16
Kick |x.......x.......|
Clap |........o.o.oxxX|
```

```pattern notes "Nappe fin" bars=1 grid=4 octave=3 key="E minor" role=pad
G3+B3+E4 - - - |
```

```pattern notes "Cloche fin" bars=1 grid=4 octave=5 key="E minor" role=melody
E5 - - - |
```

Dispositif structurel : le changement de mesure, et en A' un trois contre deux tenu (la cloche en noires pointées sur le 4/4).

## Arrangement

Form: F8 A B A' avec un B dans une autre mesure

```arrangement tempo=108
section A1     1-8    : Beat A, Hat A [from=5], Basse A, Accords A
section A2     9-24   : Beat A [to=24.3], Hat A, Basse A [to=24.3], Accords A, Chant A
section B     25-48   : Nappe B, Accords B, Cloche B, Beat B [from=31 to=48], Hat B [from=31], Basse B [from=31], Beat R [from=48]
section A'1   49-56   : Beat A, Hat A, Basse A, Accords A, Nappe A, Cloche haute
section A'2   57-72   : Beat A [mute=64 to=72], Hat A [to=72], Basse A [to=72], Accords A [to=72], Nappe A [to=72], Chant A [to=72], Cloche haute [to=69], Nappe fin [from=72], Cloche fin [from=72]
```

Longueurs : 24 (8 + 16), 24, 24 (8 + 16) mesures de 4/4. **Mesures irrégulières, nommées** : B (25–48) se lit en 6/8, 32 mesures de 6/8 dans 24 mesures de 4/4 ; ses cycles font 6 mesures de 4/4 (huit mesures de 6/8), quatre cycles : 25–30, 31–36, 37–42, 43–48 ; les barres de 6/8 tombent toutes les trois noires (25.1, 25.4, 26.3, 27.2, 28.1…).

Cycles par section :

- **A** (1–24) et **A'** (49–71) : Mi m7 – Do maj7 – La m7 – Si m7, une mesure par accord.
- **B** (25–48) : Sol – Si m – Do – Ré, deux mesures de 6/8 par accord (six mesures de 4/4 par cycle).
- **Fin** (72) : Mi m tenu (Sol – Si – Mi à la nappe, Mi5 à la cloche).

Arc d'énergie : trois parties (1–4 sans charley, 5–8 avec) → le chant entre (9–24), le premier plateau → B : tout s'arrête sauf la mesure nouvelle ; le premier cycle (25–30) sans batterie ni basse, puis le pouls de 6/8 (31–48) ; la nappe s'éclaire, sa résonance monte dans le dernier cycle → roulement (48) → A' : le groove revient avec la nappe et la cellule de B en contre-rythme (49–56), puis le chant par-dessus (57–71) : le sommet, sept parties → l'accord final (72).

Coutures :

- **8 → 9** : rien ne s'arrête ; le chant entre sur le temps.
- **24 → 25** : la batterie et la basse lâchent les temps 3 et 4 de 24 (hésitation) ; le Si4 du chant tient ; à 25 le charley se tait, la mesure change.
- **30 → 31** : le pouls de 6/8 entre au début du deuxième cycle.
- **48 → 49** : la batterie de 6/8 se tait à 48 ; le roulement de clap en doubles croches ramène le 4/4 ; la résonance de la nappe retombe d'un coup à 49.
- **56 → 57** : le chant revient sur le temps ; la cloche continue.
- **71 → 72** : tout s'arrête sauf l'accord de Mi mineur à la nappe et le Mi5 de la cloche ; le chant finit sur Fa♯5 (71), la cloche lui répond Mi5.

Événements uniques :

1. **25, structurel** : le changement de mesure, 4/4 vers 6/8, croche constante.
2. **49, structurel** : le retour au 4/4, la cellule de B gardée par-dessus (trois contre deux).
3. **24.3** : la batterie et la basse lâchent deux temps.
4. **48** : le roulement de clap, la seule relance du morceau.
5. **64** : une mesure sans grosse caisse ni clap.
6. **72** : l'accord final, la cloche a le dernier mot.

## Automation

```automation "Nappe bande" part="Nappe B" param=cutoff curve=ease-in
25.1 50, 48.4 86, 49.1 62 step
```

La fréquence du Filter passe-bande de la nappe : de 500 Hz à 2 kHz pendant B (lente puis rapide), puis 900 Hz d'un coup au retour de A (le point de 48.4 saute à 49).

```automation "Nappe résonance" part="Nappe B" param=resonance curve=step
25.1 25, 43.1 25 ease-in, 48.4 76 step, 49.1 25
```

La résonance du même filtre : 20 % jusqu'au dernier cycle de B, puis de 20 % à 60 % sur 43–48 (lente puis rapide) : la bande se resserre et chante avant le retour ; 20 % d'un coup à 49.

```automation "Chant ouverture" part="Chant A" param=cutoff curve=smooth
57.1 62, 68.4 73
```

La coupure du Filter du chant : 900 Hz en A ; en A', de 900 Hz à 1,5 kHz sur 57–68 (en S). Ouverture bornée à moins d'une octave (0,74 octave) : pas de compensation de volume.

```automation "Accords fondu" part="Accords A" param=volume curve=ease-out
65.1 100, 71.4 80
```

Le volume des accords pincés baisse de 6 dB sur 65–71 (rapide puis lente) : la fin s'amincit sous le chant sans retirer de partie.

```automation "Nappe niveau" part="Nappe B" param=volume curve=step
25.1 110, 31.1 100
```

Le volume de la nappe : −6 dB pendant le premier cycle de B (25–30), où elle porte la cloche avec l'arpège seul, puis −10 dB d'un coup à 31 quand le pouls entre. Ajouté après le premier rendu : la cloche s'y lisait 4,2 dB au-dessus du reste.

## Notes de finition

Sons (Faulk), chacun parti d'un preset d'usine de l'Oscillator puis tordu :

- **Batterie** : Drums d'usine.
- **Charley** : Drums sur sa piste ; Swing avant l'instrument (grille 1/16, quantité 58 %, fenêtre 25 %, humanisation du temps 6 ms, humanisation de la vélocité 12, graine 7) ; Filter passe-haut 6 kHz.
- **Basse** : Round Bass (triangle), tel quel.
- **Accords** : Glass Pluck (attaque 2 ms, déclin 400 ms, maintien 0 %), forme d'onde changée en dent de scie ; Filter passe-bas 1,8 kHz ; Echo 1/8 pointé (retour 30 %, mélange 20 %) ; Reverb « Piece » (taille 40 %, amortissement 50 %, pré-délai 40 ms, mélange 20 %), enregistrée comme preset du projet et reprise par le chant et la cloche.
- **Nappe** : Soft Pad (dent de scie), attaque 300 ms ; Filter **passe-bande** 500 Hz, résonance 20 %, mélange 100 %, fréquence et résonance automatisées pendant B ; Bloom Ensemble (phase stéréo 150, tonalité 300 Hz, mélange 45 %) ; Reverb (taille 80 %, amortissement 70 %, mélange 45 %).
- **Chant** : Square Lead (carré) ; Filter passe-bas 900 Hz, ouvert à 1,5 kHz sur 57–68 ; Echo noire (retour 25 %, mélange 20 %) ; Reverb « Piece ».
- **Cloche** : Glass Pluck (sinus), déclin 900 ms, maintien 60 % (25 % au premier rendu) ; Echo 1/8 pointé (retour 30 %, mélange 25 %) ; Reverb « Piece ».
- **Master** : Compressor (seuil −12 dB, ratio 2, compensation 10 dB), Ceiling −0,3 dB.

Mix: Batterie: −10 dB, C, front (no Reverb), no width, 40–100 Hz and click above 2 kHz
Mix: Charley: −18 dB, L20 (own Drums track), middle (no Reverb, Filter highpass 6 kHz), no width, above 6 kHz
Mix: Basse: −6 dB, C, front (no Reverb), no width, 40–250 Hz
Mix: Accords: −12 dB (−12 to −18 dB bars 65–71), R30, middle (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo eighth_dotted feedback 0.3 mix 0.2, Filter lowpass 1.8 kHz), no width, 150 Hz–1.8 kHz
Mix: Nappe: −10 dB (−6 dB bars 25–30), C, back (Reverb size 0.8 damping 0.7 mix 0.45, Filter bandpass 500 Hz to 2 kHz bars 25–48, 900 Hz from bar 49, resonance 20 % to 60 % bars 43–48), Bloom ensemble stereo_phase 150 depth 40 % tone 300 Hz mix 0.45, one moving band 500 Hz–2 kHz
Mix: Chant: −9 dB, C, front edge of the room (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo quarter feedback 0.25 mix 0.2, Filter lowpass cutoff 900 Hz to 1.5 kHz bars 57–68, bounded opening of 0.74 octave, no volume compensation), no width, 500 Hz–1.5 kHz
Mix: Cloche: −8 dB, C, front edge of the room (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo eighth_dotted feedback 0.3 mix 0.25, no Filter: a sine), no width, 450 Hz–1.3 kHz
Mono check: 1, 3 and 4 by reading (kick, bass and both leads at C; the only Bloom is on the Nappe, behind a bandpass at 500 Hz or more, tone 300 Hz, mix 0.45; no hard pan); 2 does not apply (no mirrored pair); the Bloom switched off once is left to the ear
Lead check: Chant, bars 65–68 (end of its filter opening), −16.3 dBFS RMS, −17.6 without the lead: 1.3 dB (filter closed, bars 9–24: −16.5 and −18.3, 1.9 dB; first half of the opening, bars 57–64: −16.1 and −17.6, 1.5 dB; whole of its second section, bars 57–71: −16.3 and −17.8, 1.5 dB). Opening bounded to 0.74 octave (900 Hz to 1.5 kHz), no volume compensation. The lead sits 3 dB below the bass fader and was not moved between the two renders.
Lead check: Cloche, bars 31–48 (B with the pulse, the densest section where it leads), −17.3 dBFS RMS, −18.4 without the lead: 1.1 dB (last cycle, bars 43–48: −17.2 and −18.4, 1.1 dB). First cycle of B, bars 25–30 (pad and arpeggio only): −21.2 and −24.7, 3.5 dB, the edge of the band. Alone as a melody over the full groove, bars 49–56: −17.4 and −18.1, 0.7 dB, buried by the rule; as a counter-line under the Chant, bars 57–68: −16.2 and −16.6, 0.5 dB (under the lead by design). First render (sustain 25 %, fader −7 dB, pad at −10 dB in bars 25–30): 4.2 dB on bars 25–30 (on top), 0.85 dB on bars 31–48 (buried), 0.5 dB on bars 49–56. Second render: sustain 60 %, fader −8 dB (2 dB below the bass fader), pad at −6 dB on bars 25–30. The bell was not raised further: it would pass the bass fader before bars 49–56 read 1 dB.

Master : crête −0,3 dBFS, −17,3 dBFS RMS, facteur de crête 17,0 dB.

Niveaux mesurés sur le rendu (RMS par section) : A 1–4 −18,2 ; 5–8 −18,2 ; 9–24 −16,5 ; B 25–30 −21,2 ; 31–42 −17,4 ; 43–48 −17,2 ; A' 49–56 −17,4 ; 57–64 −16,1 ; 65–68 −16,3 ; 69–71 −16,9 ; accord final 72 −24,7 dBFS. A' avec le chant (57–68) est la section la plus forte, 0,3 dB au-dessus de A avec le chant (9–24).

Humanisation : le Swing du charley (grille 1/16, 58 %) avec 6 ms d'humanisation du temps et 12 de vélocité ; les fantômes à 60. L'effet de l'humanisation n'a pas été mesuré sur le rendu.

Laissé à l'oreille : tout (rien n'a été écouté, les niveaux et les leads sont mesurés sur les WAV) ; en particulier la couture 24 → 25 (le passage en 6/8), la bande de la nappe quand sa résonance monte à 60 % (43–48), la cloche seule sur le groove de 49 à 56 (0,7 dB), le trois contre deux de la cloche contre le 4/4.

Ce que Faulk n'a pas su dire : la mesure de B. Le projet est resté en 4/4 ; B est écrit en croches dans des mesures de 4/4, les barres de mesure de l'écran tombent au milieu des mesures de 6/8.

Une seconde version pourrait : retirer les accords pincés de 49 à 56 pour que la cloche y mène vraiment ; écrire B dans un projet qui sait changer de signature ; faire entrer la basse de B une mesure de 6/8 plus tôt.

## Vérification

`python sheet_tool.py check fiche-detour.md` :

```

[drums] 'Beat A'  bars=1 grid=16 notes=5

[drums] 'Hat A'  bars=1 grid=16 notes=12
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Accords A'  bars=4 grid=8 notes=48
  OK     all 48 notes are in E minor

[notes] 'Basse A'  bars=4 grid=8 notes=13
  OK     all 13 notes are in E minor
  INFO   contour: range 14 semitones, highest note occurs 1x, steps 0 / leaps 8, up 28 / down 33 semitones, 3.2 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Chant A'  bars=8 grid=8 notes=25
  OK     all 25 notes are in E minor
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 8 / leaps 13, up 29 / down 29 semitones, 3.1 notes per bar

[drums] 'Beat B'  bars=3 grid=8 notes=6

[drums] 'Hat B'  bars=3 grid=8 notes=16
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Accords B'  bars=6 grid=8 notes=48
  OK     all 48 notes are in G major
  INFO   contour: range 10 semitones, highest note occurs 4x, steps 0 / leaps 47, up 94 / down 92 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse B'  bars=6 grid=8 notes=16
  OK     all 16 notes are in G major
  INFO   contour: range 15 semitones, highest note occurs 2x, steps 0 / leaps 15, up 56 / down 54 semitones, 2.7 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Nappe B'  bars=6 grid=8 notes=12
  OK     all 12 notes are in G major

[notes] 'Cloche B'  bars=6 grid=8 notes=12
  OK     all 12 notes are in G major
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 3 / leaps 8, up 17 / down 19 semitones, 2.0 notes per bar

[notes] 'Nappe A'  bars=4 grid=4 notes=12
  OK     all 12 notes are in E minor

[notes] 'Cloche haute'  bars=4 grid=8 notes=6
  OK     all 6 notes are in E minor
  INFO   contour: range 7 semitones, highest note occurs 2x, steps 1 / leaps 3, up 5 / down 7 semitones, 1.5 notes per bar
  INFO   contour: the highest note repeats; a memorable line usually has a single peak

[drums] 'Beat R'  bars=1 grid=16 notes=8

[notes] 'Nappe fin'  bars=1 grid=4 notes=3
  OK     all 3 notes are in E minor

[notes] 'Cloche fin'  bars=1 grid=4 notes=1
  OK     all 1 notes are in E minor

[arrangement] tempo=108
  A1             bars   1-8   ( 8) 4 parts
                 edits: Hat A [from=5]
  A2             bars   9-24  (16) 5 parts
                 edits: Beat A [to=24.3]; Basse A [to=24.3]
  B              bars  25-48  (24) 7 parts
                 edits: Beat B [from=31 to=48]; Hat B [from=31]; Basse B [from=31]; Beat R [from=48]
  A'1            bars  49-56  ( 8) 6 parts
  A'2            bars  57-72  (16) 9 parts
                 edits: Beat A [mute=64 to=72]; Hat A [to=72]; Basse A [to=72]; Accords A [to=72]; Nappe A [to=72]; Chant A [to=72]; Cloche haute [to=69]; Nappe fin [from=72]; Cloche fin [from=72]
  total 72 bars

[automation] 'Nappe bande'  part='Nappe B' cc=74 (cutoff) curve=ease-in points=3

[automation] 'Nappe résonance'  part='Nappe B' cc=71 (resonance) curve=step points=4

[automation] 'Chant ouverture'  part='Chant A' cc=74 (cutoff) curve=smooth points=2

[automation] 'Accords fondu'  part='Accords A' cc=7 (volume) curve=ease-out points=2

[automation] 'Nappe niveau'  part='Nappe B' cc=7 (volume) curve=step points=2

RESULT ok
```

Rendu : `detour.mid` (16 pistes de parties, 72 mesures à 108 bpm, 5 couloirs d'automation en contrôleurs).

Notes construites dans Faulk comparées à la fiche (`check_notes.py` sur le dossier enregistré) : les 11 clips mélodiques identiques mesure par mesure (hauteurs, positions, longueurs), `RESULT ok` ; les 5 clips de batterie relus dans `notes.tsv` et dans le piano roll (Beat A 5, Beat B 6, Beat R 8 dont trois fantômes à 60 et un accent à 127, Hat A 12, Hat B 16) ; 22 placements sur les fenêtres de l'arrangement ; 5 couloirs, 13 points, courbes conformes.
