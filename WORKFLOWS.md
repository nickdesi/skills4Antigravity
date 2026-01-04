# Antigravity Workflows for Skills

This repository includes a set of **Antigravity Workflows** that allow you to natively execute the skills defined in this repository. These workflows are located in `.agent/workflows/`.

## Available Workflows

### 1. MCP Builder

**ID**: `mcp-builder`
**Description**: Guide for creating high-quality Model Context Protocol (MCP) servers.
**Usage**:
> "Follow the mcp-builder workflow to create a new server."

### 2. Web Application Testing

**ID**: `webapp-testing`
**Description**: Toolkit for interacting with and testing local web applications using Playwright.
**Usage**:
> "Run the webapp-testing workflow to test the login page."

### 3. Frontend Design

**ID**: `frontend-design`
**Description**: Create distinctive, production-grade frontend interfaces with high design quality.
**Usage**:
> "Use the frontend-design workflow to design a new dashboard."

### 4. Web Artifacts Builder

**ID**: `web-artifacts-builder`
**Description**: Build elaborate, multi-component React/Tailwind/Shadcn artifacts.
**Usage**:
> "Run the web-artifacts-builder workflow for a new project."
>
### 5. Master Router

**ID**: `router`
**Description**: Master workflow that identifies the user's intent and directs them to the appropriate specialized workflow.
**Usage**:
> "Run the router workflow."

### 6. Security Audit

**ID**: `security-audit`
**Description**: Systematically scan the codebase for security vulnerabilities, exposed secrets (API keys, credentials), and common security piftalls.
**Usage**:
> "Run a security-audit on this project."

### 7. Code Refactor

**ID**: `code-refactor`
**Description**: Safely refactor code to improve quality without breaking functionality. Covers technical debt, variable naming, and function extraction.
**Usage**:
> "Use code-refactor to clean up the user controller."

### 8. Setup Check

**ID**: `setup-check`
**Description**: Verify the development environment. Checks for Node.js, Python, Git, and other essential dependencies.
**Usage**:
> "Run the setup-check."

### 9. Parallel Orchestrator

**ID**: `parallel-orchestrator`
**Description**: Deploys a team of multiple simulated agents (Plan, Code, Review) to handle complex, multi-step tasks in a single session.
**Usage**:
> "Run the parallel-orchestrator to build the payment system."

### 10. Debugging

**ID**: `debugging-workflow`
**Description**: A rigorous, scientific method for identifying the root cause of bugs. Enforces hypothesis testing and evidence gathering.
**Usage**:
> "Run the debugging-workflow to fix the crash."

### 11. Performance Audit

**ID**: `performance-audit`
**Description**: Analyzes the application for performance bottlenecks, including bundle size, render cycles, and asset optimization.
**Usage**:
> "Run a performance-audit on the dashboard."

### 12. Release Manager

**ID**: `release-manager`
**Description**: Automates the release process: updates `package.json` version, updates `CHANGELOG.md`, and creates a git tag.
**Usage**:
> "Use release-manager to ship v2.0.0."
>
## execution

These workflows are standard markdown files that the Antigravity agent can read and execute step-by-step. They are located in `.agent/workflows/*.md`.
