# Haute tension

Instrumental électronique sombre, rapide et tendu, 152 bpm (l'exception rapide du profil, lue comme un tempo plein), La mineur avec le V majeur du mineur harmonique, 96 mesures (environ 2 min 32), forme en arc : montée en deux temps, section B unique au milieu, bascule de tierce au moment le plus dense (mesure 66, 69 %), **sortie de 16 mesures par retrait**. Profil de style demandé : **morzak**. Les deux passages précédents ont pris le mi-groove dorien (118 bpm, Fa dorien) et la famille lente éolienne (84 bpm, Ré éolien) ; celui-ci prend la famille rapide et le mineur harmonique, dans une humeur de course nocturne, pas de brume. Fiche dimensionnée pour être construite dans Faulk **à l'interface seulement** : cinq rôles, dix motifs, 89 notes, un cycle de **deux accords** tenu tout le morceau.

## Brief et contraintes

- **Profil de style** : morzak (`references/styles/morzak.md`). Gardé : la famille rapide (≈ 152), le mineur modal avec le V majeur « pour une attraction plus sombre vers i », le cycle court (deux accords, une mesure chacun), la basse qui porte, peu de couches (cinq rôles), peu de réverbération sur le grave, doubles-croches droites, pas de fill, la forme en arc, un master dynamique. Plié : la durée (2 min 32 au lieu de 3 min 30 à 7) parce que chaque note se pose à la main ; la section B sur ♭VI–♭VII (mouvement 4) est là mais ne compte pas comme contrainte. Lâché : le swing (mouvement 5) : tout est droit cette fois ; le mouvement 2 (la bascule comme événement unique) est fait quand même par la signature.
- **Tempo** : 152 bpm, lu comme un tempo plein (kick sur 1 et 3, clap sur 2 et 4 : la pulsation court).
- **Tonalité** : La mineur harmonique sur le cycle (A B C D E F G♯), La éolien (Sol naturel) dans la section B ; cycle **i – V = Am – E**, une mesure chacun, deux mesures par tour, tenu tout le morceau sauf la section B.
- **Palette par rôle** :
  - pulsation : Drums, kick sur 1, le « et » de 2 et 3 (relance sur le « et » de 4 une mesure sur deux), clap sur 2 et 4 (« Beat A ») ;
  - texture aiguë : second Drums, charley fermé seul, en contretemps de croches, à −18 dB, **de la première à la dernière mesure** (« Hats ») ;
  - basse : Oscillator en dents de scie, mono, Filter passe-bas vers 350 Hz, pas de Reverb (« Bass A », « Bass B ») ;
  - harmonie : Oscillator en triangle, accords tenus une mesure, Reverb courte (« Chords A », « Chords flip », « Chords B ») ;
  - lead : Oscillator en carré, Echo à la croche, discret (« Lead A », « Lead B »).
  - master : Compressor léger (ratio 2:1), master à −3 dB.
- **Longueur cible** : 96 mesures : Intro 8 / Build 16 / Groove 16 / Break 8 / Peak 32 / Exit 16.
- **Contraintes arbitraires** (deux du profil, une à moi) :
  1. (mouvement 1) **un élément à 3–8 kHz tout du long** : le charley fermé, contretemps de croches, de la mesure 1 à la mesure 96 sans jamais sortir, à −18 dB ;
  2. (mouvement 3) **pic à 55–70 % puis sortie de 16 mesures** qui retire les couches dans l'ordre inverse de leur arrivée (lead, clap, kick, basse ; les accords et le charley vont au bout) ;
  3. (à moi) **deux accords seulement**, i et V, pendant tout le morceau ; ♭VI et ♭VII n'ont droit qu'à la section B, une fois.
- **Signature** : le même accord entendu majeur puis mineur : E (V) devient Em (v, Sol naturel) une seule fois, mesures 65–68 (la bascule est à la mesure 66), au cœur du moment le plus dense, puis le cycle revient au V majeur à 69.
- **Hypothèses** : Drums a cinq sons (kick, caisse claire, clap, charley fermé, charley ouvert) ; la longueur d'une note écrite au clavier est le pas d'aimantation (les accords tenus une mesure s'écrivent avec Snap « Bar ») ; les tenues de « Bass B » sur deux temps seront peut-être réduites à une noire ; aucun dither à l'export.

## Catalogue d'attributs (profil morzak, adapté)

- **Son** : cinq rôles, synthés simples, basse mono, grave sec, Reverb seulement sur les accords, Echo court sur le lead.
- **Harmonie** : mineur, cycle de deux accords i – V (V majeur, mineur harmonique) ; ♭VI et ♭VII une fois, dans la section B ; une bascule de tierce.
- **Mélodie** : motif court descendant, un seul sommet, au service du cycle.
- **Rythme** : tempo plein à 152, doubles-croches droites, kick syncopé, clap sur 2 et 4, charley en contretemps ; densité modérée (environ 5 attaques percussives par seconde en groove) ; pas de fill.
- **Forme** : arc, section B unique au milieu, pic à 69 %, sortie de 16 mesures par retrait.
- **Tempo** : 152.
- **Mix** : basse et sub dominants, charley bas mais continu, présence et air sous 5 %, crête 11–16 dB au-dessus du RMS.

## Boucle de départ

La pulsation d'abord, puis la basse (elle définit le style), puis les accords, puis le charley, puis le lead.

```pattern drums "Beat A" bars=2 grid=16
Kick  |x.....x.x.......|x.....x.x.....x.|
Clap  |....x.......x...|....x.......x...|
```

Pourquoi : kick sur 1, le « et » de 2 et le 3 (une relance qui pousse vers le 3), clap sur 2 et 4 ; la seconde mesure ajoute un kick sur le « et » de 4 pour que les deux mesures ne soient pas jumelles : onze attaques sur deux mesures, le grave a la place.

```pattern notes "Bass A" bars=2 grid=8 octave=1 key="A harmonic minor" role=bass
A . A . A2 . A . | E . E . E2 . G# . |
```

Pourquoi : la fondamentale en croches sur 1 et 2, l'octave sur 3, et sur le temps 4 la fondamentale (mesure 1) puis la sensible Sol♯ (mesure 2) qui tire vers La : la basse dit le cycle et son V majeur seule.

```pattern notes "Chords A" bars=2 grid=4 octave=3 key="A harmonic minor" role=chords
A3+C4+E4 - - - | G#3+B3+E4 - - - |
```

Pourquoi : Am puis E en premier renversement (Sol♯ en bas), tenus une mesure chacun, voisinage serré : deux voix bougent d'un demi-ton, le Mi reste.

```pattern drums "Hats" bars=1 grid=8
CHat  |.o.o.o.o|
```

Pourquoi : le charley fermé en contretemps de croches, en fantôme (vélocité 60), seul rôle présent de la première à la dernière mesure (contrainte 1) : l'élément à 3–8 kHz qui ne sort jamais.

```pattern notes "Lead A" bars=4 grid=8 octave=5 key="A harmonic minor" role=melody
. . E - . C - . | . . D - . B4 - . | . . C - . A4 - . | . . G#4 - - - . . |
```

Pourquoi : un seul sommet, Mi 5, première note ; descente par paires (Mi–Do sur Am, Ré–Si sur E, Do–La sur Am) jusqu'à la sensible Sol♯ tenue sur E, qui appelle le La du tour suivant ; jamais sur le temps 1 : le motif entre sur le temps 2.

## Variations

Une seule chose change par génération, jamais de retour en arrière.

```pattern drums "Beat A kick" bars=2 grid=16
Kick  |x.....x.x.......|x.....x.x.....x.|
```

- Gen 1 (forme) : « Beat A » sans clap, pour la montée (mesures 17–24) et la sortie (81–88) : la pulsation arrive avant le backbeat, et le backbeat part avant elle.

```pattern notes "Chords flip" bars=2 grid=4 octave=3 key="A minor" role=chords
A3+C4+E4 - - - | G3+B3+E4 - - - |
```

- Gen 2 (harmonie), la signature : « Chords A » dont le E majeur devient Em (Sol♯ → Sol), entendu une fois, mesures 65–68 (la bascule est à la mesure 66, à 69 % du morceau). Deux tours du cycle en mineur, puis retour au V majeur.

```pattern notes "Chords B" bars=4 grid=4 octave=3 key="A minor" role=chords
F3+A3+C4 - - - | G3+B3+D4 - - - | F3+A3+C4 - - - | G3+B3+D4 - - - |
```

- Gen 3 (harmonie) : la section B : ♭VI – ♭VII (F – G) une mesure chacun, Sol naturel (La éolien) ; le cycle i – V s'arrête, l'harmonie respire, une seule fois, mesures 41–48.

```pattern notes "Bass B" bars=4 grid=4 octave=1 key="A minor" role=bass
F . F . | F . F F2 | G . G . | G . G G2 |
```

- Gen 4 (basse) : sous la section B, la basse passe des croches aux noires, et l'octave n'arrive qu'au dernier temps d'une mesure sur deux : moins de mouvement, plus de poids.

```pattern notes "Lead B" bars=4 grid=8 octave=5 key="A harmonic minor" role=melody
. . E - . C - . | . . D - . B4 - . | . . C - . A4 - . | . . B4 - - - . . |
```

- Gen 5 (mélodie) : « Lead A » dont la dernière note ne descend plus sur la sensible : elle s'arrête sur Si (quinte de E), sans résoudre ; pour le pic.

```pattern drums "Beat A open" bars=2 grid=16
Kick  |x.....x.x.......|x.....x.x.....x.|
Clap  |....x.......x...|....x.......x...|
OHat  |................|..............x.|
```

- Gen 6 (rythme) : « Beat A » avec un charley ouvert sur le « et » de 4 de la seconde mesure, pour les huit dernières mesures du pic (73–80) : l'unique ajout de batterie du morceau.

Dix motifs : assez pour six sections avec une combinaison différente chacune.

## Arrangement

```arrangement tempo=152
section Intro   1-8   : Hats, Chords A
section Build   9-24  : Hats, Chords A, Bass A, Beat A kick [from=17]
section Groove  25-40 : Beat A [mute=40.3], Hats, Bass A, Chords A, Lead A [from=33]
section Break   41-48 : Hats, Chords B, Bass B, Lead A
section Peak    49-80 : Beat A [from=49.2 to=73], Beat A open [from=73], Hats, Bass A, Chords A [to=65], Chords flip [from=65 to=69], Chords A [from=69], Lead B [from=57]
section Exit    81-96 : Beat A kick [to=89], Hats, Bass A [to=93], Chords A
```

Coutures et événements uniques, par mesure :

- **1–8** : charley et accords seuls : le cycle i – V est la première chose entendue, avec l'élément aigu qui ne sortira plus.
- **9.1** : la basse entre sur la mesure ; **17.1** : le kick seul (« Beat A kick ») : la pulsation arrive en deux temps, couture par report.
- **25.1** : le clap entre (« Beat A » complet) ; **33.2** : le lead entre sur le temps 2.
- **40.3** (événement unique 1) : la batterie se tait sur les temps 3 et 4 de la dernière mesure du groove : l'hésitation avant la section B.
- **41–48** : la section B, le seul moment hors du cycle i – V ; pas de kick ni de clap : l'harmonie exposée, la basse en noires.
- **49.1** : la batterie rentre sur le temps 2 (`from=49.2`, événement unique 2 : le temps 1 vide), la basse et les accords sur le temps 1 : anticipation.
- **57.2** : « Lead B » entre : le moment le plus dense commence (59 %).
- **66** (événement unique 3, la signature) : E majeur devient Em, Sol naturel dans les accords, une seule fois (65–68), au-dessus d'une basse qui joue encore Sol♯ sur le temps 4 : le frottement est voulu, deux tours ; retour au V majeur à 69.
- **74.4.3** (événement unique 4) : le charley ouvert, huit fois (73–80), le seul ajout de batterie.
- **81–96** : sortie par retrait dans l'ordre inverse de l'arrivée : le lead part à 81, le clap à 81 (« Beat A kick »), le kick à 89, la basse à 93 ; les accords et le charley vont jusqu'à 96 : fin par coupe à la barre, queue de Reverb des accords.

## Notes de finition

- **Sons** : Drums par défaut, kick un peu plus court (400 ms, le tempo est rapide) ; « Hats » sur sa propre tranche à −18 dB ; basse en dents de scie, Filter passe-bas 350 Hz, pas de Reverb ; accords en triangle, Reverb par défaut, tranche à −6 dB ; lead en carré, Echo à la croche, mix 25 %, tranche à −6 dB ; Compressor 2:1 sur le master, master à −3 dB.
- **Humanisation** : aucune : tout est droit, c'est le profil ; le charley en fantôme fait le relief.
- **Laissé à l'oreille** : le niveau du charley (assez bas pour ne pas sortir, assez présent pour être senti) ; si le frottement Sol / Sol♯ des mesures 65–68 doit être gardé ou si la basse doit passer au Sol naturel ; le mix de l'Echo du lead sur le pic.
- **Version suivante** : une seconde basse à l'octave sur 57–80 ; un filtre qui s'ouvre sur la basse de 9 à 24 ; une section B de 16 mesures.

## Check

(sortie de `sheet_tool.py check`, voir `check.txt` à côté de la fiche)
