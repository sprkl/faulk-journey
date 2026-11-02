# Néon sur la rocade

Instrumental synth-pop nocturne, 104 bpm, La majeur, 64 mesures (environ 2 min 28), forme par sections avec un refrain qui revient, écrit pour être construit dans Faulk avec les devices de `develop` à `85e3d9f` : Drums, Oscillator, Echo, Reverb, Filter, Compressor. Le morceau sert à éprouver les nouveautés du jour : l'arpège de doubles-croches à vélocités écrites (luminosité des notes), les notes fantômes des autres clips dans le piano roll, le clavier de la timeline et du piano roll, les couleurs de pistes, les vumètres partout et la réduction de gain du Compressor.

## Brief et contraintes

- **Tempo** : 104 bpm (fourchette synth-pop 95–118 ; assez lent pour que l'arpège de doubles-croches reste lisible, assez vif pour que la caisse claire sur 2 et 4 avance).
- **Tonalité** : La majeur (A B C# D E F# G#) ; progression vi–IV–I–V = F#m – D – A – E, deux mesures par accord, boucle de 8 mesures.
- **Palette par rôle** :
  - pulsation : Drums, kick sur 1 et 3, caisse claire sur 2 et 4, charley fermé en croches (« Beat ») ;
  - basse : Oscillator en dents de scie, croches pompées sur la fondamentale, Filter passe-bas 500 Hz (« Bass ») ;
  - harmonie : Oscillator en carré, enveloppe courte, **arpège de doubles-croches** à vélocités écrites, Echo croche (« Arp ») ;
  - lead : Oscillator en triangle, Echo croche pointée, Reverb (« Lead ») ;
  - texture : Oscillator en sinus, attaque longue, Reverb grande, **une seule note tenue** (« Pad »).
  - master : Compressor doux, Filter passe-bas au repos à 20 kHz (ne sert que l'événement 2).
- **Longueur cible** : 64 mesures, forme par sections : Intro 8 / Couplet 16 / Refrain 16 / Cassure 8 / Refrain 2 16. Le moment le plus dense est Refrain 2 à partir de 49 (76 % : un peu tard pour la règle des 55–70 %, assumé, parce qu'une cassure avant le dernier refrain est la forme du genre).
- **Contraintes arbitraires** :
  1. l'harmonie n'est jamais tenue : elle n'existe qu'en arpège de doubles-croches ; le pad ne tient qu'**une seule note**, La, pédale sous les quatre accords ;
  2. le lead n'utilise que cinq hauteurs : A B C# E F# (pentatonique majeure de La) ;
  3. **aucun charley ouvert** : la couche aiguë est l'arpège et ses échos.
- **Hypothèses** : Drums a cinq sons (kick, caisse claire, clap, charley fermé, charley ouvert) : la percussion à trois temps de la cassure est un clap ; pas de swing (#168) ; aucun dither à l'export.

## Boucle de départ

Pulsation d'abord, puis l'arpège (c'est lui qui définit le genre ici), puis la basse, puis le lead, puis le pad.

```pattern drums "Beat A" bars=2 grid=16
Kick  |x.......x.......|x.......x.....x.|
Snare |....X.......X...|....X.......X...|
CHat  |..x...x...x...x.|..x...x...x...x.|
```

Pourquoi : kick sur 1 et 3, un kick anticipé sur le « a » de 4 une mesure sur deux, caisse claire accentuée sur 2 et 4, charley fermé sur les contretemps seulement ; pas de charley ouvert (contrainte 3).

```pattern notes "Arp" bars=8 grid=16 vel=80 key="A major" role=chords
F#3@105 A3 C#4 F#4@60 A4@105 F#4 C#4 A3@60 F#3@105 A3 C#4 F#4@60 C#4@105 A3 F#3 A3@60 |
F#3@105 A3 C#4 F#4@60 A4@105 F#4 C#4 A3@60 F#3@105 A3 C#4 F#4@60 C#4@105 A3 F#3 A3@60 |
D3@105 F#3 A3 D4@60 F#4@105 D4 A3 F#3@60 D3@105 F#3 A3 D4@60 A3@105 F#3 D3 F#3@60 |
D3@105 F#3 A3 D4@60 F#4@105 D4 A3 F#3@60 D3@105 F#3 A3 D4@60 A3@105 F#3 D3 F#3@60 |
A3@105 C#4 E4 A4@60 C#5@105 A4 E4 C#4@60 A3@105 C#4 E4 A4@60 E4@105 C#4 A3 C#4@60 |
A3@105 C#4 E4 A4@60 C#5@105 A4 E4 C#4@60 A3@105 C#4 E4 A4@60 E4@105 C#4 A3 C#4@60 |
E3@105 G#3 B3 E4@60 G#4@105 E4 B3 G#3@60 E3@105 G#3 B3 E4@60 B3@105 G#3 E3 G#3@60 |
E3@105 G#3 B3 E4@60 G#4@105 E4 B3 G#3@60 E3@105 G#3 B3 E4@60 B3@105 G#3 E3 G#3@60 |
```

Pourquoi : chaque accord en arpège monte-descend sur une mesure (fondamentale, tierce, quinte, octave, dixième, puis redescente), répété deux fois ; les vélocités écrites (105 sur les temps, 80 entre, 60 sur les « a ») font la pulsation de la couche aiguë ; c'est la seule harmonie du morceau (contrainte 1).

```pattern notes "Bass A" bars=8 grid=8 octave=1 key="A major" role=bass
F#1 F#1 F#1 F#1 F#1 F#1 F#1 F#1 | F#1 F#1 F#1 F#1 F#1 F#1 F#2 F#2 |
D2 D2 D2 D2 D2 D2 D2 D2 | D2 D2 D2 D2 D2 D2 D3 D3 |
A1 A1 A1 A1 A1 A1 A1 A1 | A1 A1 A1 A1 A1 A1 A2 A2 |
E2 E2 E2 E2 E2 E2 E2 E2 | E2 E2 E2 E2 E2 E2 E3 E3 |
```

Pourquoi : croches pompées sur la fondamentale de chaque accord, l'octave sur les deux dernières croches de chaque accord annonce le changement : la basse suit l'harmonie à la lettre.

```pattern notes "Lead A" bars=8 grid=8 octave=5 key="A major" role=melody
. . E - F# - E - | C# - - - . . A4 B4 | C# - E - - - . . | . . . . . . . . |
. . E - F# - A - | F# - E - - - . . | C# - B4 - A4 - - - | - - - - . . . . |
```

Pourquoi : cinq hauteurs (contrainte 2), un appel (mesures 1–3) qui tourne autour de mi, une réponse (5–7) qui monte au sommet La 5 une seule fois (mesure 5, temps 4) et redescend par degrés jusqu'à la fondamentale ; la mesure 4 est vide et la 8 tenue, l'Echo remplit.

```pattern notes "Pad" bars=8 grid=4 octave=3
A - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - | - - - - |
```

Pourquoi : une seule note, La 3, pédale sous F#m (tierce), D (quinte), A (fondamentale) et E (quarte, tension) : la texture ne change pas, l'arpège fait le mouvement (contrainte 1).

## Variations

Une seule chose change par génération, jamais de retour en arrière.

```pattern drums "Hats" bars=1 grid=16
CHat  |x.o.x.o.x.o.x.o.|
```

Gen 1 (rythme) : « Beat A » réduit à son charley, mis en croches avec les contretemps en fantôme ; pour l'intro, sous le pad et l'arpège.

```pattern drums "Beat B" bars=2 grid=16
Kick  |x.......x..x....|x.......x..x..x.|
Snare |....X.......X...|....X.......X...|
CHat  |x.x.x.x.x.x.x.x.|x.x.x.x.x.x.x.x.|
```

Gen 2 (rythme) : « Beat A » dont le charley passe sur toutes les croches et dont le kick gagne le « a » de 3 à chaque mesure ; pour les refrains.

```pattern notes "Bass B" bars=8 grid=8 octave=1 key="A major" role=bass
F#1 F#1 F#1 F#2 F#1 F#1 F#1 F#2 | F#1 F#1 F#1 F#2 F#1 F#1 F#2 F#2 |
D2 D2 D2 D3 D2 D2 D2 D3 | D2 D2 D2 D3 D2 D2 D3 D3 |
A1 A1 A1 A2 A1 A1 A1 A2 | A1 A1 A1 A2 A1 A1 A2 A2 |
E2 E2 E2 E3 E2 E2 E2 E3 | E2 E2 E2 E3 E2 E2 E3 E3 |
```

Gen 3 (basse) : « Bass A » dont une croche sur quatre saute à l'octave : la basse pompe plus fort ; pour les refrains.

```pattern notes "Arp half" bars=8 grid=8 vel=80 key="A major" role=chords
F#3@105 C#4 A4@105 C#4 F#3@105 C#4 C#4@105 F#3 | F#3@105 C#4 A4@105 C#4 F#3@105 C#4 C#4@105 F#3 |
D3@105 A3 F#4@105 A3 D3@105 A3 A3@105 D3 | D3@105 A3 F#4@105 A3 D3@105 A3 A3@105 D3 |
A3@105 E4 C#5@105 E4 A3@105 E4 E4@105 A3 | A3@105 E4 C#5@105 E4 A3@105 E4 E4@105 A3 |
E3@105 B3 G#4@105 B3 E3@105 B3 B3@105 E3 | E3@105 B3 G#4@105 B3 E3@105 B3 B3@105 E3 |
```

Gen 4 (rythme de l'harmonie) : « Arp » dont on ne garde qu'une double-croche sur deux (les positions impaires) : même contour, moitié moins dense ; pour la cassure.

```pattern notes "Lead B" bars=8 grid=8 octave=5 key="A major" role=melody
. . E - F# - E - | C# - - - . . A4 B4 | C# - E - - - . . | . . . . . . . . |
. . E - F# - A - | F# - E - - - . . | C# - E - F# - - - | - - - - . . . . |
```

Gen 5 (mélodie) : « Lead A » dont la réponse ne redescend plus : elle remonte et s'arrête sur fa dièse, la sixte, sans résoudre ; pour la fin de la cassure et la fin du morceau.

```pattern drums "Fill" bars=2 grid=16
Kick  |x.......x.......|x.......x.......|
Snare |....X.......X...|....X...o.o.oxXX|
```

Gen 6 (rythme) : « Beat A » sans charley dont la dernière mesure roule en doubles vers la barre (fantôme, coup, fantôme, accent, accent) : anticipation, le temps 1 de la section suivante est vide, la batterie repart sur le temps 2.

```pattern drums "Perc 3" bars=3 grid=16
Clap  |o.....x.....o...|..x.....o.....x.|....o.....x.....|
```

Gen 7 (forme, boucle asynchrone) : un clap en cycle de trois temps (fantôme, puis coup une noire et demie plus tard) posé sur le 4/4 : la figure tourne sur 3 mesures et ne retombe sur le temps 1 qu'à la quatrième ; la section de 8 la coupe avant, c'est voulu.

```pattern notes "Lead X" bars=1 grid=16 octave=5
. . . . . . . . . . . . D - . .
```

Événement unique (hauteur hors des cinq : ré 5, la quarte, une seule fois, mesure 56 temps 4) : la contrainte 2 est levée une croche, à dessein.

## Arrangement

```arrangement tempo=104
section Intro    1-8   : Pad, Hats [from=5], Arp [from=5]
section Couplet  9-24  : Beat A [mute=24.4], Bass A, Arp, Pad [to=17], Lead A [from=17]
section Refrain  25-40 : Beat B [from=25.2 to=39], Fill [from=39], Bass B, Arp, Pad, Lead A
section Cassure  41-48 : Arp half, Pad, Perc 3, Lead B [from=45], Bass A [from=48.3]
section Refrain2 49-64 : Beat B [from=49.2], Bass B, Arp, Pad, Lead A [to=56.4], Lead X [from=56.4 to=57], Lead B [from=57], Perc 3 [to=61]
```

Coutures et événements uniques, par mesure :

- **5.1** : le charley et l'arpège entrent ensemble sous le pad ; **9.1** : la basse et la batterie entrent, le pad continue jusqu'à 17 : couture par report.
- **16.4.3** : jet d'Echo sur le lead à son entrée (événement unique 1) : le mix de l'Echo de la piste Lead passe de 0,3 à 0,8 sur une croche (16.4.3 → 17.1) et revient : couloir de device.
- **24.4** : la batterie se tait sur le dernier temps du couplet (`mute=24.4`), **25.1** vide côté batterie, « Beat B » repart sur le temps 2 (anticipation) ; la basse change de motif à 25.1 sans attendre : couture coarse + fine.
- **39 → 41** : « Fill » roule vers la cassure ; la cassure n'a pas de batterie, le roulement tombe dans le silence : couture par silence.
- **41 → 48** : le cutoff du **Filter du master** s'ouvre de 400 Hz à 20 kHz sur les huit mesures de la cassure (événement unique 2, couloir du master) : la cassure sort du brouillard vers le refrain.
- **45.1** : « Lead B » entre seul au-dessus de l'arpège réduit ; **48.3** : la basse rentre en retard, sur le temps 3 (`Bass A [from=48.3]`), deux temps avant le refrain : hésitation inversée (la basse annonce).
- **49.1** vide côté batterie, « Beat B » sur le temps 2 : anticipation ; **49.1** : le Filter du master est grand ouvert.
- **56.4** : une seule note hors des cinq, ré 5 (« Lead X »), à la fin de la phrase (événement unique 3) ; « Lead A » s'arrête juste avant pour lui laisser la place.
- **61** : le clap à trois temps s'arrête (`Perc 3 [to=61]`) : la fin se simplifie.
- **64** : fin par coupe à la barre, la queue de Reverb du pad et du lead et l'Echo de l'arpège finissent seuls.

## Notes de finition

- **Drums** : kick tune 50 Hz, declin 450 ms, punch 0,6 ; caisse claire 190 Hz, snap 0,65, declin 180 ms ; charley 8 kHz, declin 40 ms ; clap 1 500 Hz.
- **Bass** : dents de scie, attaque 3 ms, declin 150 ms, sustain 40 %, release 80 ms ; Filter passe-bas 500 Hz, résonance 15 %.
- **Arp** : carré, attaque 2 ms, declin 120 ms, sustain 0, release 60 ms, gain 0,45 ; Echo synchronisé croche, feedback 0,35, mix 0,25.
- **Lead** : triangle, attaque 15 ms, declin 300 ms, sustain 60 %, release 250 ms ; Echo croche pointée, feedback 0,45, mix 0,3 (événement 1 le pousse à 0,8) ; Reverb taille 0,6, mix 0,25.
- **Pad** : sinus, attaque 1 500 ms, release 2 500 ms, gain 0,35 ; Reverb taille 0,85, mix 0,45.
- **Master** : Compressor seuil −14 dB, ratio 2, makeup 2 dB ; Filter passe-bas 20 kHz au repos (couloir de l'événement 2) ; volume du master à régler après un premier export pour une crête sous −1 dBFS sans limitation.
- **Humain** : les vélocités de l'arpège et des caisses claires sont écrites ; pas de drift en millisecondes.
- **Laissé à l'oreille** : le niveau de l'arpège contre le lead à partir de 17, le point de départ du filtre de la cassure (400 Hz peut être trop sourd avec la basse absente).
- **Deuxième version** : un pont de 8 mesures sur ii–V (Bm – E) avant le dernier refrain, et un second pad qui tient la quinte (mi) pour épaissir sans briser la contrainte 1.

## Check

```

[drums] 'Beat A'  bars=2 grid=16 notes=17

[notes] 'Arp'  bars=8 grid=16 notes=128
  OK     all 128 notes are in A major
  INFO   contour: range 23 semitones, highest note occurs 2x, steps 0 / leaps 127, up 255 / down 253 semitones, 16.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Bass A'  bars=8 grid=8 notes=64
  OK     all 64 notes are in A major
  INFO   contour: range 22 semitones, highest note occurs 2x, steps 0 / leaps 7, up 48 / down 26 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Lead A'  bars=8 grid=8 notes=16
  OK     all 16 notes are in A major
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 8 / leaps 6, up 14 / down 21 semitones, 2.0 notes per bar

[notes] 'Pad'  bars=8 grid=4 notes=1

[drums] 'Hats'  bars=1 grid=16 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[drums] 'Beat B'  bars=2 grid=16 notes=27

[notes] 'Bass B'  bars=8 grid=8 notes=64
  OK     all 64 notes are in A major
  INFO   contour: range 22 semitones, highest note occurs 5x, steps 0 / leaps 31, up 192 / down 170 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Arp half'  bars=8 grid=8 notes=64
  OK     all 64 notes are in A major
  INFO   contour: range 23 semitones, highest note occurs 2x, steps 0 / leaps 51, up 189 / down 191 semitones, 8.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Lead B'  bars=8 grid=8 notes=16
  OK     all 16 notes are in A major
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 7 / leaps 7, up 19 / down 17 semitones, 2.0 notes per bar

[drums] 'Fill'  bars=2 grid=16 notes=13

[drums] 'Perc 3'  bars=3 grid=16 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Lead X'  bars=1 grid=16 notes=1

[arrangement] tempo=104
  Intro          bars   1-8   ( 8) 3 parts
                 edits: Hats [from=5]; Arp [from=5]
  Couplet        bars   9-24  (16) 5 parts
                 edits: Beat A [mute=24.4]; Pad [to=17]; Lead A [from=17]
  Refrain        bars  25-40  (16) 6 parts
                 edits: Beat B [from=25.2 to=39]; Fill [from=39]
  Cassure        bars  41-48  ( 8) 5 parts
                 edits: Lead B [from=45]; Bass A [from=48.3]
  Refrain2       bars  49-64  (16) 8 parts
                 edits: Beat B [from=49.2]; Lead A [to=56.4]; Lead X [from=56.4 to=57]; Lead B [from=57]; Perc 3 [to=61]
  total 64 bars

RESULT ok
```

