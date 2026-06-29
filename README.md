# Algeria's Keys

Site vitrine de **Algeria's Keys**, la plateforme d'investissement immobilier pour la diaspora algérienne.
Baseline : *Investir aujourd'hui, bâtir demain.*

Site statique (HTML/CSS/JS, sans dépendance ni build), prêt pour **GitHub Pages**.

## Structure
```
.
├── index.html
├── .nojekyll
└── assets/
    ├── logo.png              (logo sur fond clair)
    ├── logo_transparent.png  (logo sur fond sombre, ex. footer)
    ├── favicon.png
    └── apple-touch-icon.png
```

## Mettre en ligne sur GitHub Pages

1. Crée un dépôt sur GitHub (ex. `algerias-keys`).
2. Pousse le contenu de ce dossier à la racine du dépôt :
   ```bash
   git init
   git add .
   git commit -m "Site Algeria's Keys"
   git branch -M main
   git remote add origin https://github.com/TON-COMPTE/algerias-keys.git
   git push -u origin main
   ```
3. Sur GitHub : **Settings → Pages → Source : Deploy from a branch → Branch : main / (root) → Save**.
4. Le site sera publié sous `https://TON-COMPTE.github.io/algerias-keys/` (compter 1 à 2 min).

## Nom de domaine personnalisé (optionnel)
Pour brancher `algeriaskeys.com` : ajoute un fichier `CNAME` à la racine contenant `algeriaskeys.com`, puis configure les enregistrements DNS chez ton hébergeur (mêmes principes que pour ridgeeproduction.com via OVH).

## À noter
- Le formulaire de liste d'attente fonctionne uniquement côté navigateur (validation + message). Pour collecter réellement les e-mails, branche un service comme Formspree, un Google Form, ou une fonction serverless.
- Les liens LinkedIn / Instagram et l'adresse e-mail sont des placeholders à remplacer.
