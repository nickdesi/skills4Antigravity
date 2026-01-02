# Comment utiliser les Skills avec Google Antigravity

([English version](./TUTORIAL.md))

Ce guide explique comment utiliser les **workflows natifs** inclus dans ce dépôt avec votre agent Google Antigravity.

## Prérequis

1. **Agent Google Antigravity** : Vous devez avoir accès à l'environnement de l'agent Antigravity.
2. **Cloner ce dépôt** : Vous devez avoir cloner ce dépôt sur votre machine locale, ou qu'il soit accessible à l'agent.

```bash
git clone https://github.com/nickdesi/skills4Antigravity.git
```

## Comment ça marche

Antigravity cherche les workflows dans le répertoire `.agent/workflows/`. En ayant ce dépôt dans votre espace de travail (ou en copiant le dossier `.agent` dans votre projet), l'agent peut automatiquement découvrir et exécuter ces workflows avancés.

## Workflows Disponibles

### 1. Design Frontend (`frontend-design`)

**Utilisez ceci pour** : Créer des interfaces web de haute qualité, non génériques.
**Commande** :
> "Utilise le workflow frontend-design pour créer une landing page pour un café."

### 2. Test d'Application Web (`webapp-testing`)

**Utilisez ceci pour** : Tester des applications web locales avec Playwright.
**Commande** :
> "Lance le workflow webapp-testing pour vérifier le flux de connexion sur localhost:3000."

### 3. Créateur de Serveur MCP (`mcp-builder`)

**Utilisez ceci pour** : Construire des serveurs Model Context Protocol pour connecter des sources de données.
**Commande** :
> "Suis le workflow mcp-builder pour créer un serveur MCP SQLite."

### 4. Créateur d'Artefacts Web (`web-artifacts-builder`)

**Utilisez ceci pour** : Créer des artefacts React complexes et multi-fichiers.
**Commande** :
> "Lance le workflow web-artifacts-builder pour faire un tableau de bord."

### 5. Master Router (`router`)

**Utilisez ceci pour** : Quand vous ne savez pas quel workflow choisir.
**Commande** :
> "Lance le workflow router."

### 6. Audit de Sécurité (`security-audit`)

**Utilisez ceci pour** : Scanner le code pour des vulnérabilités et secrets.
**Commande** :
> "Lance un audit de sécurité sur ce projet."

### 7. Refactoring de Code (`code-refactor`)

**Utilisez ceci pour** : Nettoyer la dette technique proprement.
**Commande** :
> "Utilise le workflow code-refactor pour nettoyer utilities.py."

## Conseils pour de meilleurs résultats

- **Soyez Spécifique** : Lorsque vous invoquez un workflow, donnez du contexte.
  - *Mauvais* : "Lance le workflow de design."
  - *Bon* : "Utilise le workflow frontend-design pour créer un tableau de bord en mode sombre pour une application de trading crypto."
- **Révisez les Plans** : L'agent proposera souvent un plan avant d'exécuter le workflow. Révisez-le attentivement.
- **Emplacement des Workflows** : Vous pouvez personnaliser ces workflows en éditant les fichiers markdown dans `.agent/workflows/`.
