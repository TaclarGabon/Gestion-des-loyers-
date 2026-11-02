# Gestion des loyers V1.5.5.2 — correction archivage UGB

Correction ciblée : les copies UGB sont désormais enregistrées sous `loyers/gestion-loyers-partagee/bordereaux_ugb/{locataire_mois}/blocs/...`, chemin couvert par les règles Firestore communiquées. Aucun changement des paiements ni de la présentation.

Tester un seul bordereau d’octobre depuis le site hébergé avec connexion Firebase, puis vérifier sur un deuxième appareil. Ne pas archiver de documents bancaires non masqués tant que les règles Firestore n'ont pas été restreintes aux comptes autorisés. Les règles actuelles autorisent tout utilisateur authentifié du projet.

Limites : 3 Mo par fichier ; Firestore n’est pas un stockage documentaire idéal pour de nombreux fichiers ; test réel non encore effectué.
