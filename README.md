# Music’All 🎵

Application web autonome d'éducation musicale pour collégiens (6e à 3e), pensée pour un usage simple en SEGPA.

## Mise en ligne sur GitHub Pages

1. Créer un dépôt GitHub, par exemple `music-all`.
2. Décompresser l'archive et déposer `index.html`, `style.css`, `app.js` et `README.md` à la racine du dépôt.
3. Dans GitHub : **Settings → Pages**.
4. Dans **Build and deployment**, choisir **Deploy from a branch**.
5. Sélectionner `main` et `/ (root)`, puis **Save**.
6. Après quelques instants, GitHub affiche l'adresse publique de l'application.

## Fonctionnalités

- Accueil et navigation par niveau (6e, 5e, 4e, 3e).
- Leçons courtes avec une partie « Ce qu'il faut retenir ».
- Exercices à choix multiples, questions mélangées aléatoirement.
- Correction immédiate et explication de la bonne réponse.
- Récompenses : 2 notes par bonne réponse et 3 notes bonus en cas de sans-faute.
- Parcours transversal avec 10 questions tirées au hasard.
- Boutique virtuelle avec quatre bonus personnels : joker, choix musical, personnalisation et indice.
- Sauvegarde locale avec `localStorage`.

## Personnaliser les contenus

Ouvrir `app.js` :
- `lessons` contient les leçons et les questions de chaque niveau.
- `journeyQuestions` contient les questions du parcours transversal.
- `shopItems` contient les quatre bonus personnels, leur description et leur coût.

Chaque leçon comporte `title`, `emoji`, `summary`, `content`, `remember` et `questions`.
Une question est écrite sous la forme :
`["Question", ["Réponse A", "Réponse B", "Réponse C"], indexDeLaBonneRéponse]`

## Important : fonctionnement des données

Cette version ne demande aucun compte et n'envoie aucune donnée sur un serveur. Les points, résultats et échanges sont enregistrés dans le navigateur de l'appareil utilisé. Ils ne sont donc pas automatiquement synchronisés entre plusieurs appareils ou navigateurs. Si les élèves partagent un même ordinateur ou navigateur, leurs points peuvent être partagés : prévoir idéalement un appareil ou un profil navigateur par élève, ou faire évoluer l'application avec un système d'identification.

## Cadre pédagogique

Les thèmes proposés constituent une base de départ à adapter à la progression réellement suivie dans la classe. Les programmes officiels d'éducation musicale organisent les apprentissages autour de la production et de la perception, avec des compétences telles que chanter et interpréter, écouter et comparer, explorer et créer, échanger et partager. Les thèmes ne constituent pas une progression annuelle imposée.

Références :
- [Éduscol – Éducation musicale cycles 2 et 3](https://eduscol.education.gouv.fr/4737/ressources-d-accompagnement-des-enseignements-en-education-musicale-aux-cycles-2-et-3)
- [Éduscol – Ressources d'accompagnement du cycle 4](https://eduscol.education.gouv.fr/5721/ressources-d-accompagnement-du-programme-d-education-musicale-au-cycle-4)
