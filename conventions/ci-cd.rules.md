# ⚙️ Règles CI/CD

## Objectifs

- Automatiser les tests et le linting
- Empêcher les déploiements cassés
- Garder un historique clair des releases

## Pipelines minimum

1. **CI (push sur PR)**  
   - Installation des dépendances
   - Lint (ruff / flake8, mypy facultatif)
   - Tests (pytest)
   - Build (si frontend)

2. **CD (tag ou merge sur main)**  
   - Build image Docker
   - Push vers registry
   - Déploiement (Cloud Run / autre)
   - Notification (Slack / mail) en cas d’échec
