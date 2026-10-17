# Prépa Attaché AAE 2027

Créé par **G. FUMONT** · FMT Collaboration.

Application web installable (PWA) de préparation au concours interne d'attaché d'administration de l'État (ministères de l'Éducation nationale et de l'Enseignement supérieur), session 2027.

- `index.html` : l'application.
- `free-data.js` : contenus en accès libre.
- `contenu.enc` : contenus de la version complète, chiffrés (AES-256-GCM) avec la clé du gestionnaire. L'application du gestionnaire les publie dans Firestore (collection `contenu`), lisible seulement pendant l'essai de 7 jours ou avec un abonnement actif.
- `firestore.rules` : règles de sécurité Firestore (comptes, abonnements, contenus, clés).
- `veille/` : une synthèse d'actualité par jour (`AAAA-MM-JJ.json`) et `index.json`, mise à jour chaque matin.
- `sw.js` : fonctionnement hors ligne.

Publication : GitHub Pages, branche `main`, dossier racine.
