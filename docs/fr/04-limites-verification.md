# 4. Limites et vérification

Ce parcours décrit le médiateur EVC, ses sous-comptes, ses autorisations et ses contrôles différés.
Il ne constitue ni un audit de sécurité ni une validation économique des coffres qui l'utilisent.
La sûreté réelle dépend des contrôleurs, des collatéraux et de leurs fonctions de rappel.
Une intégration doit traiter avec prudence les appels imbriqués, les opérateurs et l'identité propagée par le contexte.
Les états intermédiaires peuvent être volontairement non vérifiés tant que la transaction n'est pas terminée.
Il faut donc raisonner sur l'état final et sur toutes les vérifications planifiées par le connecteur.
Les interfaces et implémentations du dossier src donnent le périmètre exact décrit ici.
Pour vérifier le comportement, consulter les scénarios du dossier test et leurs cas de contrôle différé.
Aucune installation, compilation ou exécution de test n'a été réalisée pour ce parcours documentaire.
