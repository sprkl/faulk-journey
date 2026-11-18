# Manège

## Brief et contraintes

Instrumental électronique enjoué, façon chanson sans paroles, 116 bpm, **La majeur**, avec une visite en **La mineur harmonique** (le parallèle), 80 mesures (2 min 46). Un refrain qui revient trois fois, sans changer une note, et qui rapporte quelque chose de chaque visite : c'est un tour de manège.

Form: F10 Rondo (A B A C A)

Profil : aucun

Profil de style : aucun (rotation morzak → drifting-cycles → aucun). Mes propres choix.

- **Tempo** : 116 bpm, 4/4, croches droites.
- **Tonalité** : La majeur (La Si Do♯ Ré Mi Fa♯ Sol♯) pour A et C ; La mineur harmonique (La Si Do Ré Mi Fa Sol♯) pour B ; l'accord de Mi majeur, commun aux deux, sert de porte au retour.
- **Palette par rôles** : pulsation = batterie (grosse caisse sur chaque temps, clap, charley à contretemps) ; basse = sub (sinus), jamais sur le premier temps ; harmonie = accords courts au son carré (A et C) ; nappe = dent de scie lente et large (B et coda seulement) ; lead = dent de scie filtrée, porte le refrain ; cloche = sinus à déclin long avec écho (la voix de B, puis le contre-chant du dernier A).
- **Longueur** : 80 mesures.
- **Forme** : F10. Les deux fiches précédentes sont F7 et F1 (exclues) ; F0 n'est pas demandé ; restent F5, F8, F10, F11 jamais utilisées et F2, F3, F4, F9 déjà vues. L'humeur « enjoué, chantant » est celle que F10 nomme ; un refrain immuable se prête aux clips liés.

Trois contraintes :

1. **A ne change jamais ses notes** : le refrain, sa basse et ses accords sont les mêmes à chaque retour ; ce qui change vient des visites (l'octave après B, le rythme à trois des charleys et la cloche après C).
2. **Le refrain tient en cinq notes** : La Si Do♯ Mi Fa♯ (pentatonique majeure), sommet Fa♯5 une seule fois par tour.
3. **La basse ne joue jamais le premier temps** : la grosse caisse le tient seule ; et **aucun roulement** : chaque couture est un retrait (fenêtres), jamais un remplissage.

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Filter, Echo, Reverb, Bloom, Compressor, Ceiling).

## Boucle de départ

Le refrain : quatre mesures, cinq notes, un seul sommet (Fa♯5, mesure 3), il finit sur Si (la quinte de Mi) : une question qui ramène au début.

```pattern notes "Hook" bars=4 grid=8 octave=4 key="A major" role=hook
C#5 . E5 . C#5 B4 A4 . | F#4 . A4 . B4 - - . |
C#5 . E5 . F#5 E5 C#5 . | B4 . C#5 B4 - - . . |
```

La basse : la fondamentale sur les contretemps, jamais sur le premier temps, une note de l'accord en levée.

```pattern notes "Basse A" bars=4 grid=8 octave=2 key="A major" role=bass
. A1 . A1 . . A1 C#2 | . F#1 . F#1 . . F#1 A1 |
. D2 . D2 . . D2 F#2 | . E2 . E2 . . E2 B1 |
```

Le cycle de A : La add9 – Fa♯m7 – Ré maj7 – Mi, une mesure par accord, voix serrées.

```pattern notes "Accords A" bars=4 grid=4 octave=3 key="A major" role=chords
A3+B3+C#4+E4 - - - | F#3+A3+C#4+E4 - - - | F#3+A3+C#4+D4 - - - | E3+G#3+B3+E4 - - - |
```

```pattern drums "Beat A" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |..x...x...x...x.|
```

## Variations

- **Hook haut** (gén. 2, registre) : le refrain une octave plus haut, pour le retour après B.

```pattern notes "Hook haut" bars=4 grid=8 octave=5 key="A major" role=hook
C#6 . E6 . C#6 B5 A5 . | F#5 . A5 . B5 - - . |
C#6 . E6 . F#6 E6 C#6 . | B5 . C#6 B5 - - . . |
```

- **Nappe B** (gén. 3, harmonie et tonalité) : la visite en La mineur harmonique, Fa maj7 – Rém7 – Lam add9 – Mi, deux mesures par accord ; le Mi majeur final est la porte du retour.

```pattern notes "Nappe B" bars=8 grid=4 octave=3 key="A harmonic minor" role=pad
F3+A3+C4+E4 - - - | - - - - | F3+A3+C4+D4 - - - | - - - - |
E3+A3+B3+C4 - - - | - - - - | E3+G#3+B3+E4 - - - | - - - - |
```

