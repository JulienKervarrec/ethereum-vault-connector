# 2. Comptes, collatéraux et contrôleurs

L'EVC identifie un propriétaire puis lui permet d'utiliser plusieurs sous-comptes dérivés de son adresse.
Chaque sous-compte conserve sa propre liste de collatéraux activés et son contrôleur éventuel.
Activer un collatéral ne déplace pas automatiquement les actifs : cela le rend visible pour les contrôles ultérieurs.
Le contrôleur est le coffre autorisé à créer et suivre la dette de ce compte.
Un seul contrôleur est actif à la fois, ce qui évite que plusieurs coffres modifient simultanément le même état d'emprunt.
Les opérateurs peuvent agir au nom d'un propriétaire selon les autorisations enregistrées par le connecteur.
Le code vérifie l'identité de l'appelant et le préfixe de sous-compte avant de transmettre un appel.
Ces relations forment la frontière d'autorisation que chaque coffre doit respecter.

[Chapitre suivant : appels groupés et contrôles différés](03-appels-controles.md)
