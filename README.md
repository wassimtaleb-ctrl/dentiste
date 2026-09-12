# Démo — Cabinet dentaire Dr Charki Meryem

Cette démo est une application web statique en français. Elle utilise uniquement des données fictives et fonctionne sans base de données ni installation de dépendances.

Elle est également conçue comme une application mobile installable sur Android et iPhone.

## Lancer la démo le plus simplement possible

Ouvrez le dossier `dist`, puis double-cliquez sur `index.html`. La démo s’ouvre dans le navigateur.

Si le navigateur bloque certaines fonctions locales, ouvrez un terminal dans le projet et lancez :

```bash
python -m http.server 8000 --directory dist
```

Puis ouvrez `http://localhost:8000`.

## Profils de démonstration

- **Dr Charki Meryem** : accès complet, y compris dossier clinique, odontogramme, traitements et rapports.
- **Hanane** : accès administratif aux patients, rendez-vous et paiements. Les informations cliniques sont masquées.

Aucun mot de passe n’est nécessaire dans cette démo. Les ajouts de patients sont sauvegardés uniquement dans le navigateur et peuvent être effacés avec le bouton **Réinitialiser**.

## Publication sur GitHub Pages

Le workflow `.github/workflows/pages.yml` publie automatiquement le dossier `dist` sur GitHub Pages après chaque envoi sur la branche `main`.

Dans GitHub : **Settings → Pages → Source → GitHub Actions**. Ensuite, envoyez le projet sur la branche `main`.

## Installer sur téléphone

La version mobile doit être ouverte depuis son adresse GitHub Pages en HTTPS.

### Android

1. Ouvrir le site dans Chrome.
2. Appuyer sur **Installer l’application** si la proposition apparaît.
3. Sinon : menu ⋮ → **Ajouter à l’écran d’accueil**.

### iPhone

1. Ouvrir le site dans Safari.
2. Appuyer sur le bouton **Partager**.
3. Choisir **Sur l’écran d’accueil**.
4. Confirmer avec **Ajouter**.

L’application s’ouvrira ensuite depuis son icône **Cabinet Dr Charki**.

## Avertissement important

Cette version sert uniquement à une présentation. N’y saisissez aucune donnée réelle de patient. La version de production devra utiliser une authentification forte, une base de données sécurisée, des sauvegardes chiffrées, une journalisation d’audit et un hébergement validé pour les données de santé au Maroc.
