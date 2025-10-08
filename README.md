# NeuroSIG × Baseline — Demo

*Natural language to Baseline queries — a demo bridge for faster web-feature adoption.*

---

## What this is
This demo shows how **NeuroSIG** can connect natural-language “signals” to **Baseline’s query grammar and developer tooling**.  
The goal is to streamline how developers access modern web features by lowering the barrier between asking plain questions and retrieving structured results.  

Baseline already provides excellent feature data. NeuroSIG reduces the friction of *“how do I phrase the query?”* so developers can reach the right signals faster.

---

## Why it matters
Baseline provides high-quality data sources like the Web Platform Dashboard API and web-features package. Many developers face friction when trying to integrate them. This demo highlights how a natural-language layer can make those resources more approachable, especially under real-world time constraints:

- **Faster discovery:** Plain questions → Baseline-compatible queries.  
- **Lower barrier:** No need to memorize feature IDs or syntax.  
- **Adoption boost:** Quicker path to using modern web features.  
- **Scrappy MVP:** Built in under 12 hours during the hackathon to illustrate integration potential quickly.  

---

## Key Features
- **Natural-language input → Baseline queries**  
- **Copy or open queries** directly in Baseline tools  
- **Hackathon MVP build** with <12 hours to highlight integration potential  

---

## How it works (demo flow)

1. A user enters a natural-language question (e.g., *“Can I use CSS :has() on iOS 15? Fallback?”*).  
2. Click **Translate**. The demo maps it to Baseline’s query grammar.  
3. The right-hand button redirects to a result page (e.g. Baseline docs or API output); the demo also renders a **Baseline-style query** (e.g.,  
   `features.css.selectors.has AND engines:safari AND versions:15 AND need:fallback`).  
4. The left-hand column allows copying the generated query for reuse (e.g. **Copy query** or **Open Baseline** to continue in existing tools).  

_Left/Right intent (if your UI shows two sides):_  
- Left panel = Baseline’s structured query (from reference).  
- Right panel = NeuroSIG’s contribution (natural + structured).  

---

## Example queries
- **“Does Chrome support WebGPU yet?”**  
  → `features.api.webgpu AND engines:chrome`  

- **“Can I use :has() on iOS 15? Fallback?”**  
  → `features.css.selectors.has AND engines:safari AND versions:15 AND need:fallback`  

---

## Status
Prototype demo (no backend). Built for the Baseline Hackathon to illustrate integration potential.  

---

## Built With
- **Languages/Frameworks:** JavaScript, React, basic HTML/CSS  
- **Platform:** GitHub Pages for hosting  
- **Integration Target:** Baseline’s Web Platform Dashboard API & web-features package  

---

## Roadmap
Future directions (if this were to grow beyond the hackathon prototype):  
- Expand mappings (cover more features, engines, versions).  
- Explore VS Code extension / lightweight command tools.  
- Simple ways to share query results (e.g. “cards” for PRs/issues).  
- Multilingual input & basic accessibility modes.  

---

## Notes
This repo was created as part of the **Baseline Tooling Hackathon (Oct 2025)**.  
It is an MVP demo to explore the concept of bridging natural-language inputs with Baseline developer tools.  

Ongoing updates may expand or refine this proof of concept.  

---

## License
MIT © 2025 NeuroSIG
