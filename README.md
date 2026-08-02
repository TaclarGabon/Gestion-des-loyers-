# Gestion des loyers — V1.5.3.8

Corrections Langley :
- Juin 2026 ajouté avec validation Mortgage et Strata uniquement.
- Ouverture d’un mois charge automatiquement les données de ce mois.
- Un mois non enregistré remet Interac, Mortgage et Strata à zéro.
- Juillet = caution ; août et suivants = loyers.


## V1.5.3.8
- Un mois ne passe en vert qu’après confirmation de Firestore.
- La sauvegarde du statut est effectuée avant l’envoi éventuel de la copie Interac.
- En cas d’échec Firebase, la validation est annulée et un message clair apparaît.
- Les mois enregistrés restent présents après actualisation et sur les autres appareils.


## Ajustements V1.5.3.8
- Suppression du bouton de réinitialisation en haut de l’application.
- Bouton « Valider le mois » déplacé tout en bas, après Mortgage et Strata.
