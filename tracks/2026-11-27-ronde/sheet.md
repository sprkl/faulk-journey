# Ronde

## Brief et contraintes

Instrumental électronique mélodique et clair, 122 bpm, **Do majeur** puis **Ré majeur**, 80 mesures (2 min 37). Le titre : une ronde, le refrain qui revient. Le groove de départ (A) revient trois fois sans que ses notes changent ; entre ses retours, deux visites : B, sans batterie, dans le relatif mineur, sur un autre son et sous une pédale de basse ; C, sans basse, en trois contre quatre, sur un accord suspendu qui ne se résout qu'au retour de A. À chaque retour, A garde quelque chose de la visite : le registre après B, le rythme de C dans le charley et le son de B en contre-chant au dernier. Ce dernier retour se hausse d'un ton à 70 % du morceau.

Form: F10 Rondo (A B A C A)

Profil : drifting-cycles

Profil de style : **drifting-cycles** (demandé par le brief ; rotation morzak → drifting-cycles → aucun).

- **Tempo** : 122 bpm, 4/4, la lecture « danse » du profil (118–126), lue telle quelle (pas de demi-temps).
- **Tonalité** : Do majeur ; B visite le relatif (La mineur) sans changer d'armure ; un seul changement de tonalité, la hausse d'un ton vers Ré majeur à la mesure 57.
- **Palette par rôles** (sept pistes) : pouls = batterie (grosse caisse, clap) et un charley sur sa propre piste ; basse = triangle rond, capable de tenir une pédale (preset d'usine Round Bass) ; harmonie pincée = accords pincés, par touches (Glass Pluck, forme d'onde changée en dent de scie pour que le filtre ait de quoi ouvrir) ; nappe = dent de scie lente et large (Soft Pad, attaque raccourcie) ; accroche = carré adouci et légèrement épaissi, le lead du refrain (Square Lead) ; cloche = sinus pincé avec écho (Glass Pluck, déclin allongé), le son de B, puis le contre-chant et la coda.
- **Longueur** : 80 mesures (2 min 37), la carte de F10 telle quelle.
- **Forme** : F10 Rondo. Les deux fiches précédentes sont la forme à deux sommets (« Col », sans numéro dans `forms.md`) et F11 « Mue » : exclues. Les cinq dernières : deux sommets, F11, F9, F6, F5. Le profil nomme F4, F9, F10 et F1 : F9 a servi au dernier passage drifting-cycles (le 24), F4 à celui d'avant (le 20), F1 le 17 ; F10 n'a jamais servi avec ce profil (une seule fois, sans profil, le 18). Carte : A 1–16, B 17–24, A 25–40 (l'accroche une octave plus haut), C 41–48, A 49–72 à pleine force (haussé d'un ton à 57), coda 73–80.

Trois contraintes (deux gestes du profil, une de moi) :

1. *(profil, geste 1)* **Un cycle par section, avec un accord d'ancrage** : A = Do add9 – La m7 – Fa maj7 – Sol sus4 ; B = La m7 – Fa maj7 – Ré m7 – Mi m7 (ancrages La m7 et Fa maj7) ; C = Fa maj7 – Sol sus4 (les deux derniers accords de A, étirés) ; le dernier A haussé = Ré add9 – Si m7 – Sol maj7 – La sus4.
2. *(profil, gestes 2 et 4)* **Une hausse tardive d'un ton à 70 %** (mesure 57 sur 80), précédée d'une mesure amincie (56 : ni batterie, ni basse, ni accords pincés) et d'une note commune (Ré, quarte de Sol sus4 et tonique de Ré) ; et **l'accord suspendu de C** (Sol sus4, 45–48) ne se résout qu'au retour de A (49).
3. *(la mienne)* **A ne change jamais ses notes** : chaque retour du refrain est le même matériau (transposé d'une octave ou d'un ton, jamais réécrit) ; ce qui change vient des visites. Le morceau se construit donc comme trois scènes (A, B, C) envoyées dans l'arrangement.

Signature du profil : la **pédale** (B : la basse tient La sous quatre accords, et ne bouge que sur le premier accord du retour de A, mesure 25) ; et **la même mélodie deux fois sur des accords différents** : la cloche de B rejoue l'accroche note pour note, sur les accords du relatif.

