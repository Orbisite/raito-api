# leo-giraud-api

Dépôt **statique** (JSON + images) pour le portfolio de **Leo Giraud** — artiste 3D. Consommé par [`leo-giraud`](../leo-giraud).

## Fichiers

| Fichier | Rôle |
|---------|------|
| `content.json` | Textes, navigation, sections (hero, compétences, galerie, prestations, avis). |
| `theme.json` | Couleurs des blocs (`primary` / `secondary` / `neutral`). |
| `site.json` | Titre, meta SEO, favicon. |
| `img/` | Visuels (remplacer `placeholder.svg` par rendus / logo). |

## Publication

1. Créer le dépôt GitHub `leo-giraud-api` (ou sous l’org **Orbisite**).
2. Pousser ce dossier sur la branche `main`.
3. Dans `leo-giraud`, copier `.env.example` → `.env.local` et mettre les URLs **raw** vers ce dépôt, par ex.  
   `https://raw.githubusercontent.com/VOTRE_ORG/leo-giraud-api/main/content.json`  
   et `VITE_API_IMG_BASE` = `…/main/img`.

Les images référencées dans les JSON sont soit une **URL absolue**, soit un **nom de fichier** dans `img/`.
