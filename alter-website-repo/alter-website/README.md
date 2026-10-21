# Alter - site principal (alteralteralter.com)

Page d'accueil : vidéo de fond en rotation, logo et coordonnées.

- `index.html` : toute la page (HTML, CSS, JS). Liens de contact dans `CONTACT`, vidéos dans `BACKGROUNDS`.
- `videos/` : vidéos desktop (H.264, sans son). `videos/mobile/` : versions légères pour téléphone.
- `posters/` : image affichée en attendant la vidéo.
- `alter_logo_white.png` : logo.

Ajouter une vidéo : encoder en H.264 avec `-movflags +faststart` (sinon le navigateur ne la lit pas bien),
mettre le fichier dans `videos/` et `videos/mobile/`, créer son poster, puis ajouter une ligne dans `BACKGROUNDS`.

Hébergement : Netlify, projet `alterwebsite` (le `netlify.toml` à la racine du dépôt publie ce dossier, sans build).