Ce que je garde du profil : majeur avec visite du relatif, cycles de 4 accords, accords étendus (add9, m7, maj7, sus4), pédale, hausse tardive unique, accroche courte de 8 notes énoncée tôt et réharmonisée, longue phrase chantée dans le dernier tiers (le contre-chant de la cloche, 57–72), balancement sur le charley seulement, roulement une seule fois avant un changement de section (48), pompage par sidechain, contraste entre harmonie lente (B, C) et rapide (A). Ce que je plie : pas d'intro sans accords (le rondo pose son refrain dès la première mesure). Ce que je laisse : la montée de bruit filtré (l'Oscillator n'a pas de bruit ; la tension de C vient d'un filtre qui s'ouvre sur les accords).

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Swing, Filter, Echo, Reverb, Bloom, Compressor, Ceiling) et ses presets d'usine.

## Catalogue d'attributs (profil drifting-cycles, adapté)

- **Son** : un lead carré épaissi, une couche pincée, une nappe chaude et large, un sub propre qui tient une pédale, un pompage par sidechain.
- **Harmonie** : Do majeur, relatif mineur au milieu, accords étendus et suspendus, un cycle par section, une hausse d'un ton à 70 %.
- **Mélodie** : une accroche de 8 notes, réharmonisée ; une longue phrase chantée dans le dernier tiers.
- **Rythme** : quatre temps au sol ; trois contre quatre pour la visite C, puis dans le charley ; balancement sur le charley seul ; un roulement avant le retour.
- **Forme** : rondo, le refrain trois fois, deux visites, une coda.
- **Tempo** : 122 bpm.

## Boucle de départ

Le porteur du pouls d'abord : quatre temps au sol, clap sur deux et quatre ; le charley en contretemps avec un fantôme sur la dernière double croche (c'est lui que le Swing retarde).

```pattern drums "Beat A" bars=1 grid=16
Kick |x...x...x...x...|
Clap |....x.......x...|
```

```pattern drums "Hat A" bars=1 grid=16
CHat |..xo..xo..xo..xo|
```

Puis ce qui définit le refrain : les accords pincés, en 3 + 3 + 2, un accord par mesure ; deux voix sur quatre ne bougent presque pas (Mi3 et Do4).

```pattern notes "Accords A" bars=4 grid=8 octave=3 key="C major" role=chords
E3+G3+C4+D4 . . E3+G3+C4+D4 . . E3+G3+C4+D4 . | E3+G3+A3+C4 . . E3+G3+A3+C4 . . E3+G3+A3+C4 . |
E3+F3+A3+C4 . . E3+F3+A3+C4 . . E3+F3+A3+C4 . | D3+G3+C4+D4 . . D3+G3+C4+D4 . . D3+G3+C4+D4 . |
```

La basse : la fondamentale en croches espacées, l'octave et une levée en fin de mesure.

```pattern notes "Basse A" bars=4 grid=8 octave=2 key="C major" role=bass
C . C . C . C3 C | A1 . A1 . A1 . A A1 | F1 . F1 . F1 . F F1 | G1 . G1 . G1 . G D |
```

L'accroche : huit notes sur le rythme des accords, un seul sommet (La, mesure 3) ; énoncée d'abord dans le médium.

```pattern notes "Accroche A" bars=4 grid=8 octave=4 key="C major" role=melody
E - - D - - C - | E - - - - - . . | A - - G - - E - | D - - - - - . . |
```

La nappe : trois voix, un accord par mesure.

```pattern notes "Nappe A" bars=4 grid=4 octave=3 key="C major" role=pad
G3+D4+E4 - - - | G3+C4+E4 - - - | A3+C4+E4 - - - | G3+C4+D4 - - - |
```

## Variations

