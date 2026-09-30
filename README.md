# Sadikeen Firoz

Technical SEO Strategist and Systems Architect

I design automated web diagnostics, crawl engines, and performance auditing tools. My work focuses on rendering parity, crawler indexability, structured data validation, Generative Engine Optimization (GEO), and Core Web Vitals under real-world mobile constraints.

[WebAudits.pro](https://webaudits.pro) &middot; [AestheticArches.com](https://aestheticarches.com) &middot; [GitHub Repositories](https://github.com/xcalibur73?tab=repositories)

---

## Flagship Systems

### [WebAudits.pro](https://webaudits.pro)
Full-stack web auditing platform and open-source diagnostic suite ([github.com/xcalibur73/webaudits](https://github.com/xcalibur73/webaudits)). Evaluates crawl behavior, server-side hydration drift, JSON-LD knowledge graphs, and AI search citability across live production websites.
- [Public Benchmark Dataset: 100 Domains Across 5 Frameworks](https://github.com/xcalibur73/webaudits/blob/main/benchmarks/DATASET.md)
- [Production Case Study: AestheticArches Technical Remediation](https://github.com/xcalibur73/webaudits/blob/main/case-studies/aesthetic-arches.md)

### [VitalsSniper](https://github.com/xcalibur73/vitalssniper)
In-browser Core Web Vitals diagnostic engine and Chrome extension. Measures real-time Interaction to Next Paint (INP) with Long Animation Frame attribution, Largest Contentful Paint (LCP) subparts, and DOM tree depth directly within active browser tabs.

### [AestheticArches.com](https://aestheticarches.com)
Architectural publication running custom automated content pipelines, 0 CLS responsive layouts, and structured Schema.org entity graphs. Serves as the primary production testbed for rendering parity and automated publishing workflows.

---

## Open-Source Diagnostic Engines

Each tool operates as an independent Python CLI package with automated test suites, structured JSON output, and an interactive counterpart on [WebAudits.pro/tools](https://webaudits.pro/tools):

| Tool | Diagnostic Scope | Interactive Version |
| :--- | :--- | :--- |
| [DOMHydrate](https://github.com/xcalibur73/dom-hydrate) | Compares raw SSR HTML against hydrated client DOM to detect rendering drift | [Hydration Audit](https://webaudits.pro/tools/hydration-audit) |
| [IndexTrace](https://github.com/xcalibur73/index-trace) | Evaluates indexability, canonical loops, redirect chains, and RFC 9309 robots rules | [Index Trace](https://webaudits.pro/tools/index-trace) |
| [LinkBleed](https://github.com/xcalibur73/link-bleed) | Traverses internal link graphs, calculates PageRank distribution, and flags orphan nodes | [Link Bleed](https://webaudits.pro/tools/link-bleed) |
| [ContextSilo](https://github.com/xcalibur73/context-silo) | Audits anchor relevance, topical contiguity, and keyword cannibalization | [Context Silo](https://webaudits.pro/tools/context-silo) |
| [SchemaGraph](https://github.com/xcalibur73/schema-graph) | Builds, traverses, and validates interconnected Schema.org JSON-LD graphs | [Schema Graph](https://webaudits.pro/tools/schema-graph) |
| [CitationPulse](https://github.com/xcalibur73/citation-pulse) | Evaluates AI search citability, passage citability scoring, and llms.txt compliance | [GEO Audit](https://webaudits.pro/tools/geo-audit) |
| [PayloadSniper](https://github.com/xcalibur73/payload-sniper) | Profiles JavaScript execution cost, long tasks, and INP risks under CPU throttling | [Payload Sniper](https://webaudits.pro/tools/payload-sniper) |
| [ImgSpec](https://github.com/xcalibur73/img-spec) | Inspects responsive srcset delivery, viewport matching, and LCP priority tags | [Img Spec](https://webaudits.pro/tools/img-spec) |
| [OverflowTrace](https://github.com/xcalibur73/overflow-trace) | Identifies horizontal viewport overflows and pinpoints offending CSS/DOM nodes | [Overflow Trace](https://webaudits.pro/tools/overflow-trace) |
| [ProseLint](https://github.com/xcalibur73/prose-lint) | Deterministic editorial linter, style compliance validator, and content compiler | [Prose Lint](https://webaudits.pro/tools/prose-lint) |

---

## Technical Stack

- **Diagnostics & Crawling**: Python, Chromium DevTools Protocol (CDP), Playwright, Cheerio, BeautifulSoup
- **Frontend & Web Platform**: TypeScript, Next.js, React, Tailwind CSS, Chrome Extension APIs (Manifest V3)
- **Search & Architecture**: Core Web Vitals, Schema.org JSON-LD, RFC 9309 robots parsing, GEO / llms.txt standards
- **CMS & Publishing**: WordPress REST API, headless Next.js architectures, Gutenberg block engines

---

## Contact

- GitHub: [@xcalibur73](https://github.com/xcalibur73)
- Platform: [webaudits.pro](https://webaudits.pro)
- Email: [sfsadik22@gmail.com](mailto:sfsadik22@gmail.com)
