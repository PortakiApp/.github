# Contribuer à Portaki (dépôts publics)

Merci de votre intérêt pour Portaki. Ce fichier s’applique par défaut aux dépôts publics de [PortakiApp](https://github.com/PortakiApp) qui n’ont pas leur propre `CONTRIBUTING.md`.

## Où contribuer

| Zone | Dépôt typique | Profil contributeur |
|------|---------------|---------------------|
| SDK, schéma, CLI, docs auteur | `portaki-sdk` | Développeur module / intégrateur |
| Modules catalogue | `portaki-modules` | Auteur de module officiel ou communautaire |
| Site marketing | `portaki-landing` | Contenu, i18n, UX vitrine |

L’API, le dashboard hôte et l’infra production ne sont pas ouverts aux PR externes pour l’instant.

## Avant une pull request

1. Ouvrir une **issue** pour les changements non triviaux (nouveau module, breaking SDK).
2. Créer une branche depuis `main` (ou la branche par défaut du dépôt).
3. Exécuter les vérifications locales du dépôt (voir README du repo) :
   - **portaki-sdk** : `pnpm install`, `pnpm test`, build des paquets concernés.
   - **portaki-modules** : scripts CI du module (`test`, `build`, backend Java si présent).
4. Ne jamais committer de secrets, tokens, URLs internes ou données personnelles.

## Commits

Préférence pour [Conventional Commits](https://www.conventionalcommits.org/) : `feat:`, `fix:`, `docs:`, `chore:`, etc. Messages en français ou anglais, mais clairs et orientés « pourquoi ».

## Modules (`portaki-modules`)

- Respecter `portaki.module.json` et le schéma [`module.v1.json`](https://github.com/PortakiApp/portaki-sdk/blob/main/schema/module.v1.json).
- Déclarer `requiresHostSdk` (semver **X.Y.Z**) aligné sur la version publiée de `@portaki/module-sdk`.
- Données et handlers gateway dans le **backend** du module (`backend/`), pas dans l’orchestrateur.
- UI invité dans le paquet npm ; UI hôte via `hostSurfaces` + shell Portaki (pas de routes REST dédiées module dans l’API publique).
- E-mails transactionnels : contenu module uniquement ; pas d’envoi SMTP/Resend depuis le JAR.

## Revue

Les mainteneurs peuvent demander des ajustements, des tests ou une mise à jour de la doc. La fusion se fait quand la CI est verte et le périmètre est accepté.

## Code de conduite

En participant, vous acceptez le [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).
