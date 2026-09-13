# DÉKORA — Audit global final V15.1

## Statut
Candidat GitHub-ready sous réserve d'un test manuel de parcours dans un navigateur avant publication.

## Corrections appliquées
- Consolidation du workflow CMS : brouillon → aperçu → validation → publication.
- Suppression des dépendances V14 cassées dans la collecte V15.
- Ajout de contrôles réels pour logo, signature, couleurs, topbar, visibilité et imports logo/Hero.
- L'import Hero utilise le vrai champ existant `heroImageFileV13` comme contrôle historique et le nouveau contrôle V15.1 `v151HeroFile`.
- Correction du détail commande : `unitPrice` est utilisé pour calculer/afficher les lignes.
- Correction du CA/finance : commandes annulées et remboursées exclues du CA commercial.
- Ajout de la modification des promotions existantes.
- Diagnostic V15.1 ajouté au back-office.

## Vérifications statiques
- JavaScript : 3 blocs admin + 7 blocs storefront parsés avec `new Function` sans erreur.
- Aucune référence aux identifiants DOM V14 cassés dans le bloc V15.1.
- Présence des fonctions/stockages storefront : favoris, panier, commandes, suivi.
- Présence du bridge d'aperçu `DEKORA_V15_PREVIEW` / `DEKORA_V15_READY`.

## Limites avant Firebase
- Authentification admin encore locale : prototype uniquement.
- CMS, catalogue, commandes et session reposent encore sur localStorage/sessionStorage.
- Paiement Mobile Money reste simulé dans le prototype HTML.
- La synchronisation multi-appareils n'est pas garantie avant Firebase.
- Les modifications catalogue/éditorial existantes sont encore enregistrées directement côté prototype ; le workflow transactionnel complet de publication multi-entités sera finalisé dans Firebase (Firestore + Storage + Auth).

## Séquence recommandée
1. Test manuel V15.1 sur PC, tablette et mobile.
2. Publication de la version V15.1 sur GitHub Pages.
3. Smoke test public + admin sur GitHub Pages.
4. Mise en place Firebase Auth, Firestore et Storage.
5. Migration des données et remplacement progressif du localStorage/sessionStorage.
6. Tests de sécurité, règles Firestore/Storage, commandes et paiements réels.
