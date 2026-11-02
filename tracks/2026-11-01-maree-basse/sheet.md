# Marée basse

Dub instrumental lent, 76 bpm, Ré dorien, 48 mesures (environ 2 min 32), forme par sections avec une coupure dub, écrit pour être construit dans Faulk avec les devices de `develop` à `7734e31` : Drums, Oscillator, Echo, Reverb, Filter, Compressor. Le morceau est pensé pour que les gestes du mixage soient dans la timeline : couloir de **panoramique du master** (#412) et couloir de **Filter du master** édités à la souris dans l'arrangement (#407), et un jet d'Echo sur la caisse claire piloté par un couloir de device.

## Brief et contraintes

- **Tempo** : 76 bpm (fourchette dub 60–90 ; assez lent pour que les contretemps du skank respirent, assez rapide pour que la caisse claire sur 3 ne traîne pas).
- **Tonalité** : Ré dorien (D E F G A B C) ; **un seul accord**, Dm7 (D F A C), tout le morceau.
- **Palette par rôle** :
  - pulsation : Drums, kick sur 1 et 3, caisse claire sur 3 (demi-temps), **aucun charley** (« Beat ») ;
  - basse : Oscillator en triangle, enveloppe courte, Filter passe-bas 300 Hz (« Bass ») ;
  - harmonie : Oscillator en carré, declin 90 ms, Echo synchronisé croche pointée, accords Dm7 sur tous les « et » (« Skank ») ;
  - lead : Oscillator en dents de scie + Filter passe-bas 1,8 kHz + Echo croche (« Horn ») ;
  - texture : Oscillator en sinus, attaque longue, Reverb grande (« Pad »).
  - master : Filter passe-bas au repos à 20 kHz, Compressor doux ; panoramique du master au centre sauf l'événement 2.
- **Longueur cible** : 48 mesures, forme par sections : Intro 8 / A 16 / Coupure 8 / A' 16. Le moment le plus dense est A' à partir de 37 (75 %).
- **Contraintes arbitraires** :
  1. un seul accord, Dm7 : la basse et le lead font le mouvement, jamais l'harmonie ;
  2. **aucun charley**, fermé ou ouvert : la couche aiguë du rythme est le skank et ses échos ;
  3. le lead n'utilise que cinq hauteurs : D F G A C (pentatonique mineure).
- **Hypothèses** : Drums n'a ni rim ni shaker (5 sons) : les fantômes sont des caisses claires à vélocité 60 ; pas de swing (#168) : le laid-back vient des contretemps écrits et de l'Echo ; aucun dither à l'export.

## Boucle de départ

Pulsation d'abord, puis le skank (c'est lui qui définit le genre ici), puis la basse, puis le lead, puis le pad.

```pattern drums "Beat A" bars=2 grid=16
Kick  |x.......x.....x.|x.......x.......|
Snare |........X.......|........X.....o.|
```

Pourquoi : kick sur 1 et 3, un kick anticipé sur le « a » de 4 une mesure sur deux, caisse claire accentuée sur 3 seulement, un fantôme sur le « a » de 4 de la deuxième mesure ; pas de charley (contrainte 2).

```pattern notes "Skank" bars=1 grid=8 octave=4 key="D dorian" role=chords
. D+F+A+C5 . D+F+A+C5 . D+F+A+C5 . D+F+A+C5
```

Pourquoi : Dm7 complet sur chaque « et », jamais sur le temps : le kick et la caisse claire ont les temps, le skank a les contretemps (contrainte 1).

```pattern notes "Bass A" bars=2 grid=16 octave=2 key="D dorian" role=bass
D - - . . . A1 - - . . . . C - . | D - - . . . F - . . A1 - - - . . |
```

Pourquoi : ligne dub clairsemée, fondamentale sur le temps 1 puis la quinte en dessous entre les temps ; le do (septième) et le fa (tierce) sont le mouvement que l'accord unique ne fait pas.

```pattern notes "Horn A" bars=4 grid=8 octave=4 key="D dorian" role=melody
. . . . A . C5 . | D5 - - - . . . . | . . A . G . F . | D - - - . . . . |
```

Pourquoi : cinq hauteurs (contrainte 3), appel qui monte au sommet D5 une seule fois (mesure 2, temps 1), réponse qui redescend par degrés vers la fondamentale ; la mesure 4 est tenue, l'Echo remplit.

```pattern notes "Pad" bars=4 grid=4 octave=3
D+A+C4 - - - | - - - - | - - - - | - - - - |
```

