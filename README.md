# Page style Wikipédia

## Contexte

Wikipédia est l'un des sites les plus visités au monde. Et pourtant, sa structure de base est très simple : des titres, des paragraphes, des listes, des images et des liens.

Dans cet exercice, vous allez recréer une page qui ressemble à un article Wikipédia, en utilisant uniquement du HTML.

Pas de CSS pour le moment : le navigateur applique ses styles par défaut, et c'est très bien ainsi !

Choisissez un sujet qui vous plaît : un animal, une ville, un sport, un personnage historique, une recette...

Chaque niveau complète la page un peu plus.

---

## Niveau 0 — Mise en place

**Objectif** : créer les fichiers et vérifier que tout fonctionne.

**Spécifications** :

1. Créez un dossier nommé `wikipedia` (sur votre bureau, ou dans vos documents, ...).
2. Dans ce dossier, créez un fichier nommé `index.html`.
3. Ouvrez ce fichier dans VSCode.
4. Copiez-collez le boilerplate vu en cours.
5. Dans le `<head>`, donnez un titre à votre page (le nom de votre sujet).
6. Dans le `<body>`, écrivez un simple paragraphe pour tester.
7. Sauvegardez (`Ctrl + S` ou `Cmd + S`), puis ouvrez le fichier dans votre navigateur.

> ℹ️ Rien ne s'affiche ? Vérifiez que vos balises sont bien **ouvertes et fermées**, et que le fichier est bien enregistré avec l'extension `.html`.

---

## Niveau 1 — Socle

**Objectif** : poser la structure principale de l'article.

**Spécifications** :

1. Remplacez votre paragraphe de test par un **grand titre** avec le nom de votre sujet.
2. Sous ce titre, écrivez **un ou deux paragraphes d'introduction** : qui ou quoi est ce sujet ? Quelques phrases suffisent.
3. Mettez en valeur **un ou deux mots importants** dans vos paragraphes.

> ℹ️ Sur Wikipédia, le titre du sujet est mis en gras dans le premier paragraphe. Cherchez quelle balise HTML permet de faire ça !

---

## Niveau 2 — Consolidation

**Objectif** : structurer l'article en plusieurs sections.

**Spécifications** :

1. Ajoutez **au moins deux sections** à votre article, chacune avec :
   - un **sous-titre** (une balise de titre moins importante que le grand titre),
   - un ou deux **paragraphes** de contenu.
2. Dans au moins une section, ajoutez une **liste à puces** ou une **liste numérotée** selon ce qui est le plus adapté au contenu.

> ℹ️ Quand utilise-t-on une liste à puces ? Quand utilise-t-on une liste numérotée ? C'est une question de sens, pas de préférence.

---

## Niveau 3 — Extension

**Objectif** : ajouter des images et des liens externes.

**Spécifications** :

1. Ajoutez **au moins une image** dans votre article.
   - Elle peut venir d'internet (copiez l'adresse de l'image).
   - Elle doit avoir une description alternative.
   - Elle doit avoir un titre informatif.
2. Dans votre article, ajoutez **au moins un lien** qui pointe vers une page extérieure (par exemple la vraie page Wikipédia de votre sujet).

> ℹ️ Pour récupérer l'adresse d'une image sur le web : clic droit sur l'image → "Copier l'adresse de l'image". Attention : cette adresse doit commencer par `https://` !

> ℹ️ Pour qu'un lien s'ouvre dans un nouvel onglet, cherchez l'attribut `target` sur [MDN Web Docs](https://developer.mozilla.org/fr/docs/Web/HTML/Element/a). Ce n'est pas encore vu en cours, mais c'est une bonne occasion d'explorer !

---

## Niveau 4 — Challenge

**Objectif** : ajouter un sommaire cliquable, comme sur Wikipédia.

Sur Wikipédia, il y a toujours un sommaire en haut de page qui permet de naviguer directement vers une section.

**Spécifications** :

1. Ajoutez une section **"Sommaire"** en haut de votre page, juste après l'introduction.
2. Cette section doit contenir une **liste numérotée** avec le nom de chacune de vos sections.
3. Chaque élément de cette liste doit être un **lien** qui amène directement à la section correspondante dans la page.

> ℹ️ Ce type de lien s'appelle une **ancre**. Pour créer une ancre :
> - donnez un `id` à votre balise de titre (par exemple `id="description"`),
> - puis créez un lien dont l'adresse commence par `#` (par exemple `href="#description"`).
>
> Vous n'avez pas encore vu ça en cours : cherchez des exemples sur [MDN Web Docs](https://developer.mozilla.org/fr/docs/Web/HTML/Element/a#lier_à_un_élément_sur_la_même_page) ou demandez !

---

## Niveau 5 — Exploration libre

**Objectif** : aller plus loin et peaufiner la page.

Voici des idées à explorer librement :

- Ajoutez une section **"Voir aussi"** en bas de page avec des liens vers des articles liés.
- Ajoutez un lien **"Retour en haut de page"** tout en bas, qui renvoie vers le titre principal.
- Utilisez des **sous-sous-titres** (`h3`) dans une section pour la découper davantage.
- Ajoutez une **deuxième image** dans une autre section.
- Essayez d'utiliser la balise `<em>` pour mettre un mot en italique dans un paragraphe.

> ℹ️ [MDN Web Docs](https://developer.mozilla.org/fr/) est votre meilleure ressource pour explorer de nouvelles balises. Cherchez, testez, observez !

---

## Bonus optionnels

Ces idées vont au-delà du cours. Elles sont là pour les plus curieux, sans obligation :

- **Commentaires HTML** : ajoutez des commentaires dans votre code pour indiquer où commence et où finit chaque section (par exemple `<!-- Section : Description -->`).
- **Validation** : copiez votre code dans le [validateur HTML du W3C](https://validator.w3.org/#validate_by_input) et corrigez les erreurs signalées.
- **Bonnes pratiques** : vérifiez que toutes vos images ont bien un attribut `alt` rempli, et que tous vos liens ont bien un attribut `title`.
