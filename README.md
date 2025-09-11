# Ridgee Production — site multipage (GitHub Pages)

## Pages
- `/` Accueil (hero vidéo + CTA)
- `/services.html`
- `/references.html` (avec 2 vidéos)
- `/artistes.html`
- `/a-propos.html` (photo Sabri)
- `/contact.html` (Formspree)

## Déploiement GitHub Pages
1. Crée un dépôt **public** et ajoute tous les fichiers en respectant l’arborescence.
2. Dans **Settings → Pages → Build and deployment** :
   - Source: **Deploy from a branch**
   - Branch: **main** / **root**
3. Domaine :
   - Dans le repo, garde le fichier `CNAME` avec `ridgeeproduction.com`.
   - Sur **OVH** (Zone DNS) :
     - **A** @ → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
     - **CNAME** **www** → `sabrilabonnevoix.github.io.`  
       (supprime l’entrée TXT `3|welcome` sur `www` si elle existe)
4. Retourne dans **Settings → Pages**, mets **ridgeeproduction.com** dans *Custom domain* puis **Enforce HTTPS**.

## Formspree
Crée un formulaire sur Formspree et remplace `your-form-id` dans `contact.html`.