Pourquoi : fondamentale, quinte et septième sans tierce : la texture ne dit pas « mineur », le skank le dit.

## Variations

Une seule chose change par génération, jamais de retour en arrière.

```pattern drums "Kick only" bars=2 grid=16
Kick  |x.......x.....x.|x.......x.......|
```

Gen 1 (rythme) : « Beat A » sans la caisse claire ; pour l'intro, la pulsation seule sous le pad.

```pattern drums "Beat B" bars=2 grid=16
Kick  |x.......x.....x.|x.......x.....x.|
Snare |........X.....o.|........X...o.o.|
```

Gen 2 (rythme) : « Beat A » dont le kick anticipé revient à chaque mesure et dont les fantômes de caisse claire doublent ; pour A'.

```pattern notes "Bass B" bars=2 grid=16 octave=2 key="D dorian" role=bass
D - - . . . A1 - - . . . . C - . | D - - . . . F - . . A1 - - D3 - . |
```

Gen 3 (basse) : « Bass A » dont la fin de phrase saute à l'octave (ré 3) : la réponse de la basse remonte avant la mesure suivante ; pour la coupure et A'.

```pattern notes "Skank held" bars=2 grid=8 octave=4 key="D dorian" role=chords
. D+F+A+C5 - - - - - - | . . . . . . . . |
```

Gen 4 (harmonie, rythme) : un seul skank tenu sur une mesure, puis une mesure de silence : dans la coupure, l'Echo remplit l'espace laissé.

```pattern notes "Horn B" bars=4 grid=8 octave=4 key="D dorian" role=melody
. . . . . A . C5 | . D5 - - - . . . | . . . A . G . F | . D - - - . . . |
```

Gen 5 (rythme de la mélodie) : « Horn A » avec toutes les attaques en retard d'une croche : la réponse hésite, le sommet D5 tombe sur le « et » de 1 ; pour la seconde moitié de A'.

```pattern drums "Fill" bars=2 grid=16
Kick  |x.......x.......|x.......x.......|
Snare |........X.......|........X...oxoX|
```

Gen 6 (rythme) : « Beat A » dont la dernière mesure roule en doubles (fantôme, coup, fantôme, accent) vers la barre : anticipation, le temps 1 de la section suivante est vide, la batterie repart sur le temps 2.

```pattern notes "Horn F" bars=1 grid=16 octave=5
. . . . . . . . . . . . . . F -
```

Événement unique (hauteur hors des cinq : fa 5, une seule fois, mesure 40 avant-dernière double) : la contrainte 3 est levée une double-croche, à dessein.

## Arrangement

```arrangement tempo=76
section Intro   1-8   : Pad, Kick only [from=5]
section A       9-24  : Beat A [mute=24.4], Bass A, Skank, Pad [to=17], Horn A [from=17]
section Coupure 25-32 : Skank held, Bass B [from=25.3], Pad, Fill [from=31]
section Apost   33-48 : Beat B [from=33.2], Bass B, Skank, Horn A [from=37 to=41], Horn F [from=40.4 to=41], Horn B [from=41 to=45], Pad [from=45]
```

Coutures et événements uniques, par mesure :

