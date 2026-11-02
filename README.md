# Gestion des loyers V1.5.5.1 — Test archivage UGB

Conserve l’interface V1.5.5.0 et les paiements existants. Ajoute Voir et Joindre / Remplacer la copie pour les lignes UGB Sandrine et Nelly.

Stockage : Cloud Firestore, collection `bordereaux_ugb`, documents par locataire et mois, sous-collection `blocs` (base64). Pas Firebase Storage, pas de forfait Blaze requis pour ce mécanisme. Limite 3 Mo par pièce, formats JPG PNG WEBP PDF.

**IMPORTANT :** Fonctionnement conditionné par les règles de sécurité Firestore autorisant exclusivement les utilisateurs authentifiés habilités. Vérifier les règles AVANT d’archiver des pièces bancaires. Ne pas ouvrir cette collection publiquement. Un test depuis deux comptes/appareils est indispensable. Les données ne sont pas chiffrées de bout en bout.

Aucun fichier ancien n’est récupéré automatiquement, et le nom d’un fichier ne prouve pas son archivage. Le bouton Voir télécharge le document (sur mobile, il peut s’ouvrir dans le visualiseur de téléchargements).

Ne pas déployer sur main sans contrôle des règles et test ; utiliser une branche de test. Les modifications n’affectent pas les paiements.
