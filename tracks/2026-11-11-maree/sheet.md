# Marée

Instrumental électronique mélodique, 108 bpm (lecture médiane du profil), **Ré majeur** (maison) avec la **relative Si mineur** visitée au milieu et une **montée d'une tierce mineure vers Fa majeur** aux deux tiers, écrit sur le **profil de style drifting-cycles** (`.claude/skills/music-producer/references/styles/drifting-cycles.md`). Le titre : la marée, le même rivage que l'eau redessine à chaque heure. Le morceau est un **thème et variations** : un crochet de huit mesures énoncé dès la première, jamais récrit, réharmonisé par un cycle d'accords différent à chaque section, passé à la basse, réduit à son squelette sur une pédale, puis soulevé d'une tierce mineure et joué en canon avec lui-même. 96 mesures (3 min 33), forme **F4 Thème et variations**.

## Brief et contraintes

- **Profil de style** : **drifting-cycles**. Gardé : lecture médiane du tempo (108 dans 100–112), maison majeure et relative mineure visitée au milieu, cycles de 4 accords d'une ou deux mesures, un cycle neuf par section de 16 mesures, accords étendus (maj7, m7, add9, sus2, sus4), une section de pédale (la tonique tenue sous des accords qui bougent), une montée tardive de +3 demi-tons, crochet court énoncé tôt et varié par les accords, une longue phrase chantée dans le dernier tiers, intro sans accords, les deux signatures (la basse qui tient une note sous les accords puis bouge au premier temps du sommet ; la même mélodie deux fois sous des accords différents), formes préférées (F4 prise). Départs du profil : la montée tombe à 67 % (mesure 65 de 96) ; le roulement avant un changement de section est un bégaiement de Hiccup (le device existe, pas de roulement de caisse) ; pas de pompage de sidechain ni de montée de bruit filtré (Faulk n'a ni sidechain externe ni oscillateur de bruit : la montée est le filtre de la nappe qui s'ouvre) ; pas de swing sur les charleys (Faulk n'a pas de swing, #168 ouvert). Pas de voix.
- **Tempo** : 108 bpm.
- **Tonalité** : Ré majeur. Cinq images d'accords, une par section, chacune gardant un accord de la précédente comme ancre (move 1) :
  - **cycle A** (Thème, 1–16) : **Dmaj7 – Bm7 – Gmaj7 – Asus4** (I – vi – IV – Vsus), une mesure par accord, **sans nappe** : seuls l'arpège et la basse l'impliquent (intro sans accords, move 6) ;
  - **cycle B** (Variation 1, 17–32) : **Gmaj7 – Asus2 – Bm7 – F#m7** (IV – Vsus2 – vi – iii), une mesure par accord ; ancres G et Bm ; la nappe entre : **le même crochet, d'autres accords dessous** (signature 2, move 5) ;
  - **cycle C** (Variation 2, 33–48, **Si mineur**) : **Bm9 – Em7 – Gmaj7 – F#m7** (i – iv – VI – v), deux mesures par accord (harmonie lente) ; ancres G et F#m ;
  - **cycle D** (Variation 3, 49–64, pédale) : **Gmaj7/D – Asus4/D – Bm7/D – Dmaj7**, deux mesures par accord, puis **Gmaj7 – Asus4 tenu six mesures** (le sus tenu, résolu seulement au sommet, move 4) ; c'est le cycle A reparti de son troisième accord, **sur une pédale de Ré** (move 3, signature 1) ;
  - **cycle E** (Variation 4 et Retour, 65–96, **Fa majeur**) : **Fmaj7 – Dm7 – B♭maj7 – Csus4** (I – vi – IV – Vsus) : le cycle A soulevé de +3 demi-tons (move 2) ; la liaison : Asus4 (La Ré Mi) → Fmaj7 (Fa La Do Mi), La et Mi en commun, et le La4 du lead tenu à travers la coupure.
