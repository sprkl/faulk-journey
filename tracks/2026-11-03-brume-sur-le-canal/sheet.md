# Brume sur le canal

Instrumental électronique sombre, lent et lourd, 84 bpm (famille lente du profil, lue comme un tempo plein, pas comme la moitié de 168), Ré éolien, 64 mesures (environ 3 min 03), forme en arc : montée, section B unique au milieu, moment le plus dense à 41 (64 %), sortie de 8 mesures. Profil de style demandé : **morzak**. Fiche dimensionnée pour être construite dans Faulk **à l'interface seulement** : cinq rôles, neuf motifs, 85 notes, cycle de quatre accords tenu tout le morceau. Le passage du matin (« Veille sous la dalle », 118 bpm, Fa dorien, mi-groove) a pris l'autre famille de tempo et la couleur dorienne ; celui-ci prend la famille lente et la couleur éolienne, pour que le Journal ne se répète pas.

## Brief et contraintes

- **Profil de style** : morzak (`references/styles/morzak.md`). Gardé : la famille de tempo lente (70–90), le mineur modal, le cycle court (quatre accords, une mesure chacun), la couleur éolienne (v mineur, puis ♭VI et ♭VII de passage), le V majeur de mineur harmonique entendu une fois comme bascule de tierce, la basse qui porte, peu de couches, peu de réverbération sur le grave, la forme en arc, un master dynamique. Plié : la durée (3 min 03 au lieu de 3 min 30 à 7) parce que chaque note se pose à la main ; le pic à 64 % (le profil mesure 70–95 %). Lâché : les mouvements 1 (élément 3–8 kHz continu : il y est quand même, par le charley, mais sans compter comme contrainte), 2 et 3.
- **Tempo** : 84 bpm. Lecture choisie : tempo plein (le kick sur 1, la caisse claire sur 3, en demi-temps).
- **Tonalité** : Ré éolien (D E F G A B♭ C) ; cycle i – v – ♭VI – ♭VII = Dm – Am – B♭ – C, une mesure chacun, quatre mesures par tour, tenu tout le morceau sauf la section B.
- **Palette par rôle** :
  - pulsation : Drums, kick lourd sur 1 avec une relance syncopée, caisse claire sur 3 seulement (« Beat A ») ;
  - texture aiguë : second Drums, charley fermé seul, sur les temps et sur des contretemps **swingués** (« Hats swing ») ;
  - basse : Oscillator en dents de scie, mono, Filter passe-bas vers 300 Hz, pas de Reverb (« Bass A », « Bass B ») ;
  - harmonie : Oscillator en triangle, accords tenus une mesure, Reverb courte (« Chords A », « Chords flip », « Chords B ») ;
  - lead : Oscillator en carré, Echo à la noire, discret (« Lead A », « Lead B »).
  - master : Compressor léger (ratio 2:1), master à −3 dB.
- **Longueur cible** : 64 mesures : Intro 8 / Build 8 / Groove 16 / Break 8 / Peak 16 / Exit 8.
- **Contraintes arbitraires** (deux du profil, une à moi) :
  1. (mouvement 4) **une section B de 8 mesures sur ♭VI** (B♭ majeur, puis B♭ avec la sixte) entendue une seule fois, mesures 33–40, pour casser le cycle ;
  2. (mouvement 5) **une seule partie swingue** : les contretemps du charley tombent à 0,625 du temps (le cinquième trente-deuxième), tout le reste est droit ;
  3. (à moi) le lead n'a que **quatre hauteurs**, D F G A, et **ne joue jamais sur le temps 1**.
- **Signature** : le même accord entendu mineur puis majeur : Am (v) devient A majeur (V de Ré mineur harmonique, Do♯) une seule fois, mesure 42, au cœur du moment le plus dense, puis le cycle revient en mineur à la mesure 46.
- **Hypothèses** : Drums a cinq sons (kick, caisse claire, clap, charley fermé, charley ouvert) ; Faulk n'a pas de swing : le swing est écrit note par note sur une grille de trente-deuxièmes ; les notes tenues deux mesures de « Chords B » et de « Bass B » seront peut-être réattaquées chaque mesure si l'interface ne permet pas d'allonger une note au clavier ; aucun dither à l'export.

