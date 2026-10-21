# Dépôts publics PortakiApp

Cartographie des dépôts **ouverts** de l’organisation. Pour la liste complète (privés inclus), voir le dépôt interne `.github-private`.

| Dépôt | Rôle |
|-------|------|
| [portaki-sdk](https://github.com/PortakiApp/portaki-sdk) | SDK Rust des modules Wasm (`portaki-sdk`, `portaki-sdk-macros`, `portaki-connectors`, `portaki-test-utils`) et CLI `portaki-cli` |
| [portaki-modules](https://github.com/PortakiApp/portaki-modules) | Modules officiels `modules/<id>/`, publiés en images OCI |
| [portaki-release-action](https://github.com/PortakiApp/portaki-release-action) | GitHub Action de build et publication d’un module |
| [portaki-changelog](https://github.com/PortakiApp/portaki-changelog) | Notes de version produit (`releases.yaml`) lues par l’espace hôte |
| [.github](https://github.com/PortakiApp/.github) | Profil org public, fichiers communauté par défaut |

## Dépendances publiées

- **crates.io** : [`portaki-sdk`](https://crates.io/crates/portaki-sdk), `portaki-sdk-macros`, `portaki-connectors`, `portaki-test-utils`, `portaki-cli`.
- **Modules** : images OCI `oci.portaki.app/modules/<id>:<semver>` (voir le README de `portaki-modules`).
- Les paquets npm `@portaki/*` sont dépréciés (remplacés par le SDK Rust).

## Dépôts archivés (référence)

Fusionnés ailleurs — ne plus ouvrir de PR :

| Ancien | Remplacé par |
|--------|----------------|
| `portaki-axon-libs`, `portaki-spring-boot-starter` | `portaki-libs` (privé) |
| `portaki-module-migrator`, `portaki-module-runtime-js` | `portaki-module-runtime` (privé) |
