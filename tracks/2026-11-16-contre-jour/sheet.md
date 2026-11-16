# Contre-jour

## Brief et contraintes

Instrumental électronique sombre et chaud, hypnotique, 116 bpm, **Do dorien**, 64 mesures (2 min 12). Une boucle de quatre mesures qui ne change que par le timbre, une seule interruption, puis la même boucle réharmonisée qui se développe et s'arrête au milieu d'une phrase.

Form: F6 Boucle avec une interruption

Profil de style : **morzak** (rotation morzak → drifting-cycles → aucun).

- **Tempo** : 116 bpm, 4/4 (famille « groove moyen » 112–123 du profil, lecture directe).
- **Tonalité** : Do dorien (Do Ré Mi♭ Fa Sol La Si♭) : mineur avec IV majeur (Fa). Après l'interruption, deux couleurs empruntées : La♭ (♭VI) dans le cycle B, Ré♭ (♭II) dans l'interruption seulement.
- **Palette par rôles** (cinq rôles, peu de couches) : pulsation = batterie (grosse caisse sur chaque temps, clap, charley fermé) ; basse = dent de scie mono filtrée, dominante ; harmonie = nappe douce, basse dans le mix ; arpège = carré court, un rôle à part, figure de trois pas ; lead = contre-chant qui répond dans les trous de l'arpège.
- **Longueur** : 64 mesures.
- **Forme** : F6. Les deux passages précédents sont F7 et F9 (exclus) ; F3, F2 et F4 juste avant (écartés par le brief). Le profil nomme F3 et F6 : F6 est la seule qui reste, et c'est sa forme « plateau ». Écart assumé à la carte F6 : la boucle n'est pas complète dès la mesure 1 (batterie complète à 5, lead à 13).

Trois contraintes, dont deux gestes du profil :

1. *(profil, « Où va le style » 1)* **deux cycles qui alternent sur un groove constant** : cycle A dans le mode (Dom7 – Fa, i – IV), cycle B avec une couleur empruntée (Dom – La♭ – Si♭ – Fa). Les sections viennent de l'harmonie ; la batterie ne change presque pas.
2. *(profil, « Gestes à essayer » 7)* **arpège et lead s'emboîtent** : l'arpège est une figure de trois pas sur du 4/4 (polymétrie), il laisse un trou à la fin des mesures 2 et 4, et le lead ne chante que dans ces trous jusqu'au sommet.
3. *(la mienne)* **avant l'interruption, aucune note ne change** : de 5 à 28 les clips sont les mêmes, seuls le filtre de l'arpège, sa résonance et le filtre de la basse bougent (le lead entre à 13 et varie une fois à 21 : seule entorse, écrite).

La signature du profil est placée exprès : **le Fa majeur tenu 28 mesures devient Fa mineur à la mesure 29**, et c'est l'interruption elle-même.

Hypothèses : pas de voix, pas d'échantillons ; les sons sont ceux de Faulk (Oscillator, Drums, Filter, Echo, Reverb, Bloom, Compressor, Ceiling).

Retours du fondateur pris en compte : l'interruption reste portée (basse tenue, nappe, charley fantôme sur chaque temps, une phrase du lead) ; les notes longues (nappe, lead de l'interruption et du sommet) passent par la réverbération et restent sous le niveau de la boucle.

## Catalogue d'attributs

- Tempo : 116 bpm, groove moyen, doubles croches droites (pas de swing : laissé).
- Mode et harmonie : mineur dorien, IV majeur ; cycles de 2 et 4 accords tenus chacun une demi-pièce ; ♭VI et ♭VII de passage dans le cycle B ; un accord qui change de tierce (Fa → Fam).
- Son : une voix simple pour le lead, un arpège comme rôle, une basse mono, une boîte à rythmes, cinq rôles, peu de réverbération dans le grave.
- Rythme : densité modérée, jamais chargé, aucun roulement.
- Mélodie : un arpège en cascade et une ligne qui se développe (énoncée, variée, étendue au sommet, amincie à la sortie).
- Forme : plateau avec une interruption (F6), le moment le plus dense tard (49–56, 77–88 %), fin très courte.
- Mix : la basse domine, présence et air discrets, dynamique non écrasée.

## Boucle de départ

