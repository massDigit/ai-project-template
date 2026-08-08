# RULES.md - Règles d'Ingénierie Stricte

> **Ces règles sont NON NÉGOCIABLES pour tout assistant IA ou développeur travaillant sur la codebase.**

1. **Aucun patch superficiel** : Toujours corriger la cause racine au lieu de contourner les exceptions.
2. **Découplage & Modularité** : Séparer strictement la logique métier des couches d'affichage et d'infrastructure.
3. **Contrat d'API strict** : Ne jamais altérer une signature de fonction ou de type sans mettre à jour tous ses appels.
4. **Ne jamais deviner les schemas** : Toujours lire la définition exacte des entités dans `docs/DATABASE.md` ou le code source avant consommation.
5. **Gestion propre du state** : Ne pas muter directement l'état global avec des objets partiels ou incomplets.
6. **Classification des décisions & non-usurpation d'ADR** : Ne jamais inscrire une proposition technique de l'agent dans `.ai/DECISIONS.md` sans validation explicite de l'utilisateur. Toute hypothèse non confirmée doit figurer dans `.ai/ASSUMPTIONS.md`.

