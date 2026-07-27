# Gestion des loyers — Okala & Langley

Application web mobile de suivi des loyers pour :

- **Okala**
  - Studio 1 — Sandrine Boutoto Pandza
  - Studio 2 — Nelly Loriane Engong Ngomo
- **Langley**
  - Condo B317 — Rylie Matson & Dustin Hurrell

## Fonctionnalités incluses

### Accueil

Deux grandes cartes :

- OKALA
- LANGLEY

### Okala

- dossier distinct pour chaque locataire ;
- historique de Sandrine ;
- reliquat actuel de Nelly séparé de l’historique informatif ;
- saisie de la référence et du montant des bordereaux UGB ;
- chaque reçu reste associé uniquement au bon locataire.

### Langley — Condo B317

- loyer mensuel : **2 495,00 $** ;
- caution de juillet 2026 : **2 495,00 $**, reçue par Interac ;
- saisie de la référence Interac, de la date, de l’expéditeur et du montant ;
- possibilité d’associer une capture ou un PDF comme preuve ;
- rappel mensuel séparé pour :
  - Mortgage RBC : **2 318,53 $**
  - Strata : **417,29 $**
- cases « payé / non payé » pour le mois en cours ;
- historique mensuel du loyer, du mortgage et du strata.

Les dépenses du propriétaire ne sont jamais additionnées au loyer.

## Données et confidentialité

Cette V1 fonctionne uniquement avec `localStorage`.

- Les informations saisies restent dans le navigateur de l’appareil utilisé.
- Les fichiers choisis ne sont pas téléversés sur Internet.
- Seul leur nom est enregistré localement.
- Une suppression des données du navigateur effacera les informations enregistrées.

Pour un véritable stockage multi-appareils et la conservation des images, il faudra connecter Firebase Authentication, Firestore et Firebase Storage dans une version ultérieure.

## Mise en ligne sur GitHub Pages

1. Créer un nouveau dépôt GitHub.
2. Importer tous les fichiers de ce dossier à la racine du dépôt.
3. Ouvrir **Settings**.
4. Ouvrir **Pages**.
5. Dans **Build and deployment**, sélectionner :
   - Source : `Deploy from a branch`
   - Branch : `main`
   - Folder : `/root`
6. Enregistrer.
7. Attendre une à trois minutes, puis ouvrir l’adresse GitHub Pages affichée.

## Structure

```text
gestion-loyers-github-v1/
├── index.html
├── styles.css
├── app.js
├── README.md
├── .gitignore
├── assets/
│   └── README.md
└── data/
    └── initial-data.json
```

## Version

V1.0 — juillet 2026
