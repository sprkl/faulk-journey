# Court-circuit

## Brief et contraintes

Instrumental électronique sombre et chaud, porté par la basse : une boucle de quatre mesures tenue quarante mesures, qui ne change que de timbre ; elle est coupée au milieu d'une mesure ; quatre mesures d'autre chose ; puis la boucle revient avec d'autres accords, et c'est alors seulement qu'une mélodie chante. 116 bpm, **Fa mineur**, 96 mesures (3 min 19).

Form: F6 Boucle avec une interruption

Profil : morzak

Profil de style : **morzak** (rotation morzak → drifting-cycles → aucun ; demandé par le brief).

- **Tempo** : 116 bpm, 4/4, la famille « groove médian » du profil (112–123), lue telle quelle (pas de demi-temps).
- **Tonalité** : Fa mineur (la tonalité maison du profil). Cycle A dans le mode : Fa m7 – Si♭ m (i – iv), deux mesures chacun. Cycle B à couleur empruntée : Fa – Fa m – Ré♭ – Mi♭ (I – i – ♭VI – ♭VII), une mesure chacun.
- **Palette par rôles** (six rôles, sept pistes) :
  - pulsation : batterie analogique (grosse caisse aux quatre temps, clap sur 2 et 4) et charley à contretemps sur sa propre piste ;
  - basse : dent de scie mono filtrée, elle domine ;
  - arpège : carré pincé ; **le clip ne contient que des accords tenus, le device Cascade en fait l'arpège** ;
  - harmonie : nappe sombre, étroite en niveau, hachée par le charley (porte de bruit qui écoute la piste Charley) ;
  - lead 1, « Motif » : sinus, la phrase de la boucle (première partie) ;
  - lead 2, « Voix » : dent de scie filtrée, la mélodie qui se développe (seconde partie).
- **Longueur** : 96 mesures. La carte de F6 (64 mesures : 28 + 4 + 28 + 4) est étirée à 40 + 4 + 48 + 4 pour approcher les 3 min 30 du profil.
- **Forme** : F6. Les deux fiches précédentes sont F5 « Deux rives » et F4 « Girouette » (exclues) ; les cinq dernières : F5, F4, F3, F10, F1. Le profil nomme F3, F6 et la forme à deux sommets ; F3 a servi au dernier passage morzak (le 19), F6 n'a pas servi depuis le 16 : je prends F6, le plateau hypnotique du profil. F0 écartée.

Trois contraintes (deux gestes du profil, une de moi) :

1. **Deux cycles qui alternent par section sur un groove constant** (« Où va le style », 1). Le cycle A tient les quarante premières mesures ; après la rupture, le cycle B tient tout le reste. La batterie, le charley et la figure de basse ne changent pas : la section vient de l'harmonie.
2. **Le cycle reste, le timbre bouge** (geste 8). Dans la première partie, rien n'entre ni ne sort après la mesure 9 : seules les coupures de l'arpège et de la nappe bougent. Quatre couloirs d'automation en tout.
3. **L'arpège n'est jamais écrit** (ma contrainte). Les clips de la piste Arp ne contiennent que des accords d'une ou deux mesures ; l'arpège est ce que Cascade en fait (doubles croches, montant-descendant, deux octaves).

