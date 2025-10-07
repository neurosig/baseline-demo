# NeuroSIG × Baseline — Demo

**Live demo:** `https://<YOUR-USERNAME>.github.io/<REPO-NAME>/`  
**Code:** `https://github.com/<YOUR-USERNAME>/<REPO-NAME>`

## What this is
A small **bridge** that **matches natural-language questions** to **Baseline’s query grammar/tooling**. Baseline already has excellent feature data; NeuroSIG removes the friction of “how do I phrase the query?” so developers reach the right signals faster.

## Why it matters
- **Faster discovery:** plain questions → Baseline-compatible queries.
- **Lower barrier:** no need to memorize feature IDs or syntax.
- **Adoption boost:** quicker path to using modern web features.

## How it works (demo flow)
1. Type a plain question (e.g., “Can I use CSS :has() on iOS 15? Fallback?”).
2. Click **Translate**.
3. The app renders a **Baseline-style query** (e.g., `feature:css.selectors.has AND engine:safari AND version>=15 AND need:fallback`).
4. **Copy query** or **Open Baseline** to continue in existing tools.

> **Left/Right intent (if your UI shows two sides):**  
> Left panel = Baseline’s structured query form (reference).  
> Right panel = NeuroSIG’s contribution (natural → structured).

## Example queries
- “Does Chrome support WebGPU yet?”  
  → `feature:api.webgpu AND engine:chrome`
- “Can I use :has() on iOS 15? Fallback?”  
  → `feature:css.selectors.has AND engine:safari AND version>=15 AND need:fallback`

## Status
Prototype demo (no backend). Built for the Baseline Hackathon to illustrate integration potential.

## Built with
- HTML / CSS / JavaScript (vanilla)
- GitHub Pages (static hosting)
- Baseline query grammar (integration target)

## Roadmap
- Expand mappings (more features, engines, versions).
- VS Code command/extension.
- Shareable “query cards” for PRs/issues.
- Multilingual input & accessibility modes.

## License
MIT © 2025 <Created by NeuroSIG>
