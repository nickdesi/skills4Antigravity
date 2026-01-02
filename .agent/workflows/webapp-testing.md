---
description: Toolkit for interacting with and testing local web applications using Playwright.
---

# Web Application Testing Workflow

## 1. Choose Approach

- **Static HTML**: Read file directly and identify selectors.
- **Dynamic Webapp**:
  - If server NOT running: Use `scripts/with_server.py`.
  - If server running: Proceed to Reconnaissance.

## 2. Start Server (if needed)

**Single Server**:

```bash
python scripts/with_server.py --server "npm run dev" --port 5173 -- python your_automation.py
```

**Multiple Servers**:

```bash
python scripts/with_server.py \
  --server "cd backend && python server.py" --port 3000 \
  --server "cd frontend && npm run dev" --port 5173 \
  -- python your_automation.py
```

## 3. Reconnaissance

1. **Navigate**: Go to URL and wait for `networkidle`.

   ```python
   page.goto('http://localhost:5173')
   page.wait_for_load_state('networkidle')
   ```

2. **Inspect**: Take screenshot or dump DOM to accept selectors.

   ```python
   page.screenshot(path='/tmp/inspect.png')
   ```

## 4. Automation

- Write Playwright script using discovered selectors.
- Use `sync_playwright`.
- ALWAYS close the browser: `browser.close()`.
