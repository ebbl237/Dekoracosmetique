# DÉKORA V12 — Auth Flow

## Boutique
Ouvrir `index.html`.

## Compte client
Depuis l'icône Compte ou le bouton « Mon compte » :
- Créer un compte
- Se connecter
- Modifier ses informations
- Consulter ses commandes
- Se déconnecter

Les comptes du prototype sont stockés localement dans le navigateur (`localStorage`).

## Administration
Accès séparé : `admin/login.html`.

Le lien « Accès administration » est également disponible dans le footer de la boutique et dans l'espace client.

L'admin utilise une session `sessionStorage` et redirige vers `admin/index.html` après authentification réussie. Les identifiants ne sont pas affichés dans le storefront.

## Important
Cette authentification est uniquement destinée au prototype HTML. Firebase Authentication remplacera la couche locale en production.