## Catalogue d'attributs (profil morzak, adapté)

- **Son** : cinq rôles, synthés simples, basse mono, grave sec, Reverb seulement sur les accords.
- **Harmonie** : mineur éolien, quatre accords de passage, un V majeur une fois (bascule de tierce).
- **Mélodie** : motif court, quatre hauteurs, un seul sommet, au service du cycle.
- **Rythme** : demi-temps (kick 1, caisse claire 3) ; doubles-croches droites partout sauf le charley qui swingue ; densité basse (environ 2,5 attaques percussives par seconde en groove) ; pas de fill.
- **Forme** : arc, section B unique au milieu, pic à 64 %, sortie courte par retrait.
- **Tempo** : 84.
- **Mix** : basse et sub dominants, présence et air sous 5 %, crête 11–16 dB au-dessus du RMS.

## Boucle de départ

La pulsation d'abord, puis la basse (elle définit le style), puis les accords, puis le charley swingué, puis le lead.

```pattern drums "Beat A" bars=2 grid=16
Kick  |x.........x.....|x.....x.........|
Snare |........x.......|........x.......|
```

Pourquoi : demi-temps, kick sur 1, une relance sur le « a » de 3 (mesure 1) puis sur le « a » de 2 (mesure 2) pour que les deux mesures ne soient pas jumelles, caisse claire sur 3 seulement : six attaques sur deux mesures, le grave a la place.

```pattern notes "Bass A" bars=4 grid=8 octave=2 key="D minor" role=bass
D . D . D . F . | A1 . A1 . A1 . C . | Bb1 . Bb1 . Bb1 . D . | C . C . C . G1 . |
```

Pourquoi : la fondamentale en croches sur 1, 2 et 3, un trou sur les « et », et une note de l'accord sur le temps 4 qui mène au suivant (tierce F vers Am, tierce C vers B♭, tierce D vers C, quinte G vers Dm) : la basse dit le cycle seule.

```pattern notes "Chords A" bars=4 grid=4 octave=3 key="D minor" role=chords
D3+F3+A3 - - - | C3+E3+A3 - - - | D3+F3+Bb3 - - - | C3+E3+G3 - - - |
```

Pourquoi : Dm, Am (en premier renversement, Do en bas), B♭ (deuxième renversement), C, tenus une mesure chacun, voisinage serré : les trois voix bougent d'un ton au plus.

```pattern drums "Hats swing" bars=1 grid=32
CHat  |x....o..x....o..x....o..x....o..|
```

Pourquoi : le charley sur chaque temps, et un fantôme sur le contretemps **à 0,625 du temps** (contrainte 2), seul élément qui ne soit pas sur la grille des doubles-croches : c'est le balancement du profil, écrit, sur une seule partie.

```pattern notes "Lead A" bars=4 grid=8 octave=4 key="D minor" role=melody
. . A - G - F - | . . . . D - - - | . . G - F - G - | . . F - D - . . |
```

Pourquoi : quatre hauteurs (contrainte 3), jamais sur le temps 1 : le motif entre sur le temps 2 ; un seul sommet, La 4, première note ; descente par degrés vers Ré (réponse de la mesure 2, tenue), puis une seconde phrase qui tourne autour de Sol et retombe sur Ré : appel, réponse.

## Variations

Une seule chose change par génération, jamais de retour en arrière.

```pattern drums "Beat A kick" bars=2 grid=16
Kick  |x.........x.....|x.....x.........|
```

- Gen 1 (forme) : « Beat A » sans caisse claire, pour la montée (mesures 13–16) : la pulsation arrive avant le backbeat.

```pattern notes "Chords flip" bars=4 grid=4 octave=3
D3+F3+A3 - - - | C#3+E3+A3 - - - | D3+F3+Bb3 - - - | C3+E3+G3 - - - |
```

