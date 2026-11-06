# Carnet : installer l'app sur ta tablette Android

L'app doit être en ligne sur une adresse en **https** pour que Chrome propose de l'installer.
GitHub Pages le fait gratuitement.

## 1. Mettre l'app en ligne (une seule fois, environ 5 min, depuis un ordi)

1. Connecte-toi sur https://github.com (ou crée un compte gratuit).
2. En haut à droite, clique sur **+** puis **New repository**.
   - Nom : `carnet`
   - Coche **Public**
   - Clique sur **Create repository**.
3. Sur la page du dépôt, clique sur le lien **uploading an existing file**.
4. Dézippe `carnet-pwa.zip` sur ton ordi. Ouvre le dossier et glisse **tout son contenu**
   (`index.html`, `sw.js`, `manifest.webmanifest`, les dossiers `icons` et `vendor`)
   dans la page GitHub, puis clique sur **Commit changes**.
   Les fichiers doivent être à la racine du dépôt, pas dans un sous-dossier `carnet-pwa`.
5. Va dans **Settings** → **Pages** (menu de gauche).
   - Source : **Deploy from a branch**
   - Branch : **main**, dossier **/ (root)**, puis **Save**.
6. Attends 1 à 2 minutes. Ton app est en ligne sur :
   `https://TON-PSEUDO.github.io/carnet/`

## 2. Installer sur la tablette

1. Ouvre cette adresse dans **Chrome** sur la tablette.
2. Menu **⋮** → **Installer l'application** (ou « Ajouter à l'écran d'accueil » → **Installer**).
3. L'icône **Carnet** apparaît avec tes autres apps. Elle s'ouvre en plein écran et marche **sans internet**.

## Important : tes notes

- Elles sont enregistrées **uniquement sur la tablette**, dans les données de l'app.
- Si tu désinstalles l'app ou si tu effaces les données de Chrome, elles disparaissent.
- Fais régulièrement une sauvegarde : dans la bibliothèque, bouton **⋯** → **Sauvegarder tous mes carnets…**.
  Tu peux l'envoyer directement sur Google Drive.
- Pour récupérer tes notes (sur une nouvelle tablette, par exemple) : **⋯** → **Restaurer une sauvegarde…**.

## Mettre à jour l'app plus tard

Remplace les fichiers modifiés sur GitHub, et change `carnet-v1` en `carnet-v2` dans `sw.js`.
La tablette récupère la nouvelle version à la prochaine ouverture avec internet.
Tes notes ne sont pas touchées.
