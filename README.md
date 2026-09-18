## Parcours français

Un parcours en quatre chapitres sur l’architecture, les comptes et les contrôles différés de l’EVC est disponible dans [`docs/fr/`](docs/fr/).

# Ethereum Vault Connector

L’Ethereum Vault Connector (EVC) est une couche commune destinée aux marchés de prêt.
Il coordonne des coffres compatibles ERC-4626, des collatéraux, des contrôleurs et des sous-comptes.
La documentation amont détaillée reste disponible sur [evc.wtf](https://evc.wtf/) et dans le [livre blanc](https://github.com/euler-xyz/ethereum-vault-connector/tree/master/docs/whitepaper.md).

## Contrats principaux

- `EthereumVaultConnector.sol` : médiation et exécution.
- `ExecutionContext.sol` : contexte des appels groupés.
- `TransientStorage.sol` et `Set.sol` : stockage et ensembles internes.
- `interfaces/` : contrats attendus des coffres et signatures.

Le logiciel amont est expérimental. Consulter les limites et la suite de tests du dépôt avant toute intégration.

## Licence

GPL-2.0-or-later. Voir [LICENSE](LICENSE).
