# 🧷 Règles Git & branches

## Branches

- `main` : toujours déployable en production
- `develop` : intégration continue (optionnel)
- `feat/<slug>` : nouvelles fonctionnalités
- `fix/<slug>` : corrections de bugs
- `chore/<slug>` : tâches techniques (refacto, deps…)

## Messages de commit

Format recommandé :

```txt
<type>: <description courte>

Exemples :
feat: ajoute endpoint /health
fix: corrige bug pagination sur /items
chore: met à jour dépendances fastapi 0.115
```

Types possibles : `feat`, `fix`, `chore`, `docs`, `refactor`, `test`.

## Pull Requests

- Minimum 1 review (sauf hotfix critique).
- Checklist de PR :
  - [ ] Tests passés
  - [ ] Docs mises à jour si nécessaire
  - [ ] Pas de secrets dans le diff
