# TEKKIL — Politique de confidentialité

Contenu source de la politique de confidentialité de **TEKKIL** (application de
préparation aux concours au Sénégal, éditée par K-Edtech), maintenu dans
[`index.md`](./index.md) — pensé pour être publié tel quel via **GitHub Pages**
(repo minimal, un seul fichier Markdown à la racine).

Ce document est requis publiquement par les stores mobiles (Google Play / App Store) et
par le RGPD/la loi sénégalaise sur la protection des données personnelles (droit d'accès,
de rectification et de suppression — contact : `privacy@tekkil.sn`).

## ⚠️ Constat à vérifier

L'URL publique référencée dans les checklists de soumission mobile
(`tekkil-mobile/PLAY_STORE.md`) est **`https://tekkil.sn/privacy`**. Or cette route est
actuellement servie par [`TEKKIL_Landing_Page`](../TEKKIL_Landing_Page)
(`app/privacy/page.tsx`, contenu dans `components/sections/Privacy.tsx`), **pas par ce
repo** — aucun fichier `CNAME` ni configuration Pages n'a été trouvé ici qui pointerait
vers `tekkil.sn/privacy`.

Il existe donc actuellement **trois copies** du même texte légal, avec un risque réel de
divergence dans le temps :
1. Ce repo (`tekkil-privacy/index.md`) — dernière mise à jour 5 mai 2026
2. `TEKKIL_Landing_Page/components/sections/Privacy.tsx` — la version réellement servie
   sur `tekkil.sn/privacy`
3. `tekkil-mobile/lib/features/profile/presentation/pages/privacy_policy_page.dart` —
   texte affiché directement dans l'app (contenu résumé en 7 sections, pas identique
   mot pour mot à ce fichier)

**À clarifier avec l'équipe** : soit ce repo est un brouillon/une ancienne version qui
peut être considéré comme obsolète au profit de `TEKKIL_Landing_Page`, soit c'est censé
être la source de vérité et `TEKKIL_Landing_Page` devrait aller chercher son contenu ici
au build. Dans tous les cas, une seule source de vérité devrait piloter les deux autres
copies pour éviter que la politique affichée diffère selon où l'utilisateur la consulte.

## Mettre à jour le contenu

1. Éditer [`index.md`](./index.md)
2. Mettre à jour la ligne « Dernière mise à jour : [date] » en tête de fichier
3. Répercuter le changement dans `TEKKIL_Landing_Page` et/ou `tekkil-mobile` selon ce qui
   est décidé au point ci-dessus
