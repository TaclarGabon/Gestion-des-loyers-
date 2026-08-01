## V1.5.3.3 — correction initialisation Firebase

Correction de la variable Firebase Storage qui empêchait Firebase de devenir prêt.

# Gestion des loyers — V1.5.3.3

Correction de la connexion Firebase :
- fermeture immédiate de l’écran après authentification réussie ;
- conservation du mot de passe dans le champ en cas d’erreur ;
- affichage du motif Firebase précis ;
- interface Langley et stockage Interac inchangés.

# Gestion des loyers — V1.5.3 Firebase Storage

## Nouveautés Langley
- Historique en accordéon par année et par mois.
- Mortgage corrigé à 1 882,01 $.
- Copie Interac envoyée dans Firebase Storage.
- Renommage automatique : `Interac_Loyer_Riley_AAAA-MM_Reference.ext`.
- La copie reste visible après suppression du fichier local.

## Avant le premier test
Dans Firebase Console, active **Storage**, puis publie des règles autorisant uniquement les utilisateurs authentifiés :

```
rules_version = '2';
service firebase.storage {
  match /b/{bucket}/o {
    match /interac/{allPaths=**} {
      allow read, write: if request.auth != null;
    }
  }
}
```

Dépose `index.html` et le dossier `data` ensemble sur GitHub Pages.


## V1.5.3.3
- Accordéon Langley restauré dans le thème sombre validé.
- Cartes annuelles et mensuelles foncées, textes lisibles et badges Payé / En attente.
- Aucun changement apporté à Firebase, Firestore, Storage ou aux fichiers Excel.
