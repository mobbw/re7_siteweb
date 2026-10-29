# RE7 – Site de recettes de desserts

> *La gourmandise se partage !*

RE7 est une maquette de site web de recettes de desserts **dans le cadre d'un projet en développement web (très inspiré du site jow.fr).** Chaque recette est présentée de façon visuelle : pictogrammes pour le prix, la difficulté, le temps de préparation et les calories, liste d'ingrédients illustrée et étapes détaillées.

---

## Aperçu des pages

| Page | Fichier | Description |
|---|---|---|
| Accueil | `index.html` | Bannière, puis carrousel des recettes disponibles |
| Recette : Crêpes | `recette1.html` | Pictogrammes, ingrédients et étapes de la recette |
| Recette : Fondant au chocolat | `recette2.html` | Même structure que la page des crêpes |
| À propos | `apropos.html` | Présentation de l'équipe, de la mission et de la vision de RE7 |

Pages prévues : `contacts.html`, recherche, blog et connexion (les liens existent dans la navigation mais les pages ne sont pas encore créées).

---

## Technologies utilisées

- **HTML5** pour la structure des pages
- **CSS3** pour le style : flexbox, grid (header), `position: sticky`, `@media`
- **Bootstrap 6.0.0-alpha.1** (CSS + JS) pour le carrousel multi-images de la page d'accueil
- **Google Fonts** : Lato, Raleway, Short Stack

> ⚠️ Le carrousel de l'accueil utilise la version alpha de Bootstrap 6, car elle permet d'afficher plusieurs images à la fois. Cette version peut encore changer : ne pas la remplacer par la 5.3.3 sans adapter le carrousel.

---

## Structure du projet

```
Projet_re7/
├── index.html
├── recette1.html
├── recette2.html
├── apropos.html
├── style.css
├── README.md
└── assets/
    ├── Logo_RE7_avec_toque_de_chef.svg
    ├── banner.png
    ├── crepe.png, crepe2.png, gateau.png, macaron.png, cupcake.png, fondant.png
    ├── pictogrammes (prix, difficulté, temps, calories, nutri-score)
    ├── ingrédients (farine.svg, lait.svg, oeufs.svg, ...)
    └── photos de l'équipe
```

---

## Lancer le projet en local

Aucune installation n'est nécessaire.

1. Cloner le dépôt :
   ```bash
   git clone <url-du-depot>
   ```
2. Ouvrir le dossier dans un éditeur de code (par exemple VS Code).
3. Ouvrir `index.html` dans un navigateur, ou utiliser l'extension **Live Server** de VS Code pour un rechargement automatique.

Une connexion internet est nécessaire pour charger Bootstrap et les polices Google Fonts depuis leur CDN.

---

## Fonctionnalités

- Header **sticky** (toujours visible en haut de l'écran) avec le logo centré, et des liens de navigation à gauche et à droite
- Pages de recettes en **deux colonnes** (texte et image), qui s'empilent sur petit écran
- Image de la recette **sticky** à côté du contenu sur grand écran
- **Carrousel** de recettes sur la page d'accueil
- Bannière d'accueil avec image assombrie et texte superposé
- Effet de zoom au survol des images

---

## Conventions de travail (Git)

- Branche principale : `main`
- Faire un `git pull` avant de commencer à travailler, et un `git push` une fois les modifications validées.
- **Ne jamais créer de fichier dont le nom contient `< > : " / \ | ? *`.** Ces caractères sont interdits sous Windows et bloquent le `git pull` pour tous les membres de l'équipe sous cet OS.
- Éviter les noms de fichiers avec des espaces ou des accents dans `assets/`, pour que les chemins restent fiables.

---

## Pistes d'amélioration

- [ ] Créer les pages manquantes : contact, recherche, blog, connexion
- [ ] Ajouter les recettes des macarons et des cupcakes
- [ ] Rendre le header adaptatif sur mobile (le `@media` de `style.css` est vide)
- [ ] Uniformiser la version de Bootstrap entre les pages
- [ ] Ajouter des textes `alt` sur toutes les images (page À propos)
- [ ] Remplacer les titres `<title>Document</title>` par des titres explicites

---

## Équipe

| Rôle | Nom |
|---|---|
| Cofondatrice | Kenza FERCHICHI |
| Cofondateur | Endrit SHURDHANI |
| Cofondateur | Mathias WELMANT |

---

© 2026 RE7