L'arpège d'abord : une figure de trois pas (bas, milieu, haut) en croches, qui se décale contre la mesure et laisse un trou à la fin des mesures 2 et 4.

```pattern notes "Arp A" bars=4 grid=8 octave=4 key="C dorian" role=arp
C G Eb5 C G Eb5 C G | Eb5 C G Eb5 . . . . |
C A F5 C A F5 C A | F5 C A F5 . . . . |
```

La basse porte le morceau : la fondamentale, une croche pointée d'avance, une note de passage.

```pattern notes "Basse A" bars=4 grid=8 octave=2 key="C dorian" role=bass
C . C C . C . G1 | C . C C . Bb1 C . |
F1 . F1 F1 . F1 . C | F1 . F1 F1 . A1 C . |
```

La nappe : Dom7 sans fondamentale, puis Fa, deux mesures chacun.

```pattern notes "Nappe A" bars=4 grid=4 octave=3 key="C dorian" role=pad
Eb3+G3+Bb3 - - - | - - - - | F3+A3+C4 - - - | - - - - |
```

```pattern drums "Beat" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |o.x.o.x.o.x.o.x.|
```

Les quatre premières mesures n'ont que le charley.

```pattern drums "Beat charley" bars=1 grid=16
CHat  |o.x.o.x.o.x.o.x.|
```

Le lead répond dans les trous : trois notes à la fin de la mesure 2, trois à la fin de la mesure 4.

```pattern notes "Lead A" bars=4 grid=8 octave=5 key="C dorian" role=lead
. . . . . . . . | . . . . . G F D |
. . . . . . . . | . . . . . A G - |
```

## Variations

- **Lead A var** (gén. 2, mélodie) : la seconde réponse monte au Do6.

```pattern notes "Lead A var" bars=4 grid=8 octave=5 key="C dorian" role=lead
. . . . . . . . | . . . . . G F D |
. . . . . . . . | . . . . C6 A G - |
```

- **Interruption** (gén. 3, harmonie et forme) : Fa devient Fa mineur (la signature), puis Ré♭, entendu une seule fois. Sans `key=` : le La♭ et le Ré♭ sont hors du mode, c'est l'idée.

```pattern notes "Nappe rupture" bars=4 grid=4 octave=3 role=pad
F3+Ab3+C4 - - - | - - - - | F3+Ab3+Db4 - - - | - - - - |
```

```pattern notes "Basse rupture" bars=4 grid=4 octave=1 role=bass
F1 - - - | - - - - | Db2 - - - | - - - - |
```

```pattern notes "Lead rupture" bars=4 grid=8 octave=5 role=lead
C - - - Ab4 - - - | G4 - - - - - . . | Db - - - Ab4 - - - | F4 - - - - - . . |
```

```pattern drums "Beat rupture" bars=1 grid=16
CHat  |o...o...o...o...|
```

- **Cycle B** (gén. 4, harmonie) : la boucle revient réharmonisée, un accord par mesure : Dom – La♭ – Si♭ – Fa. Le La♭ est emprunté (rappel du check : décision) ; le Fa redevient majeur.

```pattern notes "Arp B" bars=4 grid=8 octave=4 key="C dorian" role=arp
C G Eb5 C G Eb5 C G | C Ab Eb5 C Ab . . . |
D Bb F5 D Bb F5 D Bb | C A F5 C A . . . |
```

```pattern notes "Basse B" bars=4 grid=8 octave=2 key="C dorian" role=bass
C . C C . C Eb . | Ab1 . Ab1 Ab1 . Ab1 C . |
Bb1 . Bb1 Bb1 . Bb1 D . | F1 . F1 F1 . A1 C . |
```

```pattern notes "Nappe B" bars=4 grid=4 octave=3 key="C dorian" role=pad
Eb3+G3+C4 - - - | Eb3+Ab3+C4 - - - | D3+F3+Bb3 - - - | F3+A3+C4 - - - |
```

```pattern notes "Lead B" bars=4 grid=8 octave=5 key="C dorian" role=lead
. . . . . . . . | . . . . . G Ab G |
. . . . . . . . | . . . . . A G F |
```

- **Lead B var** (gén. 5, mélodie) : une levée avant chaque réponse, sommet Si♭5.

```pattern notes "Lead B var" bars=4 grid=8 octave=5 key="C dorian" role=lead
. . . . . . Eb G | - . . . . G Ab G |
. . . . . . F Bb | - . . . . A G F |
```

