# Template d'IG pour le training

Template d'Implementation Guide FHIR basé sur [ansforge/IG-modele](https://github.com/ansforge/IG-modele) (état du 2026-10-20), sans les workflows GitHub Actions ANS.

## Utilisation

1. Forker ce dépôt en **décochant** « Copy the main branch only » pour récupérer la branche `ig-template`.
2. Cloner votre fork et se placer sur la branche `ig-template`.
3. Installer [SUSHI](https://github.com/FHIR/sushi) : `npm install -g fsh-sushi`.
4. Adapter les placeholders `[code]` dans `sushi-config.yaml` (`id`, `canonical`) et `ig.ini`, ainsi que `name`, `title` et `description`.
5. Compiler : `sushi .`
6. Générer l'IG : `./_updatePublisher.sh` puis `./_genonce.sh` (Java requis).

Le résultat est dans `output/index.html`.

## Structure

* `sushi-config.yaml` : configuration de l'IG (pages, menu, dépendances).
* `input/fsh/` : artifacts FSH (profils, extensions, ValueSets, CodeSystems, exemples).
* `input/pagecontent/` : pages Markdown (à partir du niveau `###`).

Les tâches de la session sont communiquées pendant le training.