Génération 2 (harmonie, la visite B) : le relatif mineur, deux mesures par accord (l'harmonie ralentit), et la basse en pédale sur La.

```pattern notes "Nappe B" bars=8 grid=4 octave=3 key="A minor" role=pad
G3+A3+C4+E4 - - - | - - - - | F3+A3+C4+E4 - - - | - - - - | F3+A3+C4+D4 - - - | - - - - | E3+G3+B3+D4 - - - | - - - - |
```

```pattern notes "Basse B" bars=8 grid=4 octave=1 key="A minor" role=bass
A1 - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - |
```

Génération 3 (son, la signature) : la cloche rejoue l'accroche note pour note, une octave plus haut, sur les accords de B : Mi Ré Do Mi sur La m7 puis sur Ré m7, La Sol Mi Ré sur Fa maj7 puis sur Mi m7.

```pattern notes "Cloche B" bars=4 grid=8 octave=5 key="A minor" role=melody
E - - D - - C - | E - - - - - . . | A - - G - - E - | D - - - - - . . |
```

Génération 4 (registre) : le premier retour garde le registre de la visite : l'accroche une octave plus haut.

```pattern notes "Accroche 8va" bars=4 grid=8 octave=5 key="C major" role=melody
E - - D - - C - | E - - - - - . . | A - - G - - E - | D - - - - - . . |
```

Génération 5 (rythme, la visite C) : trois contre quatre. La grosse caisse, le charley et les accords frappent toutes les trois doubles croches ; pas de basse.

```pattern drums "Beat C" bars=1 grid=16
Kick |x.....x.....x...|
```

```pattern drums "Hat C" bars=1 grid=16
CHat |x..x..x..x..x..x|
```

```pattern notes "Accords C F" bars=1 grid=16 octave=3 key="C major" role=chords
E3+A3+C4 . . E3+A3+C4 . . E3+A3+C4 . . E3+A3+C4 . . E3+A3+C4 . . E3+A3+C4 |
```

```pattern notes "Accords C G" bars=1 grid=16 octave=3 key="C major" role=chords
D3+G3+C4 . . D3+G3+C4 . . D3+G3+C4 . . D3+G3+C4 . . D3+G3+C4 . . D3+G3+C4 |
```

```pattern notes "Nappe C" bars=8 grid=4 octave=3 key="C major" role=pad
F3+A3+E4 - - - | - - - - | - - - - | - - - - | G3+C4+D4 - - - | - - - - | - - - - | - - - - |
```

Génération 6 (rythme) : le roulement, une seule fois, à la mesure 48.

```pattern drums "Beat R" bars=1 grid=16
Kick |x...x...........|
Clap |....x...o.o.xxxX|
```

Génération 7 (forme, la hausse) : la note commune. Ré, quarte de Sol sus4, tenu par la cloche sur la mesure amincie ; il devient la tonique.

```pattern notes "Tenue" bars=1 grid=4 octave=5 key="C major" role=lead
D - - - |
```

Génération 8 (harmonie, la hausse) : le refrain un ton plus haut, note pour note (copies transposées, rien de réécrit).

```pattern notes "Accords A2" bars=4 grid=8 octave=3 key="D major" role=chords
F#3+A3+D4+E4 . . F#3+A3+D4+E4 . . F#3+A3+D4+E4 . | F#3+A3+B3+D4 . . F#3+A3+B3+D4 . . F#3+A3+B3+D4 . |
F#3+G3+B3+D4 . . F#3+G3+B3+D4 . . F#3+G3+B3+D4 . | E3+A3+D4+E4 . . E3+A3+D4+E4 . . E3+A3+D4+E4 . |
```

```pattern notes "Basse A2" bars=4 grid=8 octave=2 key="D major" role=bass
D . D . D . D3 D | B1 . B1 . B1 . B B1 | G1 . G1 . G1 . G G1 | A1 . A1 . A1 . A E |
```

```pattern notes "Accroche A2" bars=4 grid=8 octave=5 key="D major" role=melody
F# - - E - - D - | F# - - - - - . . | B - - A - - F# - | E - - - - - . . |
```

```pattern notes "Nappe A2" bars=4 grid=4 octave=3 key="D major" role=pad
A3+E4+F#4 - - - | A3+D4+F#4 - - - | B3+D4+F#4 - - - | A3+D4+E4 - - - |
```

Génération 9 (mélodie) : la longue phrase chantée du dernier tiers, à la cloche, sous l'accroche : de longues notes, une note de l'accord sur chaque premier temps, un seul sommet (Fa♯5, mesure 7). Elle part du Ré tenu.

```pattern notes "Chant long" bars=8 grid=8 octave=4 key="D major" role=melody
D5 - - - - - - - | F# - - - - - A - | B - - - - - - - | A - - - E - - - |
F# - - - - - - - | D5 - - - - - B - | D5 - - - - - F#5 - | E5 - - - - - - - |
```

Génération 10 (forme, la coda) : l'accroche seule, sur le son doux de B, puis l'accord tenu.

```pattern notes "Cloche coda" bars=4 grid=8 octave=5 key="D major" role=melody
F# - - E - - D - | F# - - - - - . . | B - - A - - F# - | E - - - - - . . |
```

```pattern notes "Nappe fin" bars=4 grid=4 octave=3 key="D major" role=pad
A3+E4+F#4 - - - | - - - - | - - - - | - - - - |
```

24 motifs, dont sept sont des copies transposées (octave ou ton) d'un autre.

## Arrangement

Form: F10 Rondo (A B A C A)

```arrangement tempo=122
section A1a 1-8 : Basse A, Accords A, Hat A, Beat A [from=5]
section A1b 9-16 : Beat A, Hat A, Basse A, Accords A, Nappe A, Accroche A
section B 17-24 : Basse B, Nappe B, Cloche B, Hat A [mute=19-23]
section A2 25-40 : Beat A, Hat A, Basse A [to=40], Accords A, Nappe A, Accroche 8va
section C 41-48 : Beat C [to=48], Beat R [from=48], Hat C, Accords C F [to=45], Accords C G [from=45], Nappe C
section A3 49-56 : Beat A [to=56], Hat A [to=56], Basse A [to=56], Accords A [to=56], Nappe A, Accroche 8va, Tenue [from=56]
section A4 57-72 : Beat A, Hat C, Basse A2, Accords A2, Nappe A2, Accroche A2, Chant long
section Coda 73-80 : Nappe A2 [to=77], Nappe fin [from=77], Cloche coda [to=79]
```

Longueurs : 16 (8 + 8), 8, 16, 8, 24 (8 + 16), 8 mesures.

Cycles par section :

- **A** (1–16, 25–40, 49–56) : Do add9 – La m7 – Fa maj7 – Sol sus4, une mesure par accord.
- **B** (17–24) : La m7 – Fa maj7 – Ré m7 – Mi m7, deux mesures par accord, sur une pédale de La.
- **C** (41–48) : Fa maj7 (41–44) – Sol sus4 (45–48), quatre mesures par accord, sans basse.
- **A haussé** (57–72) et **coda** (73–76) : Ré add9 – Si m7 – Sol maj7 – La sus4 ; puis Ré add9 tenu (77–80).

Arc d'énergie : le refrain posé en deux temps (1–8 sans nappe ni accroche, 9–16 complet) → B, à moins de la moitié : pas de batterie, une pédale, la cloche → retour de A, l'accroche une octave plus haut → C, la tension : trois contre quatre, pas de basse, le filtre des accords s'ouvre, un roulement → A à pleine force (49), mesure amincie (56), **hausse d'un ton** (57) : le sommet, sept parties, le rythme de C dans le charley, la cloche de B en contre-chant → coda : l'accroche seule à la cloche, l'accord tenu.

Coutures :

- **16 → 17** : la batterie, les accords et l'accroche s'arrêtent net ; le charley continue deux mesures (17–18) : c'est lui qui relie.
- **24 → 25** : le charley revient une mesure avant (24) ; la basse quitte sa pédale sur le premier temps de 25.
- **40 → 41** : la basse se tait une mesure plus tôt (40).
- **48 → 49** : le roulement de clap, la grosse caisse lâche les temps 3 et 4 ; Sol sus4 se résout en Do add9.
- **56 → 57** : mesure amincie (nappe, accroche et le Ré de la cloche seulement) ; le Ré est redit sur le premier temps de 57, où il est la tonique (dans la notation, deux notes : la tenue ne traverse pas la barre de section).
- **72 → 73** : tout s'arrête sauf la nappe ; la cloche reprend l'accroche.

Événements uniques :

1. **17–24, structurel** : huit mesures sans batterie, sous une pédale.
2. **41–48, structurel** : huit mesures sans basse, en trois contre quatre.
3. **48** : le roulement de clap, la seule relance du morceau.
4. **56–57, structurel** : la mesure amincie et la hausse d'un ton.
5. **73–78** : l'accroche jouée par la cloche, seule (échange de rôle).

## Automation

```automation "Accroche coupure" part="Accroche 8va" param=cutoff curve=ease-in
49.1 62, 56.4 86
```

La coupure du Filter de l'accroche : 900 Hz jusqu'à 49, puis de 900 Hz à 2,2 kHz sur 49–56 (lente puis rapide) ; elle reste ouverte pour la hausse.

```automation "Accroche volume" part="Accroche 8va" param=volume curve=linear
49.1 100, 56.4 97
```

Le volume de l'accroche baisse de 1 dB sur les mêmes mesures (−9 à −10 dB) : la compensation de l'ouverture. Premier rendu à 2 dB (−11 dB), le bas de la fourchette de la règle : le lead se lisait enterré en fin d'ouverture (0,91 dB) ; à 1 dB il tient (1,07 dB). Chiffres versés à la question ouverte sur la compensation.

```automation "Nappe coupure B" part="Nappe B" param=cutoff curve=smooth
17.1 52, 24.4 84
```

La coupure du Filter de la nappe s'ouvre pendant B, de 600 Hz à 2,5 kHz (en S) : la visite s'éclaire sans batterie ; elle revient à 1,2 kHz au retour de A (palier à 25).

```automation "Accords coupure C" part="Accords C F" param=cutoff curve=ease-in
41.1 55, 48.4 100
```

La coupure du Filter des accords, de 700 Hz à 4 kHz pendant C (lente puis rapide) : la montée qui tient lieu de bruit filtré ; elle retombe à 1,5 kHz à 49 (palier).

```automation "Nappe fondu" part="Nappe fin" param=volume curve=smooth
77.1 104, 80.4 80
```

Le fondu de l'accord final, en S (−8 à −20 dB). Dans Faulk le même couloir tient la nappe à −12 dB de 1 à 72 (palier) et la monte à −8 dB pour la coda, où elle porte seule la cloche (palier à 73).

## Notes de finition

Sons (Faulk), chacun parti d'un preset d'usine de l'Oscillator puis tordu :

- **Batterie** : Drums d'usine.
- **Charley** : Drums sur sa piste, Swing (grille 1/16, quantité 58 %) avant l'instrument, Filter passe-haut 6 kHz.
- **Basse** : Round Bass (triangle, attaque 3 ms, déclin 250 ms, maintien 60 %, relâchement 80 ms) ; Compressor qui écoute la Batterie (seuil −24 dB, ratio 4) : le pompage.
- **Accords** : Glass Pluck (attaque 2 ms, déclin 400 ms, maintien 0 %), forme d'onde changée en dent de scie ; Filter passe-bas 1,5 kHz, automatisé pendant C (700 Hz à 4 kHz) ; Echo 1/8 pointé (retour 30 %, mélange 20 %) ; Reverb « Piece » (taille 40 %, amortissement 50 %, pré-délai 40 ms, mélange 20 %), enregistrée comme preset du projet et reprise par l'accroche et la cloche.
- **Nappe** : Soft Pad (dent de scie), attaque 300 ms, relâchement 600 ms ; Filter passe-bas 1,2 kHz, automatisé pendant B ; Bloom Ensemble (phase stéréo 150, tonalité 300 Hz, mélange 45 %) ; Reverb (taille 80 %, amortissement 70 %, mélange 45 %) ; Compressor qui écoute la Batterie (seuil −24 dB, ratio 4).
- **Accroche** : Square Lead (carré, attaque 5 ms, maintien 75 %, relâchement 200 ms) ; Filter passe-bas 900 Hz, ouvert à 2,2 kHz sur 49–56 ; Bloom Chorus (phase 90, mélange 25 %) ; Echo noire (retour 25 %, mélange 20 %) ; Reverb « Piece ».
- **Cloche** : Glass Pluck (sinus), déclin 900 ms, maintien 25 % ; Echo 1/8 pointé (retour 30 %, mélange 25 %) ; Reverb « Piece ».
- **Master** : Compressor (seuil −12 dB, ratio 2, compensation 10 dB), Ceiling −0,3 dB.

Mix: Batterie: −10 dB, C, front (no Reverb), no width, 40–100 Hz and click above 2 kHz
Mix: Charley: −18 dB, L25 (own Drums track), middle (no Reverb, Filter highpass 6 kHz), no width, above 6 kHz
Mix: Basse: −6 dB, C, front (no Reverb, Compressor keyed by Batterie), no width, 40–250 Hz
Mix: Accords: −12 dB, R35, middle (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo eighth_dotted feedback 0.3 mix 0.2, Filter lowpass 1.5 kHz, 700 Hz to 4 kHz bars 41–48), no width, 150 Hz–4 kHz
Mix: Nappe: −12 dB (−8 dB bars 73–76, −8 to −20 dB bars 77–80), C, back (Reverb size 0.8 damping 0.7 mix 0.45, Filter lowpass 1.2 kHz, 600 Hz to 2.5 kHz bars 17–24, Compressor keyed by Batterie), Bloom ensemble stereo_phase 150 depth 40 % tone 300 Hz mix 0.45, 200 Hz–2.5 kHz
Mix: Accroche: −9 dB, C, front edge of the room (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo quarter feedback 0.25 mix 0.2, Filter lowpass cutoff 900 Hz to 2.2 kHz bars 49–56, volume −1 dB over the same bars), Bloom chorus stereo_phase 90 mix 0.25, 500 Hz–2.2 kHz
Mix: Cloche: −7 dB, C, front edge of the room (Reverb size 0.4 damping 0.5 mix 0.2 predelay 0.04, Echo eighth_dotted feedback 0.3 mix 0.25, no Filter: a sine), no width, 500 Hz–1 kHz
Mono check: 1, 3 and 4 by reading (kick, bass and both leads at C; Bloom on the Nappe with tone 300 Hz and mix 0.45, on the Accroche with stereo_phase 90 and mix 0.25; no hard pan); 2 does not apply (no mirrored pair); each Bloom switched off once is left to the ear
Lead check: Accroche, bars 53–55 (end of its filter opening), −17.0 dBFS RMS, −18.1 without the lead: 1.1 dB (filter closed, bars 25–40: −16.3 and −18.1, 1.8 dB; first statement an octave lower, bars 9–16: −16.9 and −18.0, 1.1 dB; start of the opening, bars 49–52: −16.5 and −18.0, 1.5 dB; open, densest section, bars 57–72: −16.4 and −17.5, 1.0 dB). Opening of 1.3 octave compensated by 1 dB, below the 2 to 4 dB of the rule: at 2 dB the lead read buried (0.9 dB on bars 53–55, 0.85 dB on bars 57–72). The lead was not raised: it stays 3 to 4 dB below the bass fader.
Lead check: Cloche, bars 17–24 (the only section where it leads with other parts), −18.2 dBFS RMS, −19.7 without the lead: 1.5 dB. As a counter-line under the Accroche, bars 57–72: −16.4 and −17.0, 0.6 dB (under the chords by design, and buried by the lead rule: the long phrase of the last third is more felt than heard; it sits 1 dB below the bass fader and was not raised). Alone over the pad, bars 73–76: −20.7 and −23.3, 2.7 dB (no meaning as a blend figure: nothing else plays).

Master : crête −0,3 dBFS, −17,5 dBFS RMS, facteur de crête 17,2 dB.

Niveaux mesurés sur le rendu (RMS par section) : A 1–4 −19,1 ; 5–8 −18,3 ; 9–16 −16,9 ; B 17–24 −18,2 ; A 25–40 −16,3 ; C 41–44 −18,8, 45–48 −19,0 ; A 49–52 −16,5, 53–55 −17,0 ; mesure amincie 56 −18,9 ; A haussé 57–72 −16,4 ; coda 73–76 −20,7, 77–80 −23,5 dBFS. Le dernier refrain n'est pas plus fort que le deuxième (−16,4 contre −16,3) : son sommet tient à la hausse d'un ton, au charley en trois contre quatre et au contre-chant, pas au niveau ; à l'oreille de dire si cela suffit.

Humanisation : le Swing du charley (grille 1/16, 58 %) ; les fantômes à 60 ; rien d'autre.

Laissé à l'oreille : tout (rien n'a été écouté, les niveaux et les leads sont mesurés sur les WAV) ; en particulier la cloche en contre-chant (0,6 dB), le pompage de la basse et de la nappe, la dureté des accords filtre ouvert à 4 kHz (mesure 48), la couture 56 → 57 (le Ré tenu puis redit).