- **Cloche B** (gén. 4, mélodie et son) : la voix de B, notes longues, sommet Si5 une seule fois (21.4).

```pattern notes "Cloche B" bars=8 grid=8 octave=5 key="A harmonic minor" role=melody
E5 - - A5 - - - . | F5 - E5 - C5 - - . |
D5 - - F5 - - - . | E5 - D5 - A4 - - . |
C5 - - E5 - - B5 - | A5 - - - E5 - - . |
G#5 - - B4 - - E5 - | - - - - . . . . |
```

- **Stab C** (gén. 5, rythme) : trois contre quatre, l'accord de Fa♯m7 frappé toutes les trois doubles croches.

```pattern notes "Stab C" bars=1 grid=16 octave=3 key="A major" role=chords
F#3+A3+C#4+E4 . . F#3+A3+C#4+E4 . . F#3+A3+C#4+E4 . . F#3+A3+C#4+E4 . . F#3+A3+C#4+E4 . . F#3+A3+C#4+E4 |
```

- **Stab C2** (gén. 6, harmonie) : le même geste une quarte plus haut, Sim7.

```pattern notes "Stab C2" bars=1 grid=16 octave=3 key="A major" role=chords
B3+D4+F#4+A4 . . B3+D4+F#4+A4 . . B3+D4+F#4+A4 . . B3+D4+F#4+A4 . . B3+D4+F#4+A4 . . B3+D4+F#4+A4 |
```

- **Cellule C** (gén. 7, mélodie) : trois notes du refrain, syncopées, en temps droit contre les accords à trois. Le Fa♯5 revient à chaque mesure : c'est une cellule rythmique, pas une phrase (rôle `riff`, le sommet répété est voulu).

```pattern notes "Cellule C" bars=2 grid=16 octave=5 key="A major" role=riff
. . C#5 . E5 . . F#5 . . E5 . C#5 . . . | . . C#5 . E5 . . F#5 . . . . . . . . |
```

- **Beat C** (gén. 8, rythme) : la batterie de C, le charley à trois, grosse caisse à la blanche, un seul clap.

```pattern drums "Beat C" bars=1 grid=16
Kick  |x.......x.......|
Clap  |............x...|
CHat  |x..x..x..x..x..x|
```

- **Beat A3** (gén. 9, rythme) : le Beat A qui garde de C son charley à trois.

```pattern drums "Beat A3" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |x..x..x..x..x..x|
```

- **Contre** (gén. 10, mélodie et son) : la cloche de B revient en contre-chant dans les trous du refrain (fin des mesures 2 et 4).

```pattern notes "Contre" bars=4 grid=8 octave=5 key="A major" role=counter
. . . . . . . . | . . . . . E5 F#5 A5 | - - . . . . . . | . . . . G#5 - E5 - |
```

- **Hook double** (gén. 11, registre) : le refrain aux deux octaves à la fois, pour les huit dernières mesures de A.

```pattern notes "Hook double" bars=4 grid=8 octave=4 key="A major" role=hook
C#5+C#6 . E5+E6 . C#5+C#6 B4+B5 A4+A5 . | F#4+F#5 . A4+A5 . B4+B5 - - . |
C#5+C#6 . E5+E6 . F#5+F#6 E5+E6 C#5+C#6 . | B4+B5 . C#5+C#6 B4+B5 - - . . |
```

- **Nappe fin** (gén. 12, forme) : La add9 tenu quatre mesures sous le dernier tour ; le refrain finit sur Si, la neuvième : non résolu.

```pattern notes "Nappe fin" bars=4 grid=4 octave=3 key="A major" role=pad
A3+B3+C#4+E4 - - - | - - - - | - - - - | - - - - |
```

Dispositif structurel : le trois contre quatre (accords et charley de C), puis gardé par le charley du dernier A.

## Arrangement

Form: F10 Rondo (A B A C A)

```arrangement tempo=116
section A1    1-16  : Beat A [to=16.3], Basse A, Accords A, Hook [from=5]
section B     17-24 : Nappe B, Cloche B
section A2    25-40 : Beat A, Basse A [from=26], Accords A, Hook haut
section C     41-48 : Beat C [mute=48], Stab C [to=45], Stab C2 [from=45 mute=48], Cellule C [mute=48]
section A3a   49-56 : Beat A3, Basse A, Accords A, Hook
section A3b   57-64 : Beat A3, Basse A, Accords A, Hook haut, Contre
section A3c   65-72 : Beat A3, Basse A, Accords A, Hook double, Contre
section Coda  73-80 : Hook, Nappe fin [from=77]
```