- **Arp B 16** (gén. 6, rythme) : la même figure de trois pas en doubles croches, sans trou : cinq tours et une note par mesure.

```pattern notes "Arp B 16" bars=4 grid=16 octave=4 key="C dorian" role=arp
C G Eb5 C G Eb5 C G Eb5 C G Eb5 C G Eb5 C |
C Ab Eb5 C Ab Eb5 C Ab Eb5 C Ab Eb5 C Ab Eb5 C |
D Bb F5 D Bb F5 D Bb F5 D Bb F5 D Bb F5 D |
C A F5 C A F5 C A F5 C A F5 C A F5 C |
```

- **Basse B octave** (gén. 7, registre) : sauts d'octave au sommet.

```pattern notes "Basse B octave" bars=4 grid=8 octave=2 key="C dorian" role=bass
C . C3 C . C Eb C3 | Ab1 . Ab Ab1 . Ab1 C Ab |
Bb1 . Bb Bb1 . Bb1 D Bb | F1 . F F1 . A1 C F |
```

- **Lead sommet** (gén. 8, mélodie) : le lead ne répond plus, il chante par-dessus l'arpège, huit mesures, sommet Ré6 une seule fois.

```pattern notes "Lead sommet" bars=8 grid=8 octave=5 key="C dorian" role=lead
C6 - - Bb - G - - | Ab - - G - Eb F G |
F - - D - F Bb - | A - - G - F - - |
C6 - - Bb - G - - | Ab - - C6 - Ab G - |
D6 - - Bb - F - - | C6 - - A - F - - |
```

- **Beat ouvert** (gén. 9, son) : un charley ouvert sur la dernière croche, pour le sommet.

```pattern drums "Beat ouvert" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |o.x.o.x.o.x.o...|
OHat  |..............x.|
```

Dispositif structurel : la polymétrie (figure de trois pas sur du 4/4, remise à zéro toutes les mesures en doubles croches, toutes les deux mesures en croches) ; le hoquet arpège / lead ; une décision sur le silence (la coupe à 28.3 et à 64.3).

## Arrangement

Form: F6 Boucle avec une interruption

```arrangement tempo=116
section Amorce        1-4   : Arp A, Basse A, Nappe A, Beat charley
section Boucle        5-12  : Arp A, Basse A, Nappe A, Beat
section Boucle 2     13-20  : Arp A, Basse A, Nappe A, Beat, Lead A
section Boucle 3     21-28  : Arp A [to=28.3], Basse A [to=28.3], Nappe A [to=28.3], Beat [to=28.3], Lead A var [to=28.3]
section Interruption 29-32  : Nappe rupture, Basse rupture, Lead rupture, Beat rupture
section Retour       33-40  : Arp B, Basse B, Nappe B, Beat, Lead B
section Retour 2     41-48  : Arp B, Basse B, Nappe B, Beat [mute=48.4], Lead B var
section Sommet       49-56  : Arp B 16, Basse B octave, Nappe B, Beat ouvert, Lead sommet
section Sortie       57-60  : Arp B 16, Basse B octave, Nappe B, Beat ouvert, Lead B
section Chute        61-64  : Arp B 16 [to=64.3], Basse B octave [to=64.3], Nappe B [to=64.3], Beat ouvert [to=64.3], Lead B [to=64.3]
```

Cycles d'accords par section :

- Amorce, Boucle, Boucle 2, Boucle 3 (1–28) : cycle A, Dom7 – Fa (i – IV dorien), deux mesures par accord.
- Interruption (29–32) : Fam – Ré♭ (iv – ♭II), deux mesures par accord, entendus une seule fois.
- Retour, Retour 2, Sommet, Sortie, Chute (33–64) : cycle B, Dom – La♭ – Si♭ – Fa (i – ♭VI – ♭VII – IV), une mesure par accord.

