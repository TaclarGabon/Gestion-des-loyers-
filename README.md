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