Cycles d'accords par section :

- A (1–16, 25–40, 49–72) : La add9 – Fa♯m7 – Ré maj7 – Mi, une mesure par accord (contrainte 1 : le même à chaque retour).
- B (17–24) : Fa maj7 – Rém7 – Lam add9 – Mi, deux mesures par accord, en La mineur harmonique.
- C (41–48) : Fa♯m7 (quatre mesures) – Sim7 (trois mesures) – silence (48).
- Coda (73–80) : rien sous le refrain, puis La add9 tenu (77–80).

Coutures :

- 16 → 17 : la batterie s'arrête deux temps plus tôt (16.3) ; sur 17.1 basse, accords et lead disparaissent, le mode bascule en mineur.
- 24 → 25 : le Mi majeur de la nappe est la porte ; le refrain revient une octave plus haut sur 25.1, la basse seulement à la mesure 26.
- 40 → 41 : coupe franche ; la basse sort pour huit mesures, les accords passent à trois contre quatre.
- 47 → 48 → 49 : la mesure 48 est vide (seules les queues d'écho) ; tout A revient sur 49.1, avec le charley à trois.
- 56 → 57 et 64 → 65 : le refrain monte d'une octave, la cloche entre, puis les deux octaves ensemble.
- 72 → 73 : tout tombe d'un coup ; le refrain seul, le filtre se ferme ; la nappe entre à 77.

Événements uniques :

1. 17.1 : bascule en La mineur harmonique, batterie, basse et accords sortent, la cloche entre (structurel).
2. 21.4 : le Si5 de la cloche, sa note la plus haute.
3. 26.1 : la basse revient une mesure après le refrain.
4. 41.1 : trois contre quatre, sans basse.
5. 48 : une mesure de silence (structurel).
6. 67.3 : le Fa♯6 du refrain doublé, la note la plus haute du morceau (elle sonne aussi à 27.3 et 59.3, seule ; ici avec son octave).
7. 73.1 : le refrain seul.

## Automation

La coupure du filtre du lead : ouverte pour A, assombrie pendant C où elle s'ouvre lentement puis vite vers le silence, puis elle se ferme vite puis lentement sur la coda.

```automation "Coupure lead" part="Hook" param=cutoff curve=linear
1.1 95 step, 41.1 60 ease-in, 47.4 100 step, 73.1 100 ease-out, 80.4 50
```

La coupure du filtre des accords : fermée au début de C, elle s'ouvre lentement puis vite jusqu'à la mesure vide, et revient à sa place pour le dernier A.

```automation "Coupure accords" part="Stab C" param=cutoff curve=linear
1.1 80 step, 41.1 45 ease-in, 47.4 110 step, 49.1 80
```

Le volume de la nappe : elle gonfle en S sous la cloche, retombe vers la porte, et reprend son niveau pour la coda.

```automation "Volume nappe" part="Nappe B" param=volume curve=linear
17.1 60 smooth, 21.1 95 linear, 24.4 70 step, 73.1 85
```

Dans Faulk : « Coupure lead » = Fréquence de coupure du Filter de la piste Lead ; « Coupure accords » = Fréquence de coupure du Filter de la piste Accords ; « Volume nappe » = Volume de la piste Nappe.

## Notes de finition

Sons : Lead = Oscillator dent de scie, relâchement 200 ms, Filter passe-bas automatisé (≈ 900 Hz à 6 kHz), Echo 1/8. mélange 20 %, Reverb mélange 15 %. Accords = carré, déclin 200 ms, maintien 50 %, relâchement 150 ms, Filter passe-bas automatisé (≈ 500 Hz à 6 kHz), Echo 1/8. mélange 15 % (ses queues remplissent la mesure 48). Nappe = dent de scie, attaque 400 ms, relâchement 900 ms, Filter passe-bas 1,5 kHz, Bloom Ensemble, Reverb taille 70 % mélange 40 %, volume automatisé. Cloche = sinus, attaque 2 ms, déclin 600 ms, maintien 20 %, relâchement 600 ms, Echo 1/4 mélange 30 %, Reverb mélange 35 %. Basse = sinus, relâchement 80 ms. Batterie = le kit de Drums tel quel. Master = Compressor doux puis Ceiling −0,3 dB.

Mix: Drums: C, front (no Reverb), no width, kick 50–100 Hz, hats above 5 kHz
Mix: Basse: C, front (no effect), no width, 46–100 Hz (F#1–F#2)
Mix: Accords: L15, middle (Echo eighth_dotted mix 0.15, Filter lowpass 500 Hz–6 kHz automated), no width, 165–900 Hz (E3–A4)
Mix: Nappe: C, back (Reverb size 0.7 mix 0.4, Filter lowpass 1.5 kHz), Bloom ensemble, 165 Hz–1.5 kHz (E3–E4)
Mix: Lead: C, front (Reverb mix 0.15, Echo eighth_dotted mix 0.2, Filter lowpass 900 Hz–6 kHz automated), no width, 370 Hz–6 kHz (F#4–F#6)
Mix: Cloche: R20, middle to back (Echo quarter mix 0.3, Reverb mix 0.35), no width, 440 Hz–2 kHz (A4–B5)
Mono check: 1, 3 and 4 by reading (kick, bass and lead at C; Bloom ensemble only on the pad; accords at L15 and cloche at R20 are not a mirrored pair and nothing is hard-panned); 2 does not apply; the rest is left to the ear.

Humanisation : aucune dans la fiche ; le trois contre quatre et les filtres portent le mouvement. Laissé à l'oreille : le niveau du sub contre la grosse caisse, la longueur des queues d'écho dans la mesure 48, le niveau de la cloche contre le refrain doublé. Une seconde version pourrait essayer : B en 6/8, le refrain à la basse dans la coda, un vrai cycle de trois mesures pour les accords de C.

## Check

```

[notes] 'Hook'  bars=4 grid=8 notes=16
  OK     all 16 notes are in A major
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 9 / leaps 6, up 17 / down 19 semitones, 4.0 notes per bar

[notes] 'Basse A'  bars=4 grid=8 notes=16
  OK     all 16 notes are in A major
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 1 / leaps 6, up 16 / down 14 semitones, 4.0 notes per bar

[notes] 'Accords A'  bars=4 grid=4 notes=16
  OK     all 16 notes are in A major

[drums] 'Beat A'  bars=1 grid=16 notes=10

[notes] 'Hook haut'  bars=4 grid=8 notes=16
  OK     all 16 notes are in A major
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 9 / leaps 6, up 17 / down 19 semitones, 4.0 notes per bar

[notes] 'Nappe B'  bars=8 grid=4 notes=16
  OK     all 16 notes are in A harmonic minor

[notes] 'Cloche B'  bars=8 grid=8 notes=18
  OK     all 18 notes are in A harmonic minor
  INFO   contour: range 14 semitones, highest note occurs 1x, steps 5 / leaps 12, up 33 / down 33 semitones, 2.2 notes per bar

[notes] 'Stab C'  bars=1 grid=16 notes=24
  OK     all 24 notes are in A major

[notes] 'Stab C2'  bars=1 grid=16 notes=24
  OK     all 24 notes are in A major

[notes] 'Cellule C'  bars=2 grid=16 notes=8
  OK     all 8 notes are in A major
  INFO   contour: range 5 semitones, highest note occurs 2x, steps 3 / leaps 3, up 10 / down 5 semitones, 4.0 notes per bar

[drums] 'Beat C'  bars=1 grid=16 notes=9

[drums] 'Beat A3'  bars=1 grid=16 notes=12

[notes] 'Contre'  bars=4 grid=8 notes=5
  OK     all 5 notes are in A major
  INFO   contour: range 5 semitones, highest note occurs 1x, steps 2 / leaps 2, up 5 / down 5 semitones, 1.2 notes per bar

[notes] 'Hook double'  bars=4 grid=8 notes=32
  OK     all 32 notes are in A major

[notes] 'Nappe fin'  bars=4 grid=4 notes=4
  OK     all 4 notes are in A major

[arrangement] tempo=116
  A1             bars   1-16  (16) 4 parts
                 edits: Beat A [to=16.3]; Hook [from=5]
  B              bars  17-24  ( 8) 2 parts
  A2             bars  25-40  (16) 4 parts
                 edits: Basse A [from=26]
  C              bars  41-48  ( 8) 4 parts
                 edits: Beat C [mute=48]; Stab C [to=45]; Stab C2 [from=45 mute=48]; Cellule C [mute=48]
  A3a            bars  49-56  ( 8) 4 parts
  A3b            bars  57-64  ( 8) 5 parts
  A3c            bars  65-72  ( 8) 5 parts
  Coda           bars  73-80  ( 8) 2 parts
                 edits: Nappe fin [from=77]
  total 80 bars

[automation] 'Coupure lead'  part='Hook' cc=74 (cutoff) curve=linear points=5

[automation] 'Coupure accords'  part='Stab C' cc=74 (cutoff) curve=linear points=4

[automation] 'Volume nappe'  part='Nappe B' cc=7 (volume) curve=linear points=4

RESULT ok
```
