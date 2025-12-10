# 🔒 Règles de sécurité

## Secrets

- Jamais de secret dans le code ou les commits
- Utiliser un Secret Manager ou un vault chiffré
- Fichier `.env` présent uniquement en local et ignoré par Git

## Authentification & autorisation

- Utiliser des tokens ou sessions sécurisées (JWT, cookies httponly)
- Limiter les droits (principe du moindre privilège)
- Protéger les endpoints d’admin avec des rôles explicites

## Surface d’attaque

- Activer les protections de base (rate limiting, validation des inputs)
- Configurer CORS correctement
- Filtrer/valider tous les fichiers uploadés