- **Palette par rôle** (sept pistes, master) :
  - pulsation : Drums ; « Beat A » kick sur chaque temps, clap sur 2 et 4, charley fermé en croches à 60, charley ouvert sur le dernier « a » ; « Beat B » demi-temps (kick sur 1 et le « et » de 3, clap sur 3) pour la variation 1 ; Hiccup sur la piste, mélange automatisé (bégaiement) ;
  - basse : Oscillator en dents de scie, release 150 ms, Filter passe-bas 250 Hz résonance 10 %, à −3 dB (« Bass A / B / D / E », « Hook basse ») ;
  - arpège : Oscillator en carré, release 60 ms, Filter passe-bas automatisé résonance 25 %, Echo 1/8 à 20 %, à −9 dB (« Arp A / B / E », montantes en croches) ;
  - nappe : Oscillator en dents de scie, attaque 300 ms, release 800 ms, Filter passe-bas 800 Hz automatisé, Bloom Ensemble, Reverb 35 %, à −12 dB (« Pad B / C / D1 / D2 / E / fin ») ;
  - lead : Oscillator en triangle, attaque 15 ms, release 400 ms, Bloom Vibrato au tempo 1/8 profondeur 20 %, Echo 1/8 mélange automatisé, à −6 dB (« Hook », « Tenues », « Squelette », « Hook F », « Chant ») ;
  - canon : Oscillator en sinus, attaque 30 ms, release 500 ms, Reverb 40 %, à −10 dB (« Canon » : le crochet soulevé, deux mesures plus tard) ;
  - master : Compressor seuil −14 dB, ratio 3, détection RMS, mélange 70 % ; Ceiling −0,5 dB ; master à −1 dB.
- **Longueur cible** : 96 mesures : six sections de 16 (Thème, Variation 1, 2, 3, 4, Retour).
- **Contraintes** (trois : deux moves du profil, une à moi) :
  1. **un cycle neuf par section, avec un accord de la section précédente en ancre** (move 1) ;
  2. **une montée tardive de +3 demi-tons à 67 %, avec une mesure amincie avant et une note tenue à travers la coupure** (move 2) ;
  3. **le crochet n'est jamais récrit** : ses 22 notes sont les mêmes dans toutes les sections ; seules sa hauteur d'octave (basse), sa transposition (+3) et sa réduction (squelette) changent. Pas de nouvelle mélodie avant la mesure 73 (le chant).
- **Hypothèses** : pas de voix ; aucun fichier audio ; tout vient des instruments et des effets de Faulk.
- **Forme** : `Form: F4 Thème et variations` (les deux passages précédents sont F6 « Lisière » et F0 « Floraison », exclus ; F0 exclu aussi par la ration ; le profil préfère F4, F9, F10, F1 ; F4 est la forme même de la signature « la même mélodie sous des accords différents »). Le plan de F4 est pris à 96 mesures avec deux échanges nommés : la variation 3 (pédale, squelette, nouvelle texture) et la variation 4 (nouveau centre tonal, canon) sont permutées pour que la montée tombe à 67 % et non à 51 % ; le retour reste dans la tonalité soulevée (un seul changement de tonalité, « Avoid » du profil), et son détail changé est la nappe qui tient le Csus4 non résolu sous les quatre dernières mesures.

## Catalogue d'attributs (profil drifting-cycles)

- Tempo : 108, lecture médiane.
- Mode et harmonie : Ré majeur, relative Si mineur au milieu, cycles de 4 accords (une ou deux mesures), extensions maj7 / m7 / add9 / sus2 / sus4, une section de pédale, une montée de +3.
- Son : lead triangle vibré, arpège carré filtré (le pluck), nappe large (Bloom Ensemble), sub propre qui tient la pédale, un canon en sinus ; pas de bruit filtré (absent de Faulk).
- Rythme : quatre-sur-le-temps, demi-temps pour une variation, un bégaiement avant la variation 3.
- Mélodie : crochet de 22 notes sur 8 mesures (quatre cellules de 2), énoncé à la mesure 1, réharmonisé, passé à la basse, réduit, soulevé, en canon ; une longue phrase chantée à 73.
- Forme : par sections de 16, intro sans accords, F4.
- Mix : bas-médiums pleins, sub propre, nappe large, basse et lead au centre.

## Boucle de départ

La pulsation d'abord, puis l'arpège (c'est lui qui porte l'harmonie de l'intro), la basse, le crochet.

```pattern drums "Beat A" bars=1 grid=16
Kick  |x...x...x...x...|
Clap  |....x.......x...|
CHat  |o.o.o.o.o.o.o.o.|
OHat  |..............o.|
```
Quatre sur le temps, clap 2 et 4, charleys fermés en croches à 60, un charley ouvert doux sur le dernier « a » (le fermé y sonne aussi : Faulk ne les étouffe pas l'un par l'autre, laissé tel quel).

```pattern notes "Arp A" bars=4 grid=8 octave=4 key="D major" role=arp
D4 F#4 A4 D5 D4 F#4 A4 D5 | B3 D4 F#4 B4 B3 D4 F#4 B4 | G3 B3 D4 G4 G3 B3 D4 G4 | A3 D4 E4 A4 A3 D4 E4 A4 |
```
Cascade montante en croches, deux par mesure, de la fondamentale à l'octave : D, Bm, G, Asus4 (La Ré Mi : le sus est dans l'arpège, pas de tierce). La note la plus haute revient à chaque cascade : c'est un arpège (le rappel du check est attendu).