- **5.1** : le kick seul entre sous le pad ; **9.1** : le skank et la basse entrent ensemble, la caisse claire n'arrive qu'à 9.3 avec « Beat A » : couture par silence.
- **16.4** : jet d'Echo sur la caisse claire (événement unique 1) : le mix de l'Echo de la piste Drums passe de 0 à 0,6 sur un temps (16.4 → 17.1), feedback 0,7, et revient à 0 : couloir de device.
- **24.4** : la batterie se tait sur le dernier temps (`mute=24.4`) ; **24.3 → 26.1** : le **panoramique du master** balaie de −0,8 à +0,8 puis revient au centre (événement unique 2, couloir du master, #412) : la queue d'Echo du skank traverse le champ stéréo à l'entrée de la coupure.
- **25.3** : la basse entre en retard, sur le « et » de 2 (`Bass B [from=25.3]`) : couture par hésitation.
- **31 → 33.2** : « Fill » roule vers la barre, 33.1 vide, « Beat B » repart sur le temps 2 : anticipation (coutures coarse + fine).
- **40.4.3** : une seule note hors des cinq, fa 5 (« Horn F »), à la fin de la phrase (événement unique 3).
- **45.1 → 48.4** : le cutoff du **Filter du master** se ferme de 20 kHz à 250 Hz sur quatre mesures (événement unique 4, couloir du master dans la timeline, #407) ; le pad revient à 45 pour avoir quelque chose à filtrer.
- **48** : fin par coupe à la barre ; la queue de Reverb du pad et l'Echo du skank finissent seuls, filtrés.

## Notes de finition

- **Drums** : kick tune 48 Hz, declin 600 ms, punch 0,7 ; caisse claire 170 Hz, snap 0,5 ; Echo en insert, mode synchronisé croche pointée, mix au repos 0, feedback 0,7 (ne sert que l'événement 1).
- **Bass** : triangle, attaque 5 ms, declin 250 ms, sustain 60 %, release 120 ms ; Filter passe-bas 300 Hz, résonance 10 %.
- **Skank** : carré, declin 90 ms, sustain 0, gain 0,5 ; Echo synchronisé croche pointée, feedback 0,55, mix 0,35 : c'est l'Echo qui fait le dub.
- **Horn** : dents de scie, attaque 20 ms, declin 400 ms, sustain 50 %, release 300 ms ; Filter passe-bas 1,8 kHz, résonance 20 % ; Echo croche, feedback 0,4, mix 0,3.
- **Pad** : sinus, attaque 1 200 ms, release 2 000 ms, gain 0,6 ; Reverb taille 0,85, mix 0,45. Après le premier export (pad trop fort seul dans l'intro, −22,5 dB RMS contre −19 pour A) : gain ramené à 0,35.
- **Master** : Compressor seuil −14 dB, ratio 2, makeup 2 dB ; Filter passe-bas 20 kHz au repos (couloir de l'événement 4) ; panoramique au centre (couloir de l'événement 2) ; volume à régler après un premier export pour une crête sous −1 dBFS. Premier export à 0 dB : le limiteur de sortie a travaillé (1,3 dB de réduction, crête −0,3 dBFS) ; master ramené à −3 dB, export final crête −2,0 dBFS sans limitation.
- **Humain** : les vélocités des caisses claires sont écrites ; pas de drift en millisecondes.
- **Laissé à l'oreille** : le niveau du skank contre le horn à partir de 41, le temps de fermeture du filtre final.
- **Deuxième version** : une coupure de 16 mesures avec la basse seule et ses propres jets d'Echo, et un deuxième accord (G, IV du dorien) pendant quatre mesures de A'.

## Check

```

[drums] 'Beat A'  bars=2 grid=16 notes=8

[notes] 'Skank'  bars=1 grid=8 notes=16
  OK     all 16 notes are in D dorian

[notes] 'Bass A'  bars=2 grid=16 notes=6
  OK     all 6 notes are in D dorian
  INFO   contour: range 8 semitones, highest note occurs 1x, steps 1 / leaps 4, up 8 / down 13 semitones, 3.0 notes per bar

[notes] 'Horn A'  bars=4 grid=8 notes=7
  OK     all 7 notes are in D dorian
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 3 / leaps 3, up 5 / down 12 semitones, 1.8 notes per bar

[notes] 'Pad'  bars=4 grid=4 notes=3

[drums] 'Kick only'  bars=2 grid=16 notes=5

[drums] 'Beat B'  bars=2 grid=16 notes=11

[notes] 'Bass B'  bars=2 grid=16 notes=7
  OK     all 7 notes are in D dorian
  INFO   contour: range 17 semitones, highest note occurs 1x, steps 1 / leaps 5, up 25 / down 13 semitones, 3.5 notes per bar

[notes] 'Skank held'  bars=2 grid=8 notes=4
  OK     all 4 notes are in D dorian

[notes] 'Horn B'  bars=4 grid=8 notes=7
  OK     all 7 notes are in D dorian
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 3 / leaps 3, up 5 / down 12 semitones, 1.8 notes per bar

[drums] 'Fill'  bars=2 grid=16 notes=10

[notes] 'Horn F'  bars=1 grid=16 notes=1

[arrangement] tempo=76
  Intro          bars   1-8   ( 8) 2 parts
                 edits: Kick only [from=5]
  A              bars   9-24  (16) 5 parts
                 edits: Beat A [mute=24.4]; Pad [to=17]; Horn A [from=17]
  Coupure        bars  25-32  ( 8) 4 parts
                 edits: Bass B [from=25.3]; Fill [from=31]
  Apost          bars  33-48  (16) 7 parts
                 edits: Beat B [from=33.2]; Horn A [from=37 to=41]; Horn F [from=40.4 to=41]; Horn B [from=41 to=45]; Pad [from=45]
  total 48 bars

RESULT ok
```
