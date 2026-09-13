# DÉKORA — Marketplace & Cockpit Administration V14

Prototype statique avant Firebase.

## V14 — Studio système
Le back-office dispose maintenant d’une véritable console de configuration :
- identité DÉKORA et logo texte/image ;
- import d’un logo et aperçu ;
- couleurs globales (violet, corail, or, crème, texte) ;
- topbar et couleurs de topbar ;
- hero : sur-titre, titre, sous-titre, texte, boutons, image URL/import ;
- suppression explicite du logo image et de l’image Hero ;
- navigation éditable ;
- visibilité des sections : Hero, réassurance, catégories, boutique, routine, suivi, conseils, contact, newsletter, footer ;
- textes des sections principales et du footer ;
- aperçu visuel et indicateurs du catalogue ;
- mise en page responsive avec rail de commande, cartes séparées et prévention des chevauchements.

## V13 conservé
- gestion produits : création, modification, publication, suppression ;
- catégories et promotions ;
- articles & conseils : création, modification, publication/brouillon, suppression ;
- CMS contenu ;
- cockpit, finance, commandes, stocks, clients ;
- authentification admin locale.

## Données
Le prototype utilise `localStorage` pour partager les réglages entre storefront et back-office dans le même navigateur.
Firebase devra remplacer ce stockage local pour obtenir une configuration centralisée et partagée par tous les visiteurs.

## URLs GitHub Pages
- Boutique : https://ebbl237.github.io/Dekoracosmetique/
- Administration : https://ebbl237.github.io/Dekoracosmetique/admin/login.html
