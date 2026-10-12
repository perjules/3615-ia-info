# 3615 IA / MinitelGPT — information publique

Deux pages statiques décrivant une installation personnelle de 3615 IA et le
traitement des données de son intégration Gmail. Aucun compte, message, identifiant
OAuth, clé d'API ou détail de réseau n'est inclus.

- `index.html` : présentation de l'application.
- `privacy.html` : notice de confidentialité, liée depuis l'accueil.
- `.nojekyll` : publication directe des fichiers HTML, sans moteur de site.

## Publication GitHub Pages

Dépôt : `perjules/3615-ia-info`, public, distinct du logiciel MinitelGPT.

1. Dans **Settings → Pages**, sélectionner **Deploy from a branch**, branche
   `main`, dossier **/(root)**, puis **Save**.
2. Attendre la fin de la publication et vérifier les deux URL avant de les
   déclarer dans Google Cloud :

   - Accueil : `https://perjules.github.io/3615-ia-info/`
   - Confidentialité : `https://perjules.github.io/3615-ia-info/privacy.html`

3. Dans **Google Auth Platform → Branding**, renseigner ces deux URL et le
   domaine autorisé `perjules.github.io`, puis enregistrer et retenter la
   publication depuis **Audience**. Si Google exige une preuve de propriété,
   utiliser Google Search Console pour le site réellement publié ; ne pas
   déclarer `github.com` comme un domaine que l'on possède.

Ces URL sont celles prévues par la configuration ci-dessus. La présence de ces
fichiers ne prouve pas que GitHub Pages est activé ou que Google accepte la
configuration : vérifier les pages publiées et l'état Google.

## Avant les essais Gmail réels

Dans le panneau d'administration du compte **Mistral Studio / API**, menu
**Privacy**, désactiver **Anonymous improvement data**. Le réglage API est
indépendant de celui de l'application de chat. Vérifier aussi les règles de
conservation applicables ; opt-out d'entraînement et Zero Data Retention sont
distincts. Le site ne prétend pas avoir vérifié ces réglages du compte.

Référence officielle :
https://help.mistral.ai/en/articles/455207-can-i-opt-out-of-my-input-or-output-data-being-used-for-training

Le logiciel et sa documentation d'installation restent dans
https://github.com/perjules/minitel-gpt.
