# DÉKORA COSMÉTIQUES — Front Office + Back Office

## Structure GitHub Pages

```text
DEKORA/
├── index.html              # Front Office — site vitrine / boutique
├── admin/
│   ├── login.html          # Connexion administrateur
│   └── index.html          # Back Office — gestion du site
├── .nojekyll
└── README.md
```

Le fichier `index.html` doit impérativement être à la racine du repository pour que GitHub Pages serve le Front Office comme page d'accueil.

## URLs GitHub Pages

- Front Office: `/`
- Connexion Admin: `/admin/login.html`
- Back Office: `/admin/index.html`

Le Back Office fait partie du même site et pilote les données du Front Office dans le prototype via localStorage.
