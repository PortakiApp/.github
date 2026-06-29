<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://portaki.app/logo-dark.svg">
    <img src="https://portaki.app/logo-light.svg" width="177" height="48" alt="Portaki">
  </picture>
</p>

<h3 align="center">Livret d’accueil numérique pour locations saisonnières</h3>

<p align="center">
  <a href="https://portaki.app">Site</a> ·
  <a href="mailto:contact@portaki.app">Contact</a> ·
  <a href="https://github.com/PortakiApp/portaki-sdk">SDK</a> ·
  <a href="https://github.com/PortakiApp/portaki-modules">Modules</a> ·
  <a href="https://www.npmjs.com/org/portaki">npm @portaki</a>
</p>

---

## À propos

**Portaki** est une plateforme d’**expérience voyageur** pour les hôtes Airbnb, conciergeries et gestionnaires de locations courte durée.

Basée en **France**, l’équipe conçoit un livret d’accueil numérique modulaire : règles de maison, infos pratiques, formulaires pré-arrivée, calendrier, contacts d’urgence… Le tout personnalisable par logement, accessible aux voyageurs sans friction, et pilotable depuis un espace hôte.

Notre approche : une **plateforme modulaire** où chaque capacité est un module catalogue branché sur un contrat stable (`module.v1.json`). Les auteurs étendent Portaki sans toucher au cœur applicatif — SDK ouvert, runtime sandboxé, catalogue npm `@portaki/module-*`.

| | |
|---|---|
| **Produit** | Livret invité + dashboard hôte |
| **Cible** | Hébergement touristique & conciergerie |
| **Siège** | France |
| **Contact** | [contact@portaki.app](mailto:contact@portaki.app) |
| **Site** | [portaki.app](https://portaki.app) |

## Stack technique

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java">
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/pnpm-F69220?style=for-the-badge&logo=pnpm&logoColor=white" alt="pnpm">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/WebAssembly-654FF0?style=for-the-badge&logo=webassembly&logoColor=white" alt="WebAssembly">
  <img src="https://img.shields.io/badge/AssemblyScript-007ACC?style=for-the-badge&logo=webassembly&logoColor=white" alt="AssemblyScript">
  <img src="https://img.shields.io/badge/Extism-000000?style=for-the-badge&logo=webassembly&logoColor=white" alt="Extism">
  <img src="https://img.shields.io/badge/JSON_Schema-000000?style=for-the-badge&logo=json&logoColor=white" alt="JSON Schema">
  <img src="https://img.shields.io/badge/Axon-0066CC?style=for-the-badge&logo=apache&logoColor=white" alt="Axon">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white" alt="Vitest">
  <img src="https://img.shields.io/badge/VitePress-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="VitePress">
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel">
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions">
  <img src="https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white" alt="npm">
  <img src="https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white" alt="Maven">
</p>

<details>
<summary><strong>Détail par couche</strong></summary>

| Couche | Technologies |
|--------|--------------|
| **Modules invité** | React 19, TypeScript, `@portaki/sdk`, Vitest |
| **Build & CLI** | `@portaki/cli`, pnpm workspaces, AssemblyScript → Wasm |
| **Runtime module** | Extism, gateway sandboxé, migrations Postgres générées |
| **Plateforme** | API & dashboard hôte (privés), Spring Boot, Axon CQRS |
| **Publication** | npm `@portaki/*`, GitHub Actions, Trusted Publishing OIDC |
| **Docs & vitrine** | VitePress, TypeDoc, site [portaki.app](https://portaki.app) |

</details>

## Compétences

<table>
<tr>
<td width="50%" valign="top">

**Produit & domaine**

- Expérience voyageur en location saisonnière
- Livret d’accueil digital & onboarding invité
- Espace hôte multi-logements
- Modules métier (règles, checklist, iCal, formulaires…)

</td>
<td width="50%" valign="top">

**Ingénierie**

- Architecture modulaire & contrats versionnés
- SDK auteur & developer experience (CLI, schéma, tests)
- Sandboxing Wasm pour handlers gateway
- Event sourcing / CQRS (Axon)
- CI/CD, semver automatisé, docs as code

</td>
</tr>
</table>

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
