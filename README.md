# Vol NR 2909

Le carnet de vol de Nell et Roméo.

## Mettre le site en ligne avec GitHub Pages

### ⚠️ À savoir avant

- Un site GitHub Pages est **public** : toute personne qui a le lien peut l'ouvrir. Même avec un dépôt privé (offre payante), le site reste public.
- Le site demande aux moteurs de recherche de ne pas l'indexer (`robots.txt` et balise `noindex`). Il ne sera donc pas trouvable sur Google, mais le lien n'est pas protégé par un mot de passe.
- Si tu crées un dépôt **public**, tout le monde peut aussi lire les fichiers sur github.com, photos comprises.
- Choisis un nom de dépôt discret (par ex. `nr2909`).

### Méthode simple (sans ligne de commande)

1. Va sur https://github.com/new
2. Nom du dépôt : `nr2909` (ou ce que tu veux). Visibilité : Public (obligatoire en gratuit pour Pages).
3. Clique **Create repository**.
4. Sur la page du dépôt, clique **uploading an existing file**.
5. Glisse **tout le contenu** de ce dossier : `index.html`, le dossier `img`, `.nojekyll`, `robots.txt`, `README.md`.
   - Le fichier `.nojekyll` est caché sous Windows : active « Éléments masqués » dans l'Explorateur (onglet Affichage) pour le voir. Il n'est pas indispensable, mais il évite des soucis.
6. Clique **Commit changes**.
7. Va dans **Settings → Pages**.
8. Dans **Build and deployment** : Source = **Deploy from a branch**, Branch = **main**, dossier **/ (root)**, puis **Save**.
9. Attends 1 à 2 minutes. L'adresse apparaît en haut de la page Settings → Pages :
   `https://TON-PSEUDO.github.io/nr2909/`

### Méthode en ligne de commande (avec Git)

Dans ce dossier :

```bash
git init -b main
git add .
git commit -m "Vol NR 2909"
git remote add origin https://github.com/TON-PSEUDO/nr2909.git
git push -u origin main
```

Puis active Pages comme aux étapes 7 et 8.

### Mettre à jour le site plus tard

Remplace `index.html` (et les photos si besoin) dans le dépôt, puis commit. Le site se met à jour tout seul en 1 à 2 minutes.

### Retirer le site

Settings → Pages → **Unpublish site**, ou supprime le dépôt (Settings → tout en bas → Delete this repository).
