# TEKKIL — Politique de confidentialité

Contenu source de la politique de confidentialité de **TEKKIL** (application de
préparation aux concours au Sénégal, éditée par K-Edtech), maintenu dans
[`index.md`](./index.md) — pensé pour être publié tel quel via **GitHub Pages**
(repo minimal, un seul fichier Markdown à la racine).

Ce document est requis publiquement par les stores mobiles (Google Play / App Store) et
par le RGPD/la loi sénégalaise sur la protection des données personnelles (droit d'accès,
de rectification et de suppression — contact : `ibrahimadev6@k-edtech.com`).

## Statut — source de vérité

Ce repo (`index.md`) est la **source de vérité** du texte légal. Il existe deux autres
copies, tenues manuellement synchronisées sur son contenu à chaque mise à jour :

1. `TEKKIL_Landing_Page/app/privacy/page.tsx` — page complète servie sur
   `https://tekkil.sn/privacy` (l'URL référencée dans `tekkil-mobile/PLAY_STORE.md`).
   `TEKKIL_Landing_Page/components/sections/Privacy.tsx` n'en est qu'un résumé en 5
   points sur la page d'accueil, avec un lien vers la page complète — ce n'est pas une
   troisième version divergente.
2. `tekkil-mobile/lib/features/profile/presentation/pages/privacy_policy_page.dart` —
   texte affiché directement dans l'app, adapté au format mobile (listes à puces plutôt
   que tableaux) mais couvrant les mêmes 10 sections.

Synchronisé le 31 juillet 2026 : email de contact unifié (`ibrahimadev6@k-edtech.com`)
et date de dernière mise à jour alignée (5 mai 2026) sur les trois copies.

## Mettre à jour le contenu

1. Éditer [`index.md`](./index.md)
2. Mettre à jour la ligne « Dernière mise à jour : [date] » en tête de fichier
3. Répercuter le changement dans `TEKKIL_Landing_Page` et/ou `tekkil-mobile` selon ce qui
   est décidé au point ci-dessus
