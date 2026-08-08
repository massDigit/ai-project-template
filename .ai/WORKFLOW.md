# WORKFLOW.md - Procédures de Validation & Dev Loop

## 🔁 Boucle de Développer-Tester-Valider

Avant de déclarer une tâche terminée, l'agent doit exécuter :

```bash
# 1. Verification TypeScript / Typecheck
npm run typecheck

# 2. Linter
npm run lint

# 3. Tests Unitaires & Intégration
npm test
```

Si l'une de ces commandes échoue, l'agent doit immédiatement traiter l'erreur avant de poursuivre.