```pattern notes "Bass A" bars=4 grid=8 octave=1 key="D major" role=bass
D2 - - - . D2 - . | B1 - - - . B1 - . | G1 - - - . G1 - . | A1 - - - . A1 - . |
```
Fondamentale tenue deux temps, silence, fondamentale sur le « et » de 3 : une figure, les hauteurs suivent les accords.

```pattern notes "Hook" bars=8 grid=8 octave=4 key="D major" role=lead
A4 - D5 - F#5 - - E5 | - - - - D5 - B4 - | A4 - D5 - F#5 - - G5 | A5 - - - - - . . | A4 - D5 - F#5 - - E5 | - - - - D5 - B4 - | A4 - B4 - D5 - E5 - | A4 - - - - - - - |
```
Le crochet (contrainte 3) : une cellule de deux mesures (La Ré Fa# Mi, Ré Si) dite deux fois, la seconde fois tournée vers le haut (Sol puis **La5**, le sommet, une fois, mesure 4), puis la même cellule et une descente par degrés qui se pose sur le La4 tenu une mesure : la quinte de Ré, qui deviendra la tierce de Fa. Vingt-deux notes, toutes dans Ré majeur, toutes tons d'accord ou couleurs (9e, 13e) sur chacun des cycles A, B et D.

## Variations

```pattern drums "Beat B" bars=1 grid=16
Kick  |x.........x.....|
Clap  |........x.......|
CHat  |o.o.o.o.o.o.o.o.|
```
Génération 1 (rythme, F4 variation 1) : demi-temps : kick sur 1 et le « et » de 3, clap sur 3, les croches de charley continuent.

```pattern notes "Arp B" bars=4 grid=8 octave=4 key="D major" role=arp
G3 B3 D4 G4 G3 B3 D4 G4 | A3 B3 E4 A4 A3 B3 E4 A4 | B3 D4 F#4 B4 B3 D4 F#4 B4 | F#3 A3 C#4 F#4 F#3 A3 C#4 F#4 |
```
Génération 2 (harmonie) : la même cascade sur le cycle B : G, Asus2 (La Si Mi), Bm, F#m.

```pattern notes "Bass B" bars=4 grid=8 octave=1 key="D major" role=bass
G1 - - - . G1 - . | A1 - - - . A1 - . | B1 - - - . B1 - . | F#1 - - - . F#1 - . |
```
Génération 3 (harmonie) : la figure de Bass A sur les fondamentales du cycle B.

```pattern notes "Pad B" bars=4 grid=4 octave=3 key="D major" role=pad
G3+B3+D4+F#4 - - - | A3+B3+E4 - - - | F#3+A3+B3+D4 - - - | F#3+A3+C#4+E4 - - - |
```
Génération 4 (son : les accords arrivent) : Gmaj7, Asus2, Bm7 en troisième renversement (Fa# en bas), F#m7 : la voix du bas descend Sol, La, Fa#, Fa#, le reste bouge d'un degré. Première nappe du morceau, à la mesure 17 : le crochet, inchangé, est entendu sous d'autres accords (signature 2).

```pattern notes "Hook basse" bars=8 grid=8 octave=2 key="B minor" role=bass
A2 - D3 - F#3 - - E3 | - - - - D3 - B2 - | A2 - D3 - F#3 - - G3 | A3 - - - - - . . | A2 - D3 - F#3 - - E3 | - - - - D3 - B2 - | A2 - B2 - D3 - E3 - | A2 - - - - - - - |
```
Génération 5 (registre, F4 variation 2 : la mélodie passe à la basse) : le crochet deux octaves plus bas, sur l'instrument de basse, sous le cycle C en Si mineur ; les accords sont tenus par la nappe et par les notes longues du lead. La basse ne fait plus les fondamentales : c'est l'échange de rôles (événement unique 1, structurel).

```pattern notes "Pad C" bars=8 grid=4 octave=3 key="B minor" role=pad
B3+D4+F#4+C#5 - - - | - - - - | E3+G3+B3+D4 - - - | - - - - | G3+B3+D4+F#4 - - - | - - - - | F#3+A3+C#4+E4 - - - | - - - - |
```
Génération 6 (harmonie : la relative) : Bm9 (la neuvième Do# en haut), Em7, Gmaj7, F#m7, deux mesures chacun : l'harmonie ralentit (contraste lent / rapide).

```pattern notes "Tenues" bars=8 grid=4 octave=4 key="B minor" role=lead
B4 - - - | - - - - | E4 - - - | - - - - | G4 - - - | - - - - | F#4 - - - | - - - - |
```
Génération 7 (rôle) : le lead tient les fondamentales du cycle C en notes de deux mesures pendant que la basse chante : l'autre moitié de l'échange.

```pattern notes "Bass D" bars=8 grid=8 octave=1 key="D major" role=bass
D2 - - - . D2 - . | D2 - - - . D2 - . | D2 - - - . D2 - . | D2 - - - . D2 - . | D2 - - - . D2 - . | D2 - - - . D2 - . | D2 - - - . D2 - . | D2 - - - . D2 - . |
```
Génération 8 (harmonie : la pédale, signature 1, move 3) : la figure de Bass A sur un seul Ré pendant seize mesures sous le cycle D ; la basse ne bouge qu'au premier temps de 65, sur le Fa.

```pattern notes "Pad D1" bars=8 grid=4 octave=3 key="D major" role=pad
G3+B3+D4+F#4 - - - | - - - - | A3+D4+E4 - - - | - - - - | F#3+A3+B3+D4 - - - | - - - - | D3+F#3+A3+C#4 - - - | - - - - |
```
Génération 9 (harmonie) : le cycle A reparti de son troisième accord, deux mesures chacun, sur la pédale : Gmaj7/D, Asus4/D, Bm7/D, Dmaj7.

```pattern notes "Pad D2" bars=8 grid=4 octave=3 key="D major" role=pad
G3+B3+D4+F#4 - - - | - - - - | A3+D4+E4 - - - | - - - - | - - - - | - - - - | - - - - | - - - - |
```
Génération 10 (harmonie, move 4) : Gmaj7 deux mesures puis **Asus4 tenu six mesures** (59–64), jamais résolu avant le Fmaj7 de 65 ; la mesure 64 n'a plus que cet accord et le La4 du lead (la mesure amincie, contrainte 2).

```pattern notes "Squelette" bars=8 grid=4 octave=4 key="D major" role=lead
A4 - - - | - - - - | D5 - - - | - - - - | F#5 - - - | - - - - | E5 - - - | A4 - - - |
```
Génération 11 (mélodie : réduction, F4 « le thème réduit à ses notes-squelette ») : les cinq notes longues du crochet (La, Ré, Fa#, Mi, La), en rondes ; le dernier La4 (mesure 64) est tenu à travers la coupure et jeté dans l'écho. Cinq notes, le sommet Fa#5 une fois.

```pattern notes "Arp E" bars=4 grid=8 octave=4 key="F major" role=arp
F4 A4 C5 F5 F4 A4 C5 F5 | D4 F4 A4 D5 D4 F4 A4 D5 | Bb3 D4 F4 Bb4 Bb3 D4 F4 Bb4 | C4 F4 G4 C5 C4 F4 G4 C5 |
```
Génération 12 (tonalité, move 2) : Arp A soulevé de +3 : F, Dm, B♭, Csus4.

```pattern notes "Bass E" bars=4 grid=8 octave=1 key="F major" role=bass
F2 - - - . F2 - . | D2 - - - . D2 - . | Bb1 - - - . Bb1 - . | C2 - - - . C2 - . |
```
Génération 13 (tonalité) : Bass A soulevée de +3.

```pattern notes "Pad E" bars=4 grid=4 octave=3 key="F major" role=pad
F3+A3+C4+E4 - - - | D3+F3+A3+C4 - - - | F3+Bb3+D4+A4 - - - | G3+C4+F4 - - - |
```
Génération 14 (tonalité) : Fmaj7, Dm7, B♭maj7 (Fa en bas, la septième La en haut), Csus4, une mesure chacun.

```pattern notes "Hook F" bars=8 grid=8 octave=4 key="F major" role=lead
C5 - F5 - A5 - - G5 | - - - - F5 - D5 - | C5 - F5 - A5 - - Bb5 | C6 - - - - - . . | C5 - F5 - A5 - - G5 | - - - - F5 - D5 - | C5 - D5 - F5 - G5 - | C5 - - - - - - - |
```
Génération 15 (tonalité) : le crochet soulevé de +3, inchangé sinon : sommet Do6 une fois (mesure 4).

```pattern notes "Canon" bars=10 grid=8 octave=4 key="F major" role=lead
. . . . . . . . | . . . . . . . . | C5 - F5 - A5 - - G5 | - - - - F5 - D5 - | C5 - F5 - A5 - - Bb5 | C6 - - - - - . . | C5 - F5 - A5 - - G5 | - - - - F5 - D5 - | C5 - D5 - F5 - G5 - | C5 - - - - - - - |
```
Génération 16 (forme, F4 « le thème en canon avec lui-même deux mesures plus tard ») : Hook F précédé de deux mesures de silence, sur la piste Canon (sinus doux) : la seconde voix entre à 67 et finit à 74. Sur le cycle E chaque note du canon reste ton d'accord ou couleur (9e, 13e, maj7).

```pattern notes "Chant" bars=8 grid=8 octave=5 key="F major" role=lead
C5 - - - - - A5 - | F5 - - - - - - - | D5 - - - F5 - G5 - | - - - - - - - - | A5 - - - C6 - - - | A5 - - - - - F5 - | D5 - - - - - F5 - | G5 - - - - - - - |
```
Génération 17 (mélodie : la seule phrase neuve, profil « une longue phrase chantée dans le dernier tiers ») : treize notes longues sur huit mesures, de Do5 à **Do6** (une fois, mesure 5, temps 3), qui finit sur Sol5 : la quinte du Csus4, suspendue.

```pattern notes "Pad fin" bars=4 grid=4 octave=3 key="F major" role=pad
G3+C4+F4 - - - | - - - - | - - - - | - - - - |
```
Génération 18 (forme) : le Csus4 tenu quatre mesures sous les quatre dernières mesures du crochet : la fin non résolue (le détail changé du retour).

## Arrangement

Form: F4 Thème et variations

```arrangement tempo=108
section Theme       1-16 : Beat A [from=9], Bass A, Arp A, Hook
section Variation1 17-32 : Beat B, Bass B, Arp B, Pad B, Hook
section Variation2 33-48 : Beat A, Hook basse, Pad C, Tenues
section Variation3 49-64 : Beat A [to=64], Bass D [to=64], Pad D1 [to=57], Pad D2 [from=57], Squelette
section Variation4 65-80 : Beat A, Bass E, Arp E, Pad E, Hook F [to=73], Canon [to=75], Chant [from=73]
section Retour     81-96 : Beat A [to=93], Bass E [to=93], Arp E [to=93], Pad E [to=93], Pad fin [from=93], Hook F
```

Cycles par section : **Thème** Dmaj7 – Bm7 – Gmaj7 – Asus4 (impliqué, sans nappe) ; **Variation 1** Gmaj7 – Asus2 – Bm7 – F#m7 ; **Variation 2** Bm9 – Em7 – Gmaj7 – F#m7 (Si mineur, deux mesures par accord) ; **Variation 3** Gmaj7/D – Asus4/D – Bm7/D – Dmaj7 puis Gmaj7 – Asus4 tenu (pédale de Ré) ; **Variation 4 et Retour** Fmaj7 – Dm7 – B♭maj7 – Csus4 (Fa majeur). Cinq images différentes, chacune ancrée à la précédente.

Coutures et événements uniques :
- **1.1** : crochet, arpège fermé (couloir 1) et basse, sans accords ni batterie ; **9.1** : la batterie entre (couture grossière : une partie de plus au milieu de la section, pas à sa frontière) ;
- **17.1** : la nappe entre avec le cycle B sous le crochet inchangé (signature 2) ; la batterie passe en demi-temps ; le crochet, lui, traverse la ligne sans changer : c'est la couture ;
- **33.1** : **échange de rôles** (événement unique 1, structurel) : le crochet descend dans la basse, le lead tient les fondamentales, l'arpège se tait ; la nappe passe à la relative, deux mesures par accord ;
- **48.3–48.4** : **bégaiement de Hiccup sur la batterie** (événement unique 2, couloir 3), le seul roulement du morceau, juste avant la variation 3 ;
- **49.1** : la basse se pose sur le Ré et n'en bouge plus (pédale) ; le crochet réduit à ses rondes ; la nappe s'ouvre sur seize mesures (couloir 2) ;
- **59–64** : Asus4 tenu six mesures sans résolution (événement unique 3) ; **64** : batterie et basse coupées, il ne reste que le sus de la nappe et le La4 du lead jeté dans l'écho (couloir 4) : **la mesure amincie, une note tenue à travers la coupure** ;
- **65.1** : **montée de +3** (événement unique 4, structurel) : Fmaj7 avec tout le monde, la basse bouge enfin (sur le Fa) ; **67.1** : le canon entre ; **73.1** : le crochet laisse la place au chant pendant que le canon finit à 74 ;
- **81.1** : retour du crochet soulevé sur le cycle E, le chant s'arrête : le thème comme à la mesure 1, mais avec la nappe ;
- **93.1** : batterie, basse, arpège et cycle coupés ; **93–96** : le crochet seul sur le Csus4 tenu (événement unique 5), **96** : fin non résolue sur le Do5 tenu.

Longueurs : six fois 16 : toutes multiples de 4.

## Automation

```automation "Arpège s'ouvre" part="Arp A" param=cutoff curve=ease-in
1.1 30, 16.4 100
```
Coupure du Filter de l'arpège (30 ≈ 500 Hz, 100 ≈ 4 kHz) : fermée au départ, elle s'ouvre lentement puis vite sur toute l'intro sans accords ; à 17 l'arpège est ouvert et le reste.

```automation "Nappe monte" part="Pad D1" param=cutoff curve=ease-in
49.1 40, 64.4 120
```
Coupure du Filter de la nappe sur la variation 3 (40 ≈ 800 Hz, 120 ≈ 8 kHz) : la « nouvelle texture » de F4 est le même accordage qui se dévoile ; en Faulk une rampe linéaire sur le même couloir, et la nappe reste ouverte sur le sommet.

```automation "Bégaiement" part="Beat A" cc=17 curve=step
33.1 0, 48.3 127, 49.1 0
```
Mélange de Hiccup sur la batterie (cc 17 : 0 = sec, 127 = 100 %) : à zéro tout le morceau, 100 % sur les deux derniers temps de 48 : le bégaiement du profil, une fois.

```automation "Écho jeté" part="Squelette" param=delay curve=step
49.1 25, 64.1 110, 65.1 25
```
Mélange de l'Echo du lead (25 ≈ 20 %, 110 ≈ 85 %) : jeté sur le La4 tenu de la mesure 64, ramené au premier temps de 65. Dans Faulk, un seul couloir sur la piste lead porte aussi 1.1 à 25.

## Notes de finition

- **Sons** : Bass saw release 150 ms, Filter passe-bas 250 Hz résonance 10 % ; Arp carré release 60 ms, Filter automatisé résonance 25 %, Echo 1/8 retour 30 % mélange 20 % ; Pad saw attaque 300 release 800, Filter 800 Hz automatisé, Bloom Ensemble, Reverb 35 % ; Lead triangle attaque 15 release 400, Bloom Vibrato au tempo 1/8 profondeur 20 %, Echo 1/8 mélange automatisé ; Canon sinus attaque 30 release 500, Reverb 40 % ; Drums par défaut + Hiccup (mélange 0, automatisé) ; master Compressor −14 dB 3:1 RMS mélange 70 %, Ceiling −0,5 dB.
- **Niveaux** : Drums 0, Bass −3, Arp −9, Pad −12, Lead −6, Canon −10, master −1 dB.
- **Humaniser** : rien : le vibrato de Bloom et les filtres qui s'ouvrent font le vivant ; pas de swing (absent).
- **Laissé à l'oreille** : le niveau du canon contre le lead ; la profondeur du vibrato ; la résonance de la nappe au bout de la montée (si elle siffle, 15 %).
- **Version 2** : un pompage de sidechain sur la nappe quand Faulk en aura un ; une montée de bruit filtré sous 61–64 ; le swing des charleys ; une dissolution de huit mesures après 96 au lieu de la coupure à 93.

## Vérification

Sortie de `sheet_tool.py check`, copiée telle quelle dans `check.txt` (à côté de cette fiche) ; le rendu MIDI est `maree.mid`, livré et jamais importé dans Faulk.
