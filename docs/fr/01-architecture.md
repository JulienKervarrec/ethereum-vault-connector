# 1. Architecture du connecteur EVC

L'Ethereum Vault Connector, ou EVC, relie des comptes utilisateurs à plusieurs coffres compatibles.
Le contrat central sert de médiateur : il reçoit les appels, suit leur contexte et délègue l'action au coffre visé.
Un compte peut activer un contrôleur qui représente sa dette auprès d'un coffre.
Il peut aussi déclarer des collatéraux que le contrôleur consultera pendant ses vérifications.
Le connecteur ne définit pas la logique financière d'un coffre : chaque intégration garde ses propres règles.
Cette séparation permet à plusieurs modèles de prêt de partager la même couche de coordination.
Les interfaces du dossier src décrivent les attentes entre EVC, comptes, collatéraux et contrôleurs.
La sécurité dépend donc autant du connecteur que des coffres qui interprètent son contexte.

[Chapitre suivant : comptes, collatéraux et contrôleurs](02-comptes-controleurs.md)
