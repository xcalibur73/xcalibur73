# xcalibur73

**Systems Engineer & Technical SEO Strategist**  
*Headless Chromium Automation, Core Web Vitals, and Generative Engine Optimization*

[WebAudits.pro](https://webaudits.pro) | [GitHub Repositories](https://github.com/xcalibur73?tab=repositories) | [AestheticArches.com](https://aestheticarches.com)

---

I build open-source diagnostic engines that audit DOM hydration disparities, Core Web Vitals bottlenecks, RFC 9309 crawler collisions, and semantic knowledge graphs. My work bridges low-level headless browser automation with technical search architecture, providing defensible, empirical tooling for engineering teams. These diagnostic engines power the underlying analysis pipeline of [WebAudits.pro](https://webaudits.pro).

---

## Flagship Projects

The following four core repositories represent the primary diagnostic engines developed for high-precision technical auditing:

### 1. [DOMHydrate](https://github.com/xcalibur73/dom-hydrate)
**Forensic CSR vs. SSR SEO Diff Engine**  
Compares raw server HTML against fully hydrated client DOM using native Chromium (`--headless=new --dump-dom`). Detects client-dropped Schema.org JSON-LD scripts, hydration-injected noindex directives, and internal link graph mutations before deployment.  
- **Web Platform:** [webaudits.pro/tools/hydration-audit](https://webaudits.pro/tools/hydration-audit)  
- **Benchmarks:** [Empirical 12-Site SSR vs. CSR Study](https://github.com/xcalibur73/dom-hydrate/blob/main/BENCHMARKS.md)  
- **Stack:** Python 3.10+, Headless Chromium, BeautifulSoup4, Rich

### 2. [IndexTrace](https://github.com/xcalibur73/index-trace)
**Google Search Console Forensic Diagnostic & RFC 9309 Crawler Tracer**  
Follows redirect chains hop by hop, detects redirect loops, flags SSL protocol downgrades, and pinpoints the exact line number of blocking directives in robots.txt using RFC 9309 longest-match precedence. Classifies soft-404 response patterns and provides ordered remediation steps.  
- **Web Platform:** [webaudits.pro/tools/index-trace](https://webaudits.pro/tools/index-trace)  
- **Benchmarks:** [Line-Level RFC 9309 Case Studies](https://github.com/xcalibur73/index-trace/blob/main/BENCHMARKS.md)  
- **Stack:** Python 3.10+, RFC 9309 Parser, HTTP Hop Tracer

### 3. [PayloadSniper](https://github.com/xcalibur73/payload-sniper)
**Interaction to Next Paint (INP), Long Tasks & Script Bloat-Tracer**  
Profiles JavaScript execution, main-thread Long Tasks (> 50ms), and third-party tag congestion using Chrome DevTools Protocol (CDP) performance timelines. Simulates mid-tier mobile hardware with 4x CPU throttling to diagnose synthetic INP friction points.  
- **Web Platform:** [webaudits.pro/tools/payload-sniper](https://webaudits.pro/tools/payload-sniper)  
- **Benchmarks:** [12-Site Third-Party Script Cost Study](https://github.com/xcalibur73/payload-sniper/blob/main/BENCHMARKS.md)  
- **Stack:** Python 3.10+, Chromium CDP, W3C Navigation Timing

### 4. [SchemaGraph](https://github.com/xcalibur73/schema-graph)
**Cross-Page Entity & Knowledge Graph Integrity Tracer**  
Constructs in-memory directed knowledge graphs across multi-page site clusters from Schema.org JSON-LD blocks. Detects broken `@id` URI references, circular dependency loops, orphan entity nodes, publisher metadata drift, and missing `sameAs` entity disambiguation signals.  
- **Web Platform:** [webaudits.pro/tools/schema-graph](https://webaudits.pro/tools/schema-graph)  
- **Benchmarks:** [Cross-Page Entity Integrity Study](https://github.com/xcalibur73/schema-graph/blob/main/BENCHMARKS.md)  
- **Stack:** Python 3.10+, Graph Engine, DFS Cycle Detection, 95 Unit Tests

---

## The Diagnostic Tooling Ecosystem

All repositories follow PEP 621 packaging standards, provide automated unit test suites, run GitHub Actions CI/CD pipelines, and link back to live web platform endpoints on [WebAudits.pro](https://webaudits.pro).

```text
                               +-----------------------------+
                               |        WebAudits.pro        |
                               |  Technical Audit Platform   |
                               +--------------+--------------+
                                              |
        +---------------------+---------------+---------------------+---------------------+
        |                     |                                     |                     |
        v                     v                                     v                     v
 [Rendering & DOM]    [Crawl & Directives]                 [Performance & INP]    [Semantic & Entities]
  - DOMHydrate         - IndexTrace                         - PayloadSniper        - SchemaGraph
  - OverflowTrace      - LinkBleed                          - ImgSpec              - CitationPulse
                                                                                   - ContextSilo
```

### Complete Tool Suite

| Tool | Focus Area | Core Standard / Heuristic | Platform Route |
|:---|:---|:---|:---|
| [DOMHydrate](https://github.com/xcalibur73/dom-hydrate) | SSR vs. CSR Parity | Chromium AST / DOM Expansion | [/tools/hydration-audit](https://webaudits.pro/tools/hydration-audit) |
| [IndexTrace](https://github.com/xcalibur73/index-trace) | GSC Indexing & Directives | RFC 9309 Robots.txt Parser | [/tools/index-trace](https://webaudits.pro/tools/index-trace) |
| [PayloadSniper](https://github.com/xcalibur73/payload-sniper) | INP & Long Tasks | W3C Long Tasks / 4x CPU Throttling | [/tools/payload-sniper](https://webaudits.pro/tools/payload-sniper) |
| [SchemaGraph](https://github.com/xcalibur73/schema-graph) | Entity Knowledge Graphs | W3C RDF / Schema.org Directed Graph | [/tools/schema-graph](https://webaudits.pro/tools/schema-graph) |
| [OverflowTrace](https://github.com/xcalibur73/overflow-trace) | Mobile Viewport Layout | Visual Viewport API / 0-Scroll Spill | [/tools/overflow-trace](https://webaudits.pro/tools/overflow-trace) |
| [ImgSpec](https://github.com/xcalibur73/img-spec) | LCP & Breakpoint Efficiency | Viewport Geometry / Pixel Waste | [/tools/img-spec](https://webaudits.pro/tools/img-spec) |
| [LinkBleed](https://github.com/xcalibur73/link-bleed) | Internal Link Equity | Power Iteration Link-Equity Model | [/tools/link-bleed](https://webaudits.pro/tools/link-bleed) |
| [CitationPulse](https://github.com/xcalibur73/citation-pulse) | Generative Engine Optimization | Princeton KDD 2024 Passage Citability | [/tools/geo-audit](https://webaudits.pro/tools/geo-audit) |
| [ContextSilo](https://github.com/xcalibur73/context-silo) | Semantic Anchor Vector Contiguity | TF-IDF Cosine Similarity Vectors | [/tools/context-silo](https://webaudits.pro/tools/context-silo) |

---

## Production Platforms

### [WebAudits.pro](https://webaudits.pro)
Technical performance intelligence and audit platform.
- **Architecture:** Next.js App Router, TypeScript, Tailwind CSS.
- **Performance:** 120 pre-rendered static routes, sub-2.5s mobile LCP, 0 CLS.
- **Structured Data:** 143 validated Schema.org JSON-LD instances across technical articles, reviews, and interactive diagnostic tools.

### [AestheticArches.com](https://aestheticarches.com)
Architectural and interior design publication.
- **Architecture:** GeneratePress Premium, Gutenberg custom blocks, LiteSpeed server caching, Cloudflare CDN.
- **Performance:** Zero-CLS layout budget, fluid clamp() typography scales, responsive image optimization.

---

## Engineering Standards & Methodologies

Every tool repository adheres to strict software engineering standards:
1. **Defensible Metric Taxonomy:** Metrics are explicitly labeled as established standards (RFC 9309, W3C Navigation Timing), project-derived heuristics (Passage Citability score), or experimental indicators (synthetic INP projection).
2. **Reproducible Benchmarks:** Every field study documents the exact test dataset, tool version, execution command, hardware environment, raw telemetry, and mathematical calculation formulas.
3. **Automated Testing:** 177 unit tests continuously validated across Python 3.10 and 3.12 environments via GitHub Actions CI.
4. **Cross-Platform Safety:** Fully hardened against Windows terminal encoding failures (`_safe_str` sanitization).
5. **Standardized Packaging:** PEP 621 `pyproject.toml` specification supporting direct installation via `pip install .`.

---

## Technical Stack

| Category | Technologies |
|:---|:---|
| **Core Web Vitals** | INP optimization, LCP acceleration, 0-CLS layouts, main-thread Long Task profiling |
| **Browser Automation** | Chrome DevTools Protocol (CDP), Headless Chromium, Python, Playwright |
| **Technical SEO** | RFC 9309 robots.txt, Schema.org JSON-LD, crawl budget modeling, llms.txt |
| **Frontend Engineering** | Next.js App Router, React, TypeScript, Tailwind CSS, Chrome Extensions (Manifest V3) |
| **CMS Architecture** | GeneratePress, Gutenberg blocks, LiteSpeed Cache, Redis object cache, Cloudflare CDN |

---

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=xcalibur73&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=xcalibur73&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" />
</div>
