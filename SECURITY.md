# Politique de sécurité

## Versions supportées

Les correctifs de sécurité sont publiés sur les branches de maintenance des dépôts **actifs** (voir releases et tags de chaque dépôt). Les dépôts archivés ne reçoivent plus de correctifs sauf exception critique.

## Signaler une vulnérabilité

**Ne pas** ouvrir d’issue publique avec les détails d’une vulnérabilité exploitable (fuite de secret, injection, contournement d’auth, RCE, etc.).

1. Contacter l’équipe Portaki par un canal **privé** (responsable org `PortakiApp`, ou procédure interne si vous êtes contributeur membre).
2. Inclure : description, impact, étapes de reproduction, version/commit concernés, suggestion de correctif si vous en avez une.
3. Nous accusons réception dès que possible et coordonnons une divulgation responsable.

## Périmètre

| In scope | Hors scope |
|----------|------------|
| Dépôts publics PortakiApp (SDK, modules, landing) | Services hébergés non documentés, scans génériques sans impact |
| Dépendances livrées (npm, Maven) avec preuve d’impact | Social engineering, phishing du site marketing |
| Fuites de secrets dans l’historique Git public | Problèmes déjà signalés et en cours de traitement |

## Bonnes pratiques contributeurs

- Ne pas committer de clés API, JWT, mots de passe ou `.env` réels.
- Mettre à jour les dépendances via les PR Renovate / dépendabot lorsque proposées.
- Pour les modules : ne pas exfiltrer de données invité hors contrats SDK documentés.

Merci d’aider à garder l’écosystème Portaki sûr pour les hôtes et les voyageurs.