- Gen 2 (harmonie), la signature : « Chords A » dont le Am devient A majeur (Do → Do♯), entendu une fois, mesures 41–44 (la bascule est à la mesure 42). Le Do♯ n'est pas dans Ré éolien : c'est le but (pas de `key=` sur ce motif ; c'est le V de mineur harmonique que le profil décrit).

```pattern notes "Chords B" bars=4 grid=4 octave=3 key="D minor" role=chords
Bb2+D3+F3 - - - | - - - - | Bb2+D3+G3 - - - | - - - - |
```

- Gen 3 (harmonie) : la section B (contrainte 1) : B♭ majeur tenu deux mesures, puis B♭ avec la sixte (Sol à la place de Fa : B♭6, ou Gm/B♭) deux mesures ; le cycle s'arrête, l'harmonie respire.

```pattern notes "Bass B" bars=2 grid=4 octave=2 key="D minor" role=bass
Bb1 - - - | Bb1 - - F |
```

- Gen 4 (basse) : sous la section B, la basse tient B♭ et ne bouge qu'au dernier temps (Fa, quinte) : du mouvement en croches au tenu.

```pattern notes "Lead B" bars=4 grid=8 octave=4 key="D minor" role=melody
. . A - G - F - | . . . . D - - - | . . G - F - G - | . . F - G - - - |
```

- Gen 5 (mélodie) : « Lead A » dont la réponse ne retombe plus sur Ré : elle remonte et s'arrête sur Sol (quinte de l'accord C), sans résoudre ; pour le pic.

Neuf motifs : assez pour six sections avec une combinaison différente chacune.

## Arrangement

```arrangement tempo=84
section Intro   1-8   : Hats swing, Chords A
section Build   9-16  : Hats swing, Chords A, Bass A, Beat A kick [from=13]
section Groove  17-32 : Beat A [mute=32.3], Hats swing, Bass A, Chords A, Lead A [from=25]
section Break   33-40 : Hats swing, Chords B, Bass B, Lead A
section Peak    41-56 : Beat A [from=41.2], Hats swing, Bass A, Chords flip [to=45], Chords A [from=45], Lead B
section Exit    57-64 : Beat A [to=61], Hats swing, Bass A [to=63], Chords A
```

Coutures et événements uniques, par mesure :

- **1–8** : charley swingué et accords seuls : le balancement est la première chose entendue, avant toute pulsation.
- **9.1** : la basse entre sur la mesure ; **13.1** : le kick seul (« Beat A kick ») : la pulsation arrive en deux fois, couture par report.
- **17.1** : la caisse claire entre (« Beat A » complet) ; **25.1** : le lead entre sur le temps 2 (il ne joue jamais sur 1).
- **32.3** (événement unique 1) : la batterie se tait sur les temps 3 et 4 de la dernière mesure du groove (`mute=32.3`) : l'hésitation avant la section B.
- **33–40** : la section B (contrainte 1), le seul moment hors du cycle ; pas de kick ni de caisse claire : l'harmonie exposée, la basse tenue.
- **41.1** : la batterie rentre sur le temps 2 (`from=41.2`, événement unique 2 : le temps 1 vide), la basse et les accords sur le temps 1 : anticipation.
- **42** (événement unique 3, la signature) : Am devient A majeur, Do♯ dans les accords, une seule fois ; retour au cycle en mineur à 46.
- **57–64** : sortie par retrait dans l'ordre inverse de l'arrivée : le lead part à 57, le beat à 61, la basse à 63, les accords et le charley vont jusqu'à 64 : fin par coupe à la barre, queue de Reverb des accords.

## Notes de finition

- **Sons** : Drums par défaut, kick un peu plus long (600 ms) ; « Hats swing » sur sa propre tranche à −15 dB ; basse en dents de scie, Filter passe-bas 300 Hz, pas de Reverb ; accords en triangle, Reverb par défaut, tranche à −6 dB ; lead en carré, Echo à la noire, mix 25 %, tranche à −6 dB ; Compressor 2:1 sur le master, master à −3 dB.
- **Humanisation** : le swing du charley est écrit (contrainte 2) ; pas de drift en millisecondes.
- **Laissé à l'oreille** : le niveau du charley ; si la bascule de tierce doit durer une ou deux mesures ; le mix de l'Echo du lead sur la section B.
- **Version suivante** : une seconde ligne de basse à l'octave sur le pic ; le swing du charley par un réglage de groove quand Faulk l'aura ; une sortie de 16 mesures.

## Check

(sortie de `sheet_tool.py check`, voir `check.txt` à côté de la fiche)