Arc : un plateau (5–28), l'interruption (29–32, le seul événement de la première moitié, plus gros que tout ce qui précède parce que tout s'arrête au milieu d'une mesure et que l'accord change de tierce), un second plateau qui monte par le jeu (33–48 : filtre, levées du lead), le moment le plus dense à 49–56 (arpège en doubles croches, basse à l'octave, lead chanté), une sortie de quatre mesures où le lead revient à ses réponses, et la coupe.

Coutures :

- 4 → 5 : coupe franche, la grosse caisse entre sur 5.1.
- 12 → 13 et 20 → 21 : rien ne bouge que le filtre ; le lead entre dans le trou de la mesure 14.
- 28 → 29 : **la boucle est coupée à 28.3** (deux temps de vide, seule la queue de l'écho de l'arpège) ; sur 29.1 la nappe en Fa mineur, la basse tenue, le charley fantôme.
- 32 → 33 : le Fa4 du lead s'arrête deux croches avant la barre ; la boucle revient entière sur 33.1, en cycle B.
- 48 → 49 : la batterie manque sur 48.4 (hésitation) ; l'arpège passe en doubles croches sur 49.1.
- 56 → 57 : le lead retombe dans ses réponses ; le reste ne bouge pas.
- 64 : tout s'arrête sur 64.3, la réponse du lead n'a pas lieu.

Événements uniques :

1. 28.3 : la boucle coupée au milieu de la mesure (structurel).
2. 29 : Fa devient Fa mineur (la signature du profil), une seule fois.
3. 31 : l'accord de Ré♭ (♭II), entendu nulle part ailleurs.
4. 48.4 : un temps sans batterie.
5. 55.1 : le Ré6 du lead, sa note la plus haute, une seule fois.
6. 64.3 : la coupe au milieu de la phrase (structurel).

## Automation

La coupure du filtre de l'arpège : c'est elle qui fait vivre les 28 premières mesures (lente puis rapide), elle repart plus bas au retour, reste ouverte au sommet et se referme un peu dans la sortie.

```automation "Coupure arp" part="Arp A" param=cutoff curve=linear
1.1 40 ease-in, 28.2 100 step, 33.1 60 ease-in, 49.1 105 step, 57.1 105 ease-out, 64.2 75
```

La résonance du même filtre : elle monte avec la boucle 2 et 3, et retombe au retour.

```automation "Résonance arp" part="Arp A" param=resonance curve=linear
13.1 20 linear, 28.2 60 step, 33.1 25
```

La coupure de la basse : fermée au début, ouverte à la fin de la boucle, sombre sous l'interruption, puis ouverte jusqu'au sommet.

```automation "Coupure basse" part="Basse A" param=cutoff curve=linear
5.1 45 ease-in, 28.2 80 step, 29.1 40 step, 33.1 60 linear, 49.1 90
```

Le volume de la nappe : en retrait dans la boucle, un peu devant dans l'interruption puis en retrait en S avant le retour.

```automation "Volume nappe" part="Nappe A" param=volume curve=step
1.1 85, 29.1 100 smooth, 32.4 80 step, 33.1 85
```

Dans Faulk : « Coupure arp » et « Résonance arp » = Fréquence de coupure et Résonance du Filter de la piste Arp ; « Coupure basse » = Fréquence de coupure du Filter de la piste Basse ; « Volume nappe » = Volume de la piste Nappe.

## Notes de finition

Sons : Arp = Oscillator carré, attaque 5 ms, relâchement 120 ms, Filter passe-bas automatisé (≈ 500 Hz à 6 kHz), Echo 1/8. retour 35 % mélange 20 %. Basse = dent de scie, relâchement 80 ms, Filter passe-bas automatisé (≈ 300 Hz à 1,5 kHz), sans réverbération. Nappe = dent de scie, attaque 200 ms, relâchement 600 ms, Filter passe-bas 1,5 kHz, Bloom Ensemble, Reverb taille 70 % mélange 40 %. Lead = carré, relâchement 250 ms, Filter passe-bas 4 kHz, Echo 1/4 retour 40 % mélange 25 %, Reverb mélange 25 % pré-délai 30 ms. Drums tels quels.

Mix: Drums: C, front (no Reverb), no width, kick 50–100 Hz, hats above 5 kHz
Mix: Basse: C, front (no Reverb, Filter lowpass 300 Hz–1.5 kHz automated), no width, 40–250 Hz (Db1–C3)
Mix: Nappe: C, back (Reverb size 0.7 damping 0.7 mix 0.4, Filter lowpass 1.5 kHz), Bloom ensemble stereo_phase 150 depth 40 % tone 300 Hz mix 0.45, 150 Hz–1.5 kHz (D3–Db4)
Mix: Arp: L30, middle (Echo eighth_dotted feedback 0.35 mix 0.2, Filter lowpass 500 Hz–6 kHz automated, no Reverb), no width, 260 Hz–3 kHz (C4–F5)
Mix: Lead: C, front to middle (Reverb size 0.5 mix 0.25 predelay 0.03, Echo quarter feedback 0.4 mix 0.25, Filter lowpass 4 kHz), no width, 350 Hz–5 kHz (F4–D6)
Mono check: 1, 3 and 4 by reading (kick, bass and lead at C; Bloom only on the pad with tone 300 Hz and mix 0.45; the arp at L30 has an echo but no reverb, nothing is hard-panned); 2 does not apply (no mirrored pair); the rest is left to the ear.

Humanisation : aucune dans la fiche ; les charleys fantômes (vélocité 60) et les filtres portent le mouvement. Laissé à l'oreille : le niveau de la basse contre la grosse caisse, la durée du vide de 28.3 à 29, le niveau du lead de l'interruption. Une seconde version pourrait essayer : le swing des contretemps de la basse (geste 5 du profil), une interruption de huit mesures, la figure de trois pas en triolets pour les quatre dernières mesures.

Profil : gardé = tempo, mineur dorien avec IV majeur, cycles courts, cinq rôles, arpège comme rôle, basse dominante, la signature (Fa → Fam), deux cycles qui alternent, l'emboîtement arpège / lead et la polymétrie, les couloirs de timbre, le lead qui se développe. Plié = la bascule de tierce n'est pas au moment le plus dense mais fait l'interruption ; la carte F6 (boucle incomplète quatre mesures, lead à 13). Laissé = le swing, Fa mineur comme tonalité, la fin longue (F6 s'arrête au milieu d'une phrase), la grille descendante du dernier sommet.

## Check

```
[notes] 'Arp A'  bars=4 grid=8 notes=24
  OK     all 24 notes are in C dorian
  INFO   contour: range 17 semitones, highest note occurs 4x, steps 0 / leaps 23, up 128 / down 111 semitones, 6.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse A'  bars=4 grid=8 notes=20
  OK     all 20 notes are in C dorian
  INFO   contour: range 7 semitones, highest note occurs 10x, steps 2 / leaps 7, up 21 / down 21 semitones, 5.0 notes per bar

[notes] 'Nappe A'  bars=4 grid=4 notes=6
  OK     all 6 notes are in C dorian

[drums] 'Beat'  bars=1 grid=16 notes=14

[drums] 'Beat charley'  bars=1 grid=16 notes=8
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Lead A'  bars=4 grid=8 notes=5
  OK     all 5 notes are in C dorian
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 2 / leaps 2, up 7 / down 7 semitones, 1.2 notes per bar

[notes] 'Lead A var'  bars=4 grid=8 notes=6
  OK     all 6 notes are in C dorian
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 2 / leaps 3, up 10 / down 10 semitones, 1.5 notes per bar

[notes] 'Nappe rupture'  bars=4 grid=4 notes=6

[notes] 'Basse rupture'  bars=4 grid=4 notes=2

[notes] 'Lead rupture'  bars=4 grid=8 notes=6
  INFO   contour: range 8 semitones, highest note occurs 1x, steps 1 / leaps 4, up 6 / down 13 semitones, 1.5 notes per bar

[drums] 'Beat rupture'  bars=1 grid=16 notes=4
  NOTE   no kick in this pattern: fine if another part carries the pulse

[notes] 'Arp B'  bars=4 grid=8 notes=26
  WARN   2 note(s) outside C dorian: G#4 at bar 2 beat 1.5, G#4 at bar 2 beat 3. Keep each one only if it is a decision.
  INFO   contour: range 17 semitones, highest note occurs 3x, steps 0 / leaps 25, up 124 / down 115 semitones, 6.5 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Basse B'  bars=4 grid=8 notes=20
  WARN   4 note(s) outside C dorian: G#1 at bar 2 beat 1, G#1 at bar 2 beat 2, G#1 at bar 2 beat 2.5, G#1 at bar 2 beat 3.5. Keep each one only if it is a decision.
  INFO   contour: range 10 semitones, highest note occurs 1x, steps 1 / leaps 7, up 18 / down 18 semitones, 5.0 notes per bar

[notes] 'Nappe B'  bars=4 grid=4 notes=12
  WARN   1 note(s) outside C dorian: G#3 at bar 2 beat 1. Keep each one only if it is a decision.

[notes] 'Lead B'  bars=4 grid=8 notes=6
  WARN   1 note(s) outside C dorian: G#5 at bar 2 beat 4. Keep each one only if it is a decision.
  INFO   contour: range 4 semitones, highest note occurs 1x, steps 5 / leaps 0, up 3 / down 5 semitones, 1.5 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Lead B var'  bars=4 grid=8 notes=10
  WARN   1 note(s) outside C dorian: G#5 at bar 2 beat 4. Keep each one only if it is a decision.
  INFO   contour: range 7 semitones, highest note occurs 1x, steps 6 / leaps 2, up 10 / down 8 semitones, 2.5 notes per bar

[notes] 'Arp B 16'  bars=4 grid=16 notes=64
  WARN   5 note(s) outside C dorian: G#4 at bar 2 beat 1.25, G#4 at bar 2 beat 2, G#4 at bar 2 beat 2.75, G#4 at bar 2 beat 3.5, G#4 at bar 2 beat 4.25. Keep each one only if it is a decision.
  INFO   contour: range 17 semitones, highest note occurs 10x, steps 2 / leaps 60, up 312 / down 312 semitones, 16.0 notes per bar

[notes] 'Basse B octave'  bars=4 grid=8 notes=24
  WARN   5 note(s) outside C dorian: G#1 at bar 2 beat 1, G#2 at bar 2 beat 2, G#1 at bar 2 beat 2.5, G#1 at bar 2 beat 3.5, G#2 at bar 2 beat 4.5. Keep each one only if it is a decision.
  INFO   contour: range 19 semitones, highest note occurs 2x, steps 0 / leaps 20, up 96 / down 91 semitones, 6.0 notes per bar
  INFO   contour: all steps or all leaps; strong lines balance the two

[notes] 'Lead sommet'  bars=8 grid=8 notes=28
  WARN   3 note(s) outside C dorian: G#5 at bar 2 beat 1, G#5 at bar 6 beat 1, G#5 at bar 6 beat 3.5. Keep each one only if it is a decision.
  INFO   contour: range 12 semitones, highest note occurs 1x, steps 12 / leaps 15, up 39 / down 46 semitones, 3.5 notes per bar

[drums] 'Beat ouvert'  bars=1 grid=16 notes=14

[arrangement] tempo=116
  Amorce         bars   1-4   ( 4) 4 parts
  Boucle         bars   5-12  ( 8) 4 parts
  Boucle 2       bars  13-20  ( 8) 5 parts
  Boucle 3       bars  21-28  ( 8) 5 parts
                 edits: Arp A [to=28.3]; Basse A [to=28.3]; Nappe A [to=28.3]; Beat [to=28.3]; Lead A var [to=28.3]
  Interruption   bars  29-32  ( 4) 4 parts
  Retour         bars  33-40  ( 8) 5 parts
  Retour 2       bars  41-48  ( 8) 5 parts
                 edits: Beat [mute=48.4]
  Sommet         bars  49-56  ( 8) 5 parts
  Sortie         bars  57-60  ( 4) 5 parts
  Chute          bars  61-64  ( 4) 5 parts
                 edits: Arp B 16 [to=64.3]; Basse B octave [to=64.3]; Nappe B [to=64.3]; Beat ouvert [to=64.3]; Lead B [to=64.3]
  total 64 bars

[automation] 'Coupure arp'  part='Arp A' cc=74 (cutoff) curve=linear points=6

[automation] 'Résonance arp'  part='Arp A' cc=71 (resonance) curve=linear points=3

[automation] 'Coupure basse'  part='Basse A' cc=74 (cutoff) curve=linear points=5

[automation] 'Volume nappe'  part='Nappe A' cc=7 (volume) curve=step points=4

RESULT ok
```

Rappels gardés, chacun une décision : les arpèges sont tout en sauts et répètent leur note haute (c'est la figure) ; le La♭ (G#) des motifs du cycle B est l'emprunt ♭VI ; « Lead B » est tout en degrés conjoints (une réponse de trois notes) ; « Basse B octave » est tout en sauts (octaves).
