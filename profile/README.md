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
  <a href="https://www.npmjs.com/org/portaki">npm @portaki</a>
</p>

---

Portaki aide les hôtes à partager infos pratiques, règles et services aux voyageurs — avec une **plateforme modulaire** : chaque capacité (sections, calendrier, formulaires…) est un module catalogue branché sur un contrat stable.

## Dépôts ouverts

| Dépôt | Description |
|-------|-------------|
| [**portaki-sdk**](https://github.com/PortakiApp/portaki-sdk) | Schéma `module.v1.json`, SDK JS (`@portaki/sdk`, `@portaki/module-sdk`), SDK Java module, CLI |
| [**portaki-modules**](https://github.com/PortakiApp/portaki-modules) | Catalogue officiel et communautaire `@portaki/module-*` |
| [**portaki-landing**](https://github.com/PortakiApp/portaki-landing) | Site marketing [portaki.app](https://portaki.app) |

## Construire un module

1. Lire le [guide modules](https://github.com/PortakiApp/portaki-sdk/tree/main/docs) et le schéma [`module.v1.json`](https://github.com/PortakiApp/portaki-sdk/blob/main/schema/module.v1.json).
2. S’appuyer sur [`@portaki/module-sdk`](https://www.npmjs.com/package/@portaki/module-sdk) (npm) — pas de dépendance `workspace:` vers ce monorepo en publication.
3. Ouvrir une PR sur **portaki-modules** ou publier votre paquet selon [CONTRIBUTING](https://github.com/PortakiApp/.github/blob/main/CONTRIBUTING.md).

## Sécurité

Signalement responsable : voir [SECURITY.md](https://github.com/PortakiApp/.github/blob/main/SECURITY.md) — merci de ne pas divulguer de vulnérabilité exploitable dans une issue publique.

## Équipe

Les dépôts applicatifs (API, web hôte, runtime) sont maintenus en privé par l’équipe Portaki. Les contributions externes ciblent en priorité le **SDK** et le **catalogue modules**.
