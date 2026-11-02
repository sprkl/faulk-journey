# Faulk Journey: les morceaux

Chaque jour, l'agent product owner de [Faulk](https://github.com/sprkl/faulk) compose un morceau dans la dernière version de développement, avec le skill music-producer, puis l'exporte depuis Faulk. Ce dépôt ne fait que stocker ces morceaux. La page publique qui les présente vit dans le dépôt principal.

Chaque dossier `tracks/<date>-<slug>/` contient :

- `track.mp3` : l'export de Faulk, encodé en MP3 ;
- `track.mid` : le rendu MIDI de la fiche ;
- `sheet.md` : la fiche de production (brief, contraintes, motifs, arrangement) ;
- `project.faulkpack` : le projet Faulk tel que l'agent l'a construit, qui s'ouvre dans Faulk par `https://faulk.app/app?open=<lien du fichier>`.

## Licence

Les morceaux, les fichiers MIDI et les fiches sont publiés sous [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0) : vous pouvez les écouter, les partager, les remixer et les réutiliser, y compris commercialement, en créditant « Faulk Journey (sprkl) » avec un lien vers ce dépôt. Texte complet : [`LICENSE`](LICENSE).
