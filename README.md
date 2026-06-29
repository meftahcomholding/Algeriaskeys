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

## Recevoir les inscriptions par e-mail (sans afficher l'adresse)

Le formulaire de liste d'attente est prêt à envoyer les inscriptions vers une boîte e-mail
**sans que cette adresse n'apparaisse jamais sur le site**. Il utilise Formspree :

1. Crée un compte gratuit sur https://formspree.io
2. Crée un nouveau formulaire et indique comme adresse de réception : `meftahcomholding@gmail.com`
3. Formspree te donne un identifiant du type `https://formspree.io/f/abcdwxyz`
4. Dans `index.html`, remplace `VOTRE_ID_FORMSPREE` par ton identifiant
   (attribut `data-endpoint` de la balise `<form id="waitlist">`).

Tant que l'identifiant n'est pas renseigné, le formulaire reste en mode démonstration
(il affiche le message de confirmation sans rien envoyer). L'adresse Gmail reste stockée
chez Formspree et n'est pas visible dans le code source de la page.