Écarts au profil : la fin s'arrête au milieu d'une phrase (c'est F6) au lieu de la dissolution longue du geste 3, non retenu ; la sortie de douze mesures amincit quand même la mélodie avant la coupure.

## Catalogue d'attributs (profil morzak, adapté)

- Tempo : 116 bpm, doubles croches droites.
- Mode et harmonie : Fa mineur ; cycles de deux et de quatre accords tenus chacun une section entière ; ♭VI et ♭VII de passage ; **la signature : un accord qui retourne sa tierce**, Fa majeur puis Fa mineur, en tête du cycle B, à chaque tour, et repris par la mélodie (La puis La♭).
- Son : peu de couches, sons simples ; une basse mono qui domine ; un arpège comme rôle à part entière ; peu de réverbération dans le grave.
- Rythme : densité modérée, pas de roulement de charley avant le sommet, un seul fill.
- Mélodie : l'arpège cascade ; la « Voix » est énoncée (53–68), étendue au sommet (69–84), amincie à la sortie (85–96).
- Forme : plateau (tout est là en dix secondes), une seule interruption.
- Mix : le grave domine ; le charley tient la bande 3–8 kHz d'un bout à l'autre ; master peu compressé (facteur de crête visé au-dessus de 11 dB).

## Boucle de départ

La basse d'abord (elle porte le genre) : fondamentales, une octave en fin de mesure, une levée chromatique absente : tout est dans le mode.

```pattern notes "Basse A" bars=4 grid=8 octave=1 key="F minor" role=bass
F1 . F1 F1 . F1 . F2 | F1 . F1 F1 . F1 Eb2 C2 | Bb1 . Bb1 Bb1 . Bb1 . Bb2 | Bb1 . Bb1 Bb1 . Db2 C2 Eb2 |
```

Les accords tenus que Cascade arpège : Fa m7 deux mesures, Si♭ m deux mesures ; Fa reste en bas.

```pattern notes "Accords A" bars=4 grid=4 octave=3 key="F minor" role=arp
F3+Ab3+C4+Eb4 - - - | - - - - | F3+Bb3+Db4+F4 - - - | - - - - |
```

La nappe : deux voix serrées, au-dessus de Do 3, sous les leads.

```pattern notes "Nappe A" bars=4 grid=4 octave=3 key="F minor" role=pad
Ab3+C4 - - - | - - - - | Bb3+Db4 - - - | - - - - |
```

Le motif (sinus) : huit mesures, une question puis sa réponse ; un seul sommet (La♭5, mesure 5) ; il finit sur Do, ouvert.

```pattern notes "Motif" bars=8 grid=8 octave=5 key="F minor" role=lead
. . C5 - Eb5 - F5 - | - - - - Eb5 - C5 - | Db5 - - - - - Bb4 - | C5 - - - - - . . | . . C5 - Eb5 - Ab5 - | - - G5 - F5 - Eb5 - | F5 - - - Db5 - Bb4 - | C5 - - - - - . . |
```

La batterie et le charley.

```pattern drums "Beat A" bars=1 grid=16
Kick |x...x...x...x...|
Clap |....x.......x...|
```

```pattern drums "Hat A" bars=1 grid=16
CHat |..x...x...x...x.|
```

## Variations

- **Phrase libre** (gén. 2, rythme et harmonie) : la rupture. Des triolets, seuls, sur Sol♭ maj7 (le ♭II : rien à voir avec la boucle) ; la dernière note, Do, ramène Fa. Sol♭ est hors de Fa mineur : c'est voulu, pas de `key=`.

```pattern notes "Phrase libre" bars=4 grid=12 octave=5 role=melody
F5 Db5 Bb4 Gb4 - - . . . . . . | Gb5 Db5 Bb4 F4 - - . . . . . . | F5 Db5 Bb4 Gb4 Bb4 Db5 F5 - - . . . | Gb5 - - F5 - - C5 - - - - - |
```

- **Fill** (gén. 3, rythme) : le seul fill du morceau, dernier temps de la mesure 44.

```pattern drums "Fill" bars=1 grid=16
Clap |............ooxx|
```

- **Accords B** (gén. 4, harmonie) : le cycle B ; Fa majeur puis Fa mineur : la tierce se retourne (La, puis La♭), Fa reste en bas et en haut. La bécarre est hors de Fa mineur : c'est la signature.

```pattern notes "Accords B" bars=4 grid=4 octave=3 key="F minor" role=arp
F3+A3+C4+F4 - - - | F3+Ab3+C4+F4 - - - | F3+Ab3+Db4+F4 - - - | G3+Bb3+Eb4+G4 - - - |
```

- **Nappe B** (gén. 5, harmonie) : les mêmes accords, deux voix.

```pattern notes "Nappe B" bars=4 grid=4 octave=3 key="F minor" role=pad
A3+C4 - - - | Ab3+C4 - - - | Ab3+Db4 - - - | Bb3+Eb4 - - - |
```

- **Basse B** (gén. 6, harmonie) : la même figure rythmique, sur Fa, Fa, Ré♭, Mi♭ ; La puis La♭ en note de passage disent la tierce.

```pattern notes "Basse B" bars=4 grid=8 octave=1 key="F minor" role=bass
F1 . F1 F1 . A1 . C2 | F1 . F1 F1 . Ab1 . C2 | Db2 . Db2 Db2 . Db2 . Ab1 | Eb2 . Eb2 Eb2 . Eb2 G2 Eb2 |
```

- **Voix A** (gén. 7, mélodie) : la mélodie énoncée. La puis La♭ sur le premier temps des deux premières mesures ; un seul sommet (La♭5, mesure 7).

```pattern notes "Voix A" bars=8 grid=8 octave=4 key="F minor" role=lead
A4 - - - C5 - A4 - | Ab4 - - - C5 - Ab4 - | F4 - Ab4 - Db5 - - - | Eb5 - - Db5 - - Bb4 - | A4 - - - C5 - F5 - | Ab4 - - - C5 - F5 - | Ab5 - - F5 - - Db5 - | Eb5 - - - G4 - Bb4 - |
```

- **Voix B** (gén. 8, mélodie) : étendue au sommet : plus de notes, une octave plus haut par endroits ; un seul sommet (Do6, mesure 7, la septième majeure de Ré♭).

```pattern notes "Voix B" bars=8 grid=8 octave=5 key="F minor" role=lead
A4 C5 F5 - A5 - F5 C5 | Ab4 C5 F5 - Ab5 - F5 C5 | Db5 - F5 Ab5 - - F5 - | G5 - - Eb5 - Bb4 Eb5 - | A5 - - F5 - C5 A4 - | Ab5 - - F5 - C5 Ab4 - | Db5 F5 Ab5 - C6 - Ab5 - | Bb5 - G5 - Eb5 - - - |
```

- **Voix fin** (gén. 9, mélodie) : amincie : le squelette de Voix A, une ou deux notes par mesure.

```pattern notes "Voix fin" bars=8 grid=8 octave=4 key="F minor" role=lead
A4 - - - - - - - | Ab4 - - - - - - - | F4 - - - Db5 - - - | Eb5 - - - - - - - | A4 - - - - - - - | Ab4 - - - - - - - | Ab5 - - - - - - - | Eb5 - - - - - - - |
```

- **Beat B** (gén. 10, rythme) : une grosse caisse de plus, un clap fantôme ; seulement au sommet.

```pattern drums "Beat B" bars=1 grid=16
Kick |x...x...x..xx...|
Clap |....x..o....x...|
```

- **Hat B** (gén. 11, rythme) : doubles croches douces, le contretemps accentué ; seulement au sommet.

```pattern drums "Hat B" bars=1 grid=16
CHat |o.xoo.xoo.xoo.xo|
```

Dispositif structurel (Progresser) : une décision sur le silence : la boucle est coupée au troisième temps de la mesure 40 et rien de la boucle ne sonne pendant quatre mesures.

## Arrangement

Form: F6 Boucle avec une interruption

```arrangement tempo=116
section Boucle-entree 1-8   : Accords A, Nappe A, Basse A, Beat A [from=5], Hat A [from=5]
section Boucle        9-40  : Accords A [to=40.3], Nappe A [to=40.3], Basse A [to=40.3], Beat A [to=40.3], Hat A [to=40.3], Motif [to=40.3]
section Rupture       41-44 : Phrase libre, Fill [from=44]
section Retour        45-52 : Accords B, Nappe B, Basse B, Beat A, Hat A
section Chant         53-68 : Accords B, Nappe B, Basse B, Beat A [mute=68], Hat A, Voix A
section Sommet        69-84 : Accords B, Nappe B, Basse B, Beat B, Hat B, Voix B
section Sortie        85-96 : Accords B [to=96.3], Nappe B [to=96.3], Basse B [to=96.3], Beat A [to=96.3], Hat A [to=96.3], Voix fin [to=96.3]
```

Cycles par section : Boucle (1–40) : cycle A, Fa m7 – Si♭ m. Rupture (41–44) : Sol♭ maj7 arpégé à nu. Retour, Chant, Sommet, Sortie (45–96) : cycle B, Fa – Fa m – Ré♭ – Mi♭. Deux cycles différents, plus la rupture.

Coutures :

- 4 → 5 : la batterie et le charley entrent (fenêtre `from=5`) : tout est là en dix secondes.
- 40.3 : **tout est coupé au troisième temps** (fenêtres `to=40.3`) ; les queues d'écho et de réverbération tiennent la demi-mesure.
- 44 → 45 : le fill de clap sur le dernier temps (anticipation), puis la boucle revient d'un bloc sur Fa majeur.
- 68 → 69 : une mesure sans grosse caisse ni clap (`mute=68`), le charley continue ; la Voix B part sur le premier temps.
- 84 → 85 : Beat A et Hat A reviennent, la Voix s'amincit.
- 96.3 : coupure au milieu de la phrase, sur Mi♭ (♭VII) : pas de résolution.

Événements uniques :

1. 40.3 : la boucle coupée au milieu de la mesure (**structurel**).
2. 41.1–44.4 : la phrase libre en triolets, seule (le seul passage ternaire, le seul Sol♭).
3. 44.4 : le fill de clap (le seul).
4. 45.1 : première fois que Fa est majeur.
5. 68 : la mesure sans batterie.
6. 96.3 : l'arrêt au milieu de la phrase (**structurel**).

## Automation

L'arpège s'ouvre lentement pendant toute la première partie (lente puis rapide : la fin de l'ouverture annonce la coupure), repart fermé au retour et s'ouvre jusqu'au sommet, puis se referme à la sortie.

```automation "Arp coupure 1" part="Accords A" param=cutoff curve=ease-in
1.1 40, 40.2 92
```

```automation "Arp coupure 2" part="Accords B" param=cutoff curve=ease-in
45.1 52, 69.1 84 linear, 84.4 104 smooth, 96.2 64
```

La nappe respire en deux vagues lentes (en S : on ne doit pas entendre le début ni la fin du mouvement).

```automation "Nappe coupure" part="Nappe A" param=cutoff curve=smooth
1.1 48, 17.1 72, 33.1 52, 40.2 80
```

La Voix s'ouvre de deux octaves sur vingt-quatre mesures (lente puis rapide), et son volume baisse de 2 dB sur les mêmes mesures pour que l'ouverture ne la sorte pas du mix (règle du lead ; 3 dB au premier rendu, ramenés à 2 après mesure) ; à la sortie le filtre se referme (en S), le volume reste bas.

```automation "Voix coupure" part="Voix A" param=cutoff curve=ease-in
53.1 60, 61.1 60, 84.4 96 smooth, 96.2 70
```

```automation "Voix volume" part="Voix A" param=volume curve=linear
53.1 100, 61.1 100, 84.4 92
```

Dans Faulk : Arp coupure = Filter › Fréquence de coupure de la piste Arp (300 Hz → 2 kHz ; 500 Hz → 1,5 kHz → 4 kHz → 800 Hz) ; Nappe coupure = Filter de la piste Nappe (400 Hz → 1,2 kHz → 500 Hz → 1,5 kHz) ; Voix coupure = Filter de la piste Voix (700 Hz → 700 Hz → 2,8 kHz → 1 kHz) ; Voix volume = Mixeur › Volume de la piste Voix (−3 dB → −3 dB → −5 dB ; −10 → −10 → −13 au premier rendu).

## Notes de finition

**Sons** (les notes existent, les sons suivent) :

- **Batterie** : Drums tel quel.
- **Charley** : Drums, sa propre piste ; c'est l'élément qui tient 3–8 kHz d'un bout à l'autre (sauf la rupture).
- **Basse** : Oscillator dent de scie, attaque 5 ms, relâchement 120 ms ; Filter passe-bas 700 Hz, résonance 20 %.
- **Arp** : **Cascade** (ordre montant-descendant, division 1/16, droit, 2 octaves, durée 50 %, vélocité jouée, redémarrage à chaque nouvel accord) avant l'Oscillator carré (déclin 150 ms, maintien 20 %, relâchement 100 ms) ; Filter passe-bas automatisé ; Echo 1/8., retour 30 %, mélange 15 % ; Reverb taille 40 %, amortissement 50 %, mélange 15 %.
- **Nappe** : Oscillator dent de scie, attaque 300 ms, relâchement 800 ms ; Filter passe-bas automatisé ; Bloom Ensemble, phase stéréo 150, mélange 45 %, tonalité 300 Hz ; Reverb taille 75 %, amortissement 70 %, mélange 40 % ; **Sluice dont la source est la piste Charley** (seuil d'ouverture −45 dB, fermeture −50 dB, profondeur 9 dB, attaque 1 ms, maintien 50 ms, relâchement 150 ms), placé après le Filter et avant Bloom et Reverb : la nappe est 9 dB plus bas hors des coups de charley (lu sur la piste en solo : −30 dBFS sous le charley, −37 entre deux), un lit qui respire et pas un hachoir.
- **Motif** : Oscillator sinus, attaque 20 ms, relâchement 400 ms ; Echo 1/4, retour 25 %, mélange 20 % ; Reverb taille 40 %, amortissement 50 %, mélange 20 %, pré-délai 40 ms (la pièce du plan médian).
- **Voix** : Oscillator dent de scie, attaque 20 ms, relâchement 300 ms ; Filter passe-bas automatisé (700 Hz → 2,8 kHz) ; Echo 1/4, retour 25 %, mélange 20 % ; la même Reverb que le Motif.
- **Master** : Compressor −12 dB ratio 2, compensation 9 dB ; Ceiling −0,3 dB. Rendu final : crête −0,3 dBFS, −16,2 dBFS RMS, facteur de crête 15,9 dB.

Mix: Batterie: −10 dB, C, avant (pas de Reverb), pas de largeur, grosse caisse 40–100 Hz, clap 1–5 kHz
Mix: Charley: −18 dB, L25 (sa propre piste Drums), milieu (sec, discret), pas de largeur, au-dessus de 5 kHz
Mix: Basse: −6 dB, C, avant (pas de Reverb, Filter passe-bas 700 Hz), pas de largeur, 40–250 Hz
Mix: Arp: −13 dB, R35, milieu (Reverb taille 0,4 amortissement 0,5 mélange 0,15, Echo 1/8. retour 0,3 mélange 0,15, Filter passe-bas automatisé 300 Hz–4 kHz), pas de largeur, 300 Hz–4 kHz
Mix: Nappe: −13 dB, C, arrière (Reverb taille 0,75 amortissement 0,7 mélange 0,4, Filter passe-bas automatisé 400 Hz–1,5 kHz), Bloom ensemble phase stéréo 150 mélange 0,45 tonalité 300 Hz, 200 Hz–1,5 kHz
Mix: Motif (lead de la première partie): −6,5 dB (−8 dB au premier rendu, relevé après le lead check), C, bord avant de la pièce (Reverb taille 0,4 amortissement 0,5 mélange 0,2 pré-délai 0,04, Echo 1/4 retour 0,25 mélange 0,2, pas de Filter : sinus), pas de largeur, 450 Hz–900 Hz
Mix: Voix (lead de la seconde partie): −3 dB (−10 dB au premier rendu, −4 au deuxième), C, bord avant de la pièce (même Reverb, Echo 1/4 retour 0,25 mélange 0,2, Filter passe-bas), pas de largeur, 350 Hz–3 kHz ; coupure 700 Hz à 2,8 kHz mesures 61–84, volume −2 dB sur les mêmes mesures (−3 dB → −5 dB)
Mono check: 1, 3 et 4 à la lecture (grosse caisse, basse et leads au centre ; le seul Bloom est sur la nappe, tonalité 300 Hz, mélange 0,45 ; l'arpège à R35 garde sa Reverb à 0,15) ; 2 sans objet (pas de paire en miroir) ; le reste à l'oreille
Lead check: Motif, mesures 9–40 là où il sonne, −16,1 dBFS RMS, −17,5 sans le lead : 1,4 dB (sur les mesures entières : −16,2 et −17,5, soit 1,2 dB). Premier rendu, Motif à −8 dB : 1,05 dB (0,9 sur les mesures entières), au bord de « enterré », donc relevé de 1,5 dB.
Lead check: Voix, mesures 81–84 (fin de l'ouverture), −15,7 dBFS RMS, −16,9 sans le lead : 1,2 dB ; mesures 69–84 (sommet entier) : −15,2 et −16,9, soit 1,7 dB ; mesures 53–68 (filtre fermé) : −15,1 et −17,4, soit 2,3 dB. Premier rendu (Voix −10 dB, compensation 3 dB) : 0,6 dB filtre fermé, 0,2 dB en fin d'ouverture : enterrée. Deuxième rendu (−4 dB, compensation 2 dB) : 1,9 dB et 1,0 dB.

**Niveaux, ce que les trois rendus disent** : la Voix passe par un passe-bas à 700 Hz : à fader égal elle se lit plus bas que le Motif sinus ; elle finit 3 dB au-dessus du fader de la basse, hors de la fourchette des faders, parce que la mesure sur le rendu le demande. Et l'ouverture de deux octaves n'ajoute presque rien au RMS de ce lead (ses fondamentales, 350 Hz à 1 kHz, passent déjà le filtre fermé) : avec la baisse de volume qui la compense, l'écart mesuré **baisse** pendant l'ouverture (2,3 dB filtre fermé, 1,2 dB en fin d'ouverture) alors que le son s'éclaircit. À trancher à l'oreille : le RMS large bande ne voit pas la brillance.

**Humaniser** : les coupures bougent déjà ; à l'oreille, la graine et l'accent de Cascade, un peu de dérive sur le déclin de l'arpège.

**Laissé à l'oreille** : la profondeur de la porte sur la nappe, la durée des notes de Cascade, l'équilibre basse / grosse caisse, la longueur de la queue pendant la rupture.

**Version suivante** : Cascade en triolets au sommet ; un balancement du charley et de la basse ensemble ; la rupture en vrai tempo libre.

## Check

```

[notes] 'Basse A'  bars=4 grid=8 notes=22
  OK     all 22 notes are in F minor
  INFO   contour: range 17 semitones, highest note occurs 1x, steps 2 / leaps 8, up 40 / down 30 semitones, 5.5 notes per bar

[notes] 'Accords A'  bars=4 grid=4 notes=8
  OK     all 8 notes are in F minor

[notes] 'Nappe A'  bars=4 grid=4 notes=4
  OK     all 4 notes are in F minor

[notes] 'Motif'  bars=8 grid=8 notes=18
  OK     all 18 notes are in F minor
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 9 / leaps 7, up 20 / down 20 semitones, 2.2 notes per bar

[drums] 'Beat A'  bars=1 grid=16 notes=6

[drums] 'Hat A'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Phrase libre'  bars=4 grid=12 notes=18
  INFO   contour: range 13 semitones, highest note occurs 2x, steps 2 / leaps 15, up 36 / down 41 semitones, 4.5 notes per bar
  INFO   contour: the highest note repeats; a memorable line usually has a single peak

[drums] 'Fill'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Accords B'  bars=4 grid=4 notes=16
  WARN   1 note(s) outside F minor: A3 at bar 1 beat 1. Keep each one only if it is a decision.

[notes] 'Nappe B'  bars=4 grid=4 notes=8
  WARN   1 note(s) outside F minor: A3 at bar 1 beat 1. Keep each one only if it is a decision.

[notes] 'Basse B'  bars=4 grid=8 notes=21
  WARN   1 note(s) outside F minor: A1 at bar 1 beat 3.5. Keep each one only if it is a decision.
  INFO   contour: range 14 semitones, highest note occurs 1x, steps 1 / leaps 9, up 26 / down 16 semitones, 5.2 notes per bar

[notes] 'Voix A'  bars=8 grid=8 notes=24
  WARN   3 note(s) outside F minor: A4 at bar 1 beat 1, A4 at bar 1 beat 4, A4 at bar 5 beat 1. Keep each one only if it is a decision.
  INFO   contour: range 15 semitones, highest note occurs 1x, steps 5 / leaps 18, up 42 / down 41 semitones, 3.0 notes per bar

[notes] 'Voix B'  bars=8 grid=8 notes=36
  WARN   4 note(s) outside F minor: A4 at bar 1 beat 1, A5 at bar 1 beat 3, A5 at bar 5 beat 1, A4 at bar 5 beat 4. Keep each one only if it is a decision.
  INFO   contour: range 16 semitones, highest note occurs 1x, steps 3 / leaps 32, up 74 / down 68 semitones, 4.5 notes per bar

[notes] 'Voix fin'  bars=8 grid=8 notes=9
  WARN   2 note(s) outside F minor: A4 at bar 1 beat 1, A4 at bar 5 beat 1. Keep each one only if it is a decision.
  INFO   contour: range 15 semitones, highest note occurs 1x, steps 3 / leaps 5, up 22 / down 16 semitones, 1.1 notes per bar

[drums] 'Beat B'  bars=1 grid=16 notes=8

[drums] 'Hat B'  bars=1 grid=16 notes=12
  NOTE   no kick in this pattern: fine if another part carries the pulse

[arrangement] tempo=116
  Boucle-entree  bars   1-8   ( 8) 5 parts
                 edits: Beat A [from=5]; Hat A [from=5]
  Boucle         bars   9-40  (32) 6 parts
                 edits: Accords A [to=40.3]; Nappe A [to=40.3]; Basse A [to=40.3]; Beat A [to=40.3]; Hat A [to=40.3]; Motif [to=40.3]
  Rupture        bars  41-44  ( 4) 2 parts
                 edits: Fill [from=44]
  Retour         bars  45-52  ( 8) 5 parts
  Chant          bars  53-68  (16) 6 parts
                 edits: Beat A [mute=68]
  Sommet         bars  69-84  (16) 6 parts
  Sortie         bars  85-96  (12) 6 parts
                 edits: Accords B [to=96.3]; Nappe B [to=96.3]; Basse B [to=96.3]; Beat A [to=96.3]; Hat A [to=96.3]; Voix fin [to=96.3]
  total 96 bars

[automation] 'Arp coupure 1'  part='Accords A' cc=74 (cutoff) curve=ease-in points=2

[automation] 'Arp coupure 2'  part='Accords B' cc=74 (cutoff) curve=ease-in points=4

[automation] 'Nappe coupure'  part='Nappe A' cc=74 (cutoff) curve=smooth points=4

[automation] 'Voix coupure'  part='Voix A' cc=74 (cutoff) curve=ease-in points=4

[automation] 'Voix volume'  part='Voix A' cc=7 (volume) curve=linear points=3

RESULT ok
```
