---
description: Guide for creating high-quality MCP (Model Context Protocol) servers.
---

# MCP Server Development Workflow

## 1. Deep Research and Planning

- **Understand Modern MCP Design**:
  - Balance API coverage with workflow tools.
  - Use clear, descriptive tool names (e.g., `github_create_issue`).
  - Design tools to return focused, relevant data.
- **Study Documentation**:
  - Review MCP specs: `https://modelcontextprotocol.io/sitemap.xml`
  - Review Framework docs (TS/Python SDKs).
- **Plan Implementation**:
  - Review the target service's API documentation.
  - List endpoints to implement.
  - Define Input/Output schemas (Zod/Pydantic).

## 2. Implementation

- **Set Up Project**:
  - TypeScript: `npm init` and configure `tsconfig.json`.
  - Python: Set up `pyproject.toml` or `requirements.txt`.
- **Implement Core Infrastructure**:
  - API client with auth.
  - Error handling and pagination.
- **Implement Tools**:
  - Define strictly typed schemas.
  - Include helpful descriptions for models.
  - Implement logic with async/await.

## 3. Review and Test

- **Code Quality**:
  - Check for DRY, error handling, and type safety.
- **Build and Test**:
  - TypeScript: `npm run build`
  - Verify with MCP Inspector: `npx @modelcontextprotocol/inspector`

## 4. Evaluation (Optional)

- Create prompt-based evaluations to test if an LLM can effectively use the tools to answer complex questions.
