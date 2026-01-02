---
description: Build elaborate, multi-component React/Tailwind/Shadcn artifacts.
---

# Web Artifacts Builder Workflow

## 1. Initialize Project

Run the initialization script from the repo root:

```bash
bash scripts/init-artifact.sh <project-name>
cd <project-name>
```

*This sets up React, TypeScript, Tailwind, Shadcn, and Parcel.*

## 2. Develop

- Edit the generated files in the `<project-name>` directory.
- Use Shadcn components (pre-installed).
- Design according to high aesthetic standards.

## 3. Bundle

Bundle the project into a single HTML file:

```bash
bash scripts/bundle-artifact.sh
```

*Creates `bundle.html` with inlined assets.*

## 4. Delivery

- Share the `bundle.html` file with the user.
- (Optional) Test with Playwright if requested.
