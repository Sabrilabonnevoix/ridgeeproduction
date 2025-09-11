# Ridgee Production

Site officiel de **Ridgee Production** publié sur GitHub Pages.  
Domaine : [ridgeeproduction.com](https://ridgeeproduction.com)

## Déploiement

- `index.html` = page principale
- `CNAME` = fichier contenant :  
  ```
  ridgeeproduction.com
  ```

## Étapes pour connecter le domaine

1. Dans ton dépôt GitHub → **Settings → Pages** :
   - Source = Deploy from a branch
   - Branch = main / root

2. Le fichier `CNAME` est déjà inclus et contient :
   ```
   ridgeeproduction.com
   ```

3. Chez ton registrar (OVH, Gandi, etc.), configure les **DNS** :
   ```
   A   ridgeeproduction.com   185.199.108.153
   A   ridgeeproduction.com   185.199.109.153
   A   ridgeeproduction.com   185.199.110.153
   A   ridgeeproduction.com   185.199.111.153
   ```

   Et pour le sous-domaine **www** :
   ```
   CNAME   www   <ton-username>.github.io
   ```

4. Attends la propagation (quelques minutes à 24h).

5. Retourne dans **Settings → Pages** et active **Enforce HTTPS**.

Ton site sera alors accessible sur **https://ridgeeproduction.com**