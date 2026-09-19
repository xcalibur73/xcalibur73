# xcalibur73

**Systems Engineer & Technical SEO Strategist**  
*Chromium/CDP Automation, Core Web Vitals, and Technical Search Architecture*

[WebAudits.pro](https://webaudits.pro) | [AestheticArches.com](https://aestheticarches.com) | [GitHub Repositories](https://github.com/xcalibur73?tab=repositories)

---

## About Me

I build open-source diagnostic engines that audit DOM hydration disparities, Core Web Vitals bottlenecks, RFC 9309 crawler collisions, and semantic knowledge graphs. My work bridges low-level headless browser automation (Chromium DevTools Protocol) with enterprise technical search architecture, providing defensible, empirical tooling for engineering teams.

---

## Technical SEO Focus

My engineering work targets four core failure modes in modern web platforms:

1. **Rendering & Hydration Parity**: Detecting differences between server-rendered HTML (SSR) and client-side hydrated DOM (CSR) that cause Googlebot indexing and social crawler preview failures.
2. **Crawlability & Directive Resolution**: Following multi-hop redirect chains, isolating SSL protocol downgrades, and resolving RFC 9309 robots.txt precedence down to the exact line number.
3. **Structured Data Knowledge Graphs**: Constructing in-memory entity graphs across multi-page clusters to detect broken `@id` references, circular chains, and missing disambiguation links.
4. **Lab Performance & Interaction Contention**: Profiling JavaScript hydration execution, main-thread Long Tasks (> 50ms), and uncompressed script payload weights under CPU throttling.

---

## Real Sites I Have Built

These production web platforms demonstrate my approach to technical SEO, performance engineering, and content architecture:

### 1. [WebAudits.pro](https://webaudits.pro)
**Technical Web Auditing & Performance Intelligence Platform**
- **Role:** Architecture, full-stack development, technical SEO, and diagnostic engine design.
- **Stack:** Next.js App Router, TypeScript, Tailwind CSS, Python CLI tool integrations.
- **Performance:** 120 pre-rendered static routes, sub-2.5s mobile LCP, 0 CLS across all viewports.
- **Structured Data:** 143 validated Schema.org JSON-LD instances across technical articles, comparison matrices, and diagnostic tool landing pages.
- **Live Platform:** [https://webaudits.pro](https://webaudits.pro)

### 2. [AestheticArches.com](https://aestheticarches.com)
**Architectural & Interior Design Publication**
- **Role:** CMS architecture, technical SEO, custom Gutenberg block design, and automated publishing pipeline.
- **Stack:** WordPress, GeneratePress Premium, GenerateBlocks V2, LiteSpeed Cache, Cloudflare CDN.
- **Performance:** Strict zero-CLS layout budget, fluid `clamp()` typography scales, and responsive image optimizations.
- **Topical Architecture:** Semantic internal link graph connecting architectural styles, materials, and spatial planning guides.
- **Live Site:** [https://aestheticarches.com](https://aestheticarches.com)

---

## Four Flagship Diagnostic Engines

These four standalone repositories form the core analytical foundation of my technical SEO tooling:

### 1. [DOMHydrate](https://github.com/xcalibur73/dom-hydrate) (v1.1.0)
**Forensic CSR vs. SSR SEO Diff Engine & Dynamic DOM Tracer**
- **Problem:** Client-side JavaScript hydration frequently drops server-rendered Schema.org JSON-LD, injects unexpected `noindex` directives, or strips internal link anchors before search crawlers finish rendering.
- **Solution:** Compares raw server HTML against fully hydrated client DOM using native Chromium (`--headless=new --dump-dom`). Audits Open Graph and Twitter Card social crawler parity to detect preview blindspots.
- **Web Route:** [webaudits.pro/tools/hydration-audit](https://webaudits.pro/tools/hydration-audit) | **Tests:** 4/4 passing

### 2. [IndexTrace](https://github.com/xcalibur73/index-trace) (v1.1.0)
**Google Search Console Forensic Diagnostic & RFC 9309 Crawler Tracer**
- **Problem:** Search Console reports opaque exclusion buckets ("Page with redirect", "Blocked by robots.txt", "Soft 404") without identifying the exact failure layer.
- **Solution:** Traces redirect hops with latency measurements, flags protocol downgrades, locates the exact line number of blocking directives in `robots.txt` using RFC 9309 longest-match rules, and validates declared `Sitemap:` directives.
- **Web Route:** [webaudits.pro/tools/index-trace](https://webaudits.pro/tools/index-trace) | **Tests:** 15/15 passing

### 3. [SchemaGraph](https://github.com/xcalibur73/schema-graph) (v1.0.0)
**Cross-Page Entity & Knowledge Graph Integrity Tracer**
- **Problem:** Multi-page CMS deployments generate structured data independently per page, leading to unresolving `@id` URIs, orphan nodes, and attribute drift across templates.
- **Solution:** Parses Schema.org JSON-LD across an entire sitemap to construct a directed knowledge graph. Detects broken references, DFS circular loops, orphan entity nodes, publisher/author drift, and missing `sameAs` authority links.
- **Web Route:** [webaudits.pro/tools/schema-graph](https://webaudits.pro/tools/schema-graph) | **Tests:** 95/95 passing

### 4. [PayloadSniper](https://github.com/xcalibur73/payload-sniper) (v1.1.0)
**Interaction to Next Paint (INP), Long Tasks & Script Bloat-Tracer**
- **Problem:** Heavy JavaScript bundles cause main-thread contention during page load, creating high interaction latency risks on mobile hardware.
- **Solution:** Profiles Long Tasks (> 50ms) and Total Blocking Time (TBT) via Chrome DevTools Protocol with 4x CPU throttling. Ingests W3C Resource Timing to rank the Top 5 heaviest scripts by uncompressed byte weight.
- **Web Route:** [webaudits.pro/tools/payload-sniper](https://webaudits.pro/tools/payload-sniper) | **Tests:** 10/10 passing

---

## Supporting Performance & Geometry Tooling

Compact diagnostic utilities developed to solve specific technical audit challenges:

| Tool | Focus Area | Technical Function | Platform Route |
|:---|:---|:---|:---|
| [OverflowTrace](https://github.com/xcalibur73/overflow-trace) | Viewport Geometry | Inspects DOM bounding client rects via Chromium CDP to locate horizontal viewport spill elements causing mobile usability failures. | [/tools/overflow-trace](https://webaudits.pro/tools/overflow-trace) |
| [ImgSpec](https://github.com/xcalibur73/img-spec) | LCP & Breakpoints | Compares natural image resolutions against rendered viewport dimensions to audit responsive breakpoint efficiency and byte waste. | [/tools/img-spec](https://webaudits.pro/tools/img-spec) |
| [LinkBleed](https://github.com/xcalibur73/link-bleed) | Link Equity Modeling | Simulates internal link equity distribution across site architectures using a power-iteration link model with damping factor calibration. | [/tools/link-bleed](https://webaudits.pro/tools/link-bleed) |
| [CitationPulse](https://github.com/xcalibur73/citation-pulse) | Generative Engine Optimization | Audits passage citability heuristics (based on Princeton KDD 2024 research), AI crawler access rules, and `/llms.txt` formatting. | [/tools/geo-audit](https://webaudits.pro/tools/geo-audit) |
| [ContextSilo](https://github.com/xcalibur73/context-silo) | Semantic Topical Vectors | Computes TF-IDF cosine similarity vectors across internal link anchors to detect context drift across topical clusters. | [/tools/context-silo](https://webaudits.pro/tools/context-silo) |

---

## Selected Empirical Case Studies & Benchmarks

Every benchmark follows a standardized, reproducible methodology (dataset, environment, command, raw telemetry, calculation formulas):

- **[12-Site Hydration Disparity Benchmark](https://github.com/xcalibur73/dom-hydrate/blob/main/BENCHMARKS.md)**: 33.3% of audited Next.js and Remix sites dropped structured data entities during client-side hydration, and 16.7% exhibited social crawler preview blindspots.
- **[RFC 9309 Crawler Directive Precedence Study](https://github.com/xcalibur73/index-trace/blob/main/BENCHMARKS.md)**: Documented line-level rule collisions across 12 production `robots.txt` files where subtle path differences reversed crawler permissions.
- **[12-Site Entity Graph Integrity Benchmark](https://github.com/xcalibur73/schema-graph/blob/main/BENCHMARKS.md)**: 58.3% of evaluated sites contained broken cross-page `@id` references, and 75% had zero `sameAs` disambiguation links on their primary `Organization` entity.
- **[Third-Party Script Weight & Main-Thread Cost](https://github.com/xcalibur73/payload-sniper/blob/main/BENCHMARKS.md)**: Quantified the correlation between uncompressed script payload sizes (> 1.0 MB) and main-thread Long Task frequency under 4x mobile CPU throttling.

---

## Engineering Standards

- **PEP 621 Standardized Packaging**: Every tool is packaged via `pyproject.toml` and installs cleanly via `pip install -e .`.
- **Automated CI Validation**: 180 unit tests across all 9 tools pass continuously on both Ubuntu and Windows runners.
- **Defensible Metric Taxonomy**: Clear distinction between Internet/W3C standards, official Google Search Central guidance, and project-derived heuristics.
- **Cross-Platform Hardening**: Built-in Unicode sanitization (`_safe_str`) prevents Windows console encoding crashes.

---

## Contact & Profile

- **Author**: @xcalibur73
- **Platform**: [WebAudits.pro](https://webaudits.pro)
- **Live Publication**: [AestheticArches.com](https://aestheticarches.com)
- **GitHub**: [github.com/xcalibur73](https://github.com/xcalibur73)
