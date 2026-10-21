<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://portaki.app/logo-dark.svg">
    <img src="https://portaki.app/logo-light.svg" width="177" height="48" alt="Portaki">
  </picture>
</p>

<h3 align="center">Livret d’accueil numérique pour locations saisonnières</h3>

<p align="center">
  <a href="https://portaki.app">Site</a> ·
  <a href="https://github.com/PortakiApp/portaki-sdk">SDK</a> ·
  <a href="https://github.com/PortakiApp/portaki-modules">Modules</a> ·
  <a href="https://crates.io/crates/portaki-sdk">crates.io</a>
</p>

---

Portaki aide les hôtes à partager infos pratiques, règles et services aux voyageurs. La plateforme est **modulaire** : chaque capacité du livret (accès, Wi-Fi, règles, guide local, météo…) est un module **Rust compilé en Wasm** (Extism), exécuté en bac à sable par la plateforme et rendu par le livret en interface pilotée par le serveur.

## Dépôts ouverts

| Dépôt | Description |
|-------|-------------|
| [**portaki-sdk**](https://github.com/PortakiApp/portaki-sdk) | SDK Rust (`portaki-sdk`, macros, connecteurs, utilitaires de test) et CLI `portaki`, publiés sur [crates.io](https://crates.io/crates/portaki-sdk) |
| [**portaki-modules**](https://github.com/PortakiApp/portaki-modules) | Monorepo des modules officiels, publiés en images OCI `oci.portaki.app/modules/<id>` |
| [**portaki-release-action**](https://github.com/PortakiApp/portaki-release-action) | GitHub Action : build, publication, signature et annonce d’un module au registre Portaki |
| [**portaki-changelog**](https://github.com/PortakiApp/portaki-changelog) | Notes de version produit (`releases.yaml`) affichées dans l’espace hôte |
| [**.github**](https://github.com/PortakiApp/.github) | Ce profil et les fichiers communauté par défaut |

## Construire un module

1. Installer la CLI et suivre le démarrage rapide du [SDK](https://github.com/PortakiApp/portaki-sdk#quick-start) (`portaki init`, `portaki check`).
2. Lire la [documentation du SDK](https://github.com/PortakiApp/portaki-sdk/tree/main/docs) et s’inspirer des [modules officiels](https://github.com/PortakiApp/portaki-modules/tree/main/modules).
3. Publier depuis la CI avec [portaki-release-action](https://github.com/PortakiApp/portaki-release-action), ou proposer une PR sur **portaki-modules** selon [CONTRIBUTING](https://github.com/PortakiApp/.github/blob/main/CONTRIBUTING.md).

## Sécurité

Signalement responsable : voir [SECURITY.md](https://github.com/PortakiApp/.github/blob/main/SECURITY.md) — merci de ne pas divulguer de vulnérabilité exploitable dans une issue publique.

## Équipe

Les dépôts applicatifs (plateforme, espace hôte, livret voyageur, site vitrine) sont maintenus en privé par l’équipe Portaki. Les contributions externes ciblent en priorité le **SDK** et les **modules**.
