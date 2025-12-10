# 🧩 Project Rules Hub

Ce dépôt centralise toutes les **règles de conception, d’architecture et de qualité** 
pour tes projets (FastAPI, Django, MCP, etc.).

Il est pensé pour être :

- ✅ Copiable tel quel dans un projet sous forme de dossier `.rules/`
- ✅ Lisible par des humains (docs Markdown)
- ✅ Exploitable par des agents IA / MCP (fichiers `.rules.json` structurés)

---

## 📁 Structure

- `stacks/`  
  Règles spécifiques à chaque stack :
  - `fastapi-api.rules.json`
  - `fastapi-webapp.rules.json`
  - `django-restapi.rules.json`
  - `django-webapp.rules.json`
  - `mcp-server.rules.json`

- `conventions/`  
  Règles transverses :
  - `git.rules.md` (branches, commit messages, PR)
  - `ci-cd.rules.md` (pipelines, qualité, déploiement)
  - `observability.rules.md` (logs, métriques, traces)
  - `security.rules.md` (secrets, auth, durcissement)

- `templates/`  
  Templates et squelettes à réutiliser dans les projets.

- `.rules.schema.json`  
  Schéma générique des fichiers `.rules.json` pour automatiser le contrôle.

---

## 🔧 Utilisation dans un projet existant

1. Copier ce dépôt dans ton projet sous forme de dossier masqué :

   ```bash
   cp -R project-rules/ /chemin/vers/ton-projet/.rules
   ```

2. Adapter les règles par stack au besoin (ajout/suppression de checklists).

3. (Optionnel) Connecter ce dossier `.rules/` à un **serveur MCP** ou un script Python
   qui lit les fichiers `.rules.json` et vérifie la conformité du projet.

---

## 🚀 Vision

L’objectif est d’avoir, pour chaque projet :

- un `/src` qui vit sa meilleure vie,
- un `/.rules` qui définit ce qu’est un projet propre, maintenable et prod-ready.

Ce repo sert de **cerveau de standardisation** à plugger partout.
