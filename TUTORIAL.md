# How to use Skills with Google Antigravity

([Version française](./TUTORIAL_FR.md))

This guide explains how to use the **native workflows** included in this repository with your Google Antigravity agent.

## Prerequisites

1. **Google Antigravity Agent**: You must have access to the Antigravity agent environment.
2. **Clone this Repository**: You need to have this repository cloned on your local machine, or accessible to the agent.

```bash
git clone https://github.com/nickdesi/skills4Antigravity.git
```

## How it Works

Antigravity looks for workflows in the `.agent/workflows/` directory. By having this repository in your workspace (or copying the `.agent` folder to your project), the agent can automatically discover and execute these advanced workflows.

## Available Workflows

### 1. Frontend Design (`frontend-design`)

**Use this for**: Creating high-quality, non-generic web interfaces.
**Command**:
> "Use the frontend-design workflow to create a landing page for a coffee shop."

### 2. Web App Testing (`webapp-testing`)

**Use this for**: Testing local web applications with Playwright.
**Command**:
> "Run the webapp-testing workflow to verify the login flow on localhost:3000."

### 3. MCP Server Builder (`mcp-builder`)

**Use this for**: Building Model Context Protocol servers to connect data sources.
**Command**:
> "Follow the mcp-builder workflow to create a SQLite MCP server."

### 4. Web Artifacts Builder (`web-artifacts-builder`)

**Use this for**: Creating complex, multi-file React artifacts.
**Command**:
> "Run the web-artifacts-builder workflow to make a dashboard."

### 5. Master Router (`router`)

**Use this for**: When you don't know which workflow to pick.
**Command**:
> "Run the router workflow."

### 6. Security Audit (`security-audit`)

**Use this for**: Scanning code for vulnerabilities and secrets.
**Command**:
> "Run a security audit on this project."

### 7. Code Refactor (`code-refactor`)

**Use this for**: Cleaning up technical debt safely.
**Command**:
> "Use the code-refactor workflow to clean up utilities.py."

## Tips for Best Results

- **Be Specific**: When invoking a workflow, provide context.
  - *Bad*: "Run the design workflow."
  - *Good*: "Use the frontend-design workflow to create a dark-mode dashboard for a crypto trading app."
- **Review Plans**: The agent will often propose a plan before executing the workflow. Review it carefully.
- **Workflow Location**: You can customize these workflows by editing the markdown files in `.agent/workflows/`.