Une seconde version pourrait : faire entendre la longue phrase de la cloche en retirant les accords pincés de 65 à 72 ; tenir vraiment le Ré à travers la barre 56 → 57 (une note de deux mesures) ; donner à C une vraie montée de bruit quand un oscillateur de bruit existera.

## Vérification

`python sheet_tool.py check fiche-ronde.md` :

```

[drums] 'Beat A'  bars=1 grid=16 notes=6

[drums] 'Hat A'  bars=1 grid=16 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Accords A'  bars=4 grid=8 notes=48
  OK     all 48 notes are in C major

[notes] 'Basse A'  bars=4 grid=8 notes=20
  OK     all 20 notes are in C major
  INFO   contour: range 19 semitones, highest note occurs 1x, steps 1 / leaps 10, up 50 / down 48 semitones, 5.0 notes per bar

[notes] 'Accroche A'  bars=4 grid=8 notes=8
  OK     all 8 notes are in C major
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 9 / down 11 semitones, 2.0 notes per bar

[notes] 'Nappe A'  bars=4 grid=4 notes=12
  OK     all 12 notes are in C major

[notes] 'Nappe B'  bars=8 grid=4 notes=16
  OK     all 16 notes are in A minor

[notes] 'Basse B'  bars=8 grid=4 notes=1
  OK     all 1 notes are in A minor

[notes] 'Cloche B'  bars=4 grid=8 notes=8
  OK     all 8 notes are in A minor
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 9 / down 11 semitones, 2.0 notes per bar

[notes] 'Accroche 8va'  bars=4 grid=8 notes=8
  OK     all 8 notes are in C major
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 9 / down 11 semitones, 2.0 notes per bar

[drums] 'Beat C'  bars=1 grid=16 notes=3

[drums] 'Hat C'  bars=1 grid=16 notes=6
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Accords C F'  bars=1 grid=16 notes=18
  OK     all 18 notes are in C major

[notes] 'Accords C G'  bars=1 grid=16 notes=18
  OK     all 18 notes are in C major

[notes] 'Nappe C'  bars=8 grid=4 notes=6
  OK     all 6 notes are in C major

[drums] 'Beat R'  bars=1 grid=16 notes=9

[notes] 'Tenue'  bars=1 grid=4 notes=1
  OK     all 1 notes are in C major

[notes] 'Accords A2'  bars=4 grid=8 notes=48
  OK     all 48 notes are in D major

[notes] 'Basse A2'  bars=4 grid=8 notes=20
  OK     all 20 notes are in D major
  INFO   contour: range 19 semitones, highest note occurs 1x, steps 1 / leaps 10, up 50 / down 48 semitones, 5.0 notes per bar

[notes] 'Accroche A2'  bars=4 grid=8 notes=8
  OK     all 8 notes are in D major
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 9 / down 11 semitones, 2.0 notes per bar

[notes] 'Nappe A2'  bars=4 grid=4 notes=12
  OK     all 12 notes are in D major

[notes] 'Chant long'  bars=8 grid=8 notes=12
  OK     all 12 notes are in D major
  INFO   contour: range 14 semitones, highest note occurs 1x, steps 4 / leaps 7, up 22 / down 20 semitones, 1.5 notes per bar

[notes] 'Cloche coda'  bars=4 grid=8 notes=8
  OK     all 8 notes are in D major
  INFO   contour: range 9 semitones, highest note occurs 1x, steps 4 / leaps 3, up 9 / down 11 semitones, 2.0 notes per bar

[notes] 'Nappe fin'  bars=4 grid=4 notes=3
  OK     all 3 notes are in D major

[arrangement] tempo=122
  A1a            bars   1-8   ( 8) 4 parts
                 edits: Beat A [from=5]
  A1b            bars   9-16  ( 8) 6 parts
  B              bars  17-24  ( 8) 4 parts
                 edits: Hat A [mute=19-23]
  A2             bars  25-40  (16) 6 parts
                 edits: Basse A [to=40]
  C              bars  41-48  ( 8) 6 parts
                 edits: Beat C [to=48]; Beat R [from=48]; Accords C F [to=45]; Accords C G [from=45]
  A3             bars  49-56  ( 8) 7 parts
                 edits: Beat A [to=56]; Hat A [to=56]; Basse A [to=56]; Accords A [to=56]; Tenue [from=56]
  A4             bars  57-72  (16) 7 parts
  Coda           bars  73-80  ( 8) 3 parts
                 edits: Nappe A2 [to=77]; Nappe fin [from=77]; Cloche coda [to=79]
  total 80 bars

[automation] 'Accroche coupure'  part='Accroche 8va' cc=74 (cutoff) curve=ease-in points=2

[automation] 'Accroche volume'  part='Accroche 8va' cc=7 (volume) curve=linear points=2

[automation] 'Nappe coupure B'  part='Nappe B' cc=74 (cutoff) curve=smooth points=2

[automation] 'Accords coupure C'  part='Accords C F' cc=74 (cutoff) curve=ease-in points=2

[automation] 'Nappe fondu'  part='Nappe fin' cc=7 (volume) curve=smooth points=2

RESULT ok
```

Rendu MIDI : `ronde.mid` (24 pistes de motifs, 80 mesures à 122 bpm, 5 couloirs en contrôleurs).
