# 3. Appels groupés et contrôles différés

Le connecteur peut exécuter une séquence d'appels dans un même contexte transactionnel.
Pendant cette séquence, un coffre peut demander que le contrôle d'un compte ou d'un coffre soit différé.
L'EVC mémorise alors les vérifications requises au lieu de les exécuter après chaque mouvement intermédiaire.
À la fin du contexte, il rappelle les contrôleurs et coffres concernés pour valider l'état final.
Cette mécanique autorise des opérations atomiques où un état transitoire serait temporairement insuffisant.
Un appel peut aussi être réalisé au nom d'un sous-compte en conservant l'identité originale dans le contexte.
Les fonctions de rappel doivent rejeter l'opération si la solvabilité ou l'invariant du coffre n'est plus respecté.
Toute la transaction est annulée lorsqu'un contrôle final échoue.

[Chapitre suivant : limites et vérification](04-limites-verification.md)
