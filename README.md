# DÉKORA COSMÉTIQUES — Front Office + Back Office

Prototype marketplace DÉKORA avec un Front Office public et un Back Office administrateur dans le même dépôt.

## Structure

```text
DEKORA/
├── index.html              # Front Office — boutique
├── admin/
│   ├── login.html          # Connexion administrateur
│   └── index.html          # Back Office — gestion du site
├── .nojekyll
├── .gitignore
└── README.md
```

## Fonctions CMS V13

- Ajout / modification / suppression définitive des produits.
- Publication / brouillon des produits.
- Modification des prix, promotions, stock, SKU, catégorie et image produit.
- Création / modification / suppression des catégories.
- Création / modification / publication / suppression des articles et conseils.
- Changement de l'image Hero par URL ou import local.
- Changement de la couleur de la topbarre et de la couleur de son texte.
- Gestion des textes du Hero, navigation, blocs de confiance, catégories, routine, suivi, conseils, contact, newsletter et footer.
- Les changements CMS sont écrits dans `localStorage` et reflétés sur le Front Office dans le même navigateur/origine.
- Responsive desktop / tablette / mobile.

## Important

Cette version reste un prototype HTML : les données CMS sont stockées dans le navigateur (`localStorage`). Pour que les modifications de l'administrateur soient réellement partagées entre tous les visiteurs et appareils, l'étape suivante est le branchement Firebase (Firestore + Storage + Auth).

## GitHub Pages

La publication doit utiliser la branche `main` et le dossier `/(root)`.

Front Office : `https://ebbl237.github.io/Dekoracosmetique/`

Administration : `https://ebbl237.github.io/Dekoracosmetique/admin/login.html`


## V15.1 — CMS publication workflow consolidé
- Brouillon séparé de la version publiée
- Correction de la collecte CMS : les champs réels du formulaire sont utilisés, sans dépendance aux anciens identifiants V14
- Import logo et Hero fonctionnel dans le brouillon
- Prévisualisation de la boutique dans une iframe avant publication
- Validation explicite « Valider & publier »
- Confirmation visuelle après publication
- Gestion du logo, Hero, topbar, couleurs, navigation, visibilité et contenus
- Correction du détail des lignes de commande : affichage depuis `unitPrice`
- CA / finance excluent les commandes annulées ou remboursées
- Édition des promotions existantes ajoutée
- Diagnostic local des briques catalogue, favoris, panier, commandes, suivi, CMS, articles, promotions et catégories
- Aperçu d'une fiche produit avant enregistrement
- La version V15 reste un prototype local : localStorage/sessionStorage seront remplacés par Firebase pour la synchronisation multi-appareils.
