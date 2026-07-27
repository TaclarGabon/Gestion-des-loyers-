# Gestion des loyers — V1.3.4 test lecture ciblée automatique

Cette version conserve l'historique complet de Sandrine et Nelly, les formulaires UGB et la partie Interac de Langley.

## Nouveau test

Dans les fiches Sandrine et Nelly :
1. choisir une photo JPG/PNG nette du bordereau ;
2. cliquer sur **Lire et préremplir** ;
3. vérifier le mois, la date, la référence et le montant ;
4. cliquer sur **Vérifier puis enregistrer**.

La lecture est effectuée dans le navigateur avec Tesseract.js. Une connexion Internet est nécessaire au premier chargement du lecteur. Pour cette version de test, les PDF ne sont pas analysés automatiquement : utiliser une photo ou une capture d'écran du bordereau.


## Ajustement UGB V1.3.4
La lecture cible désormais explicitement la zone supérieure droite pour le numéro et la date, ainsi que les libellés « Montant net » et « Montant du versement ». Le mois de démonstration reste Août 2026 et demeure modifiable avant validation.


## Lecture UGB V1.3.4
La lecture automatique utilise trois zones fixes du modèle UGB : référence en haut à droite, date immédiatement dessous et montant net. Pour un résultat fiable, la photo doit montrer le bordereau entier, de face, sans rotation importante et sans découper les bords. Le mois reste fixé à Août 2026 pour la démonstration et peut être modifié avant enregistrement.
