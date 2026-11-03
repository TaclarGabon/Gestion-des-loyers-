# Gestion des loyers V1.5.5.3 — Langley

Même interface que V1.5.5.2. Dans les mois déjà payés de Langley, boutons « Joindre / Remplacer la copie » et « Voir » pour archiver les preuves Interac dans Firestore (sous loyers/gestion-loyers-partagee/bordereaux_interac). Pas de modification des données de paiement.

Déploiement : extraire le ZIP puis remplacer index.html à la racine du dépôt GitHub Pages. Ne pas téléverser le ZIP lui-même comme index.html.

Test : utiliser une preuve masquée de moins de 3 Mo, vérifier « Voir » sur ordinateur puis téléphone. Les originaux bancaires non masqués ne doivent pas être archivés avant restriction des règles Firestore aux comptes autorisés.

La reconnaissance OCR n'est pas corrigée par cette version. Les copies Interac précédemment stockées via Firebase Storage ne sont pas automatiquement migrées.
