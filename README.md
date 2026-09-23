# Sadikeen Firoz

Systems Engineer and Technical SEO Specialist

I build open-source diagnostics for rendering parity, crawl behavior, structured data, AI-search visibility, and browser performance.

[WebAudits.pro](https://webaudits.pro) | [AestheticArches.com](https://aestheticarches.com) | [GitHub repositories](https://github.com/xcalibur73?tab=repositories)

## Focus

| Area | Work |
| --- | --- |
| Rendering | Compare server HTML with the hydrated DOM to find content, metadata, and link changes. |
| Crawlability | Trace redirects, inspect robots.txt rules, and diagnose indexability conflicts. |
| Structured data | Validate linked-data relationships across pages and surface broken entity references. |
| Performance | Profile script cost, long tasks, image delivery, and mobile layout failures. |

## Flagship diagnostic suite

[WebAudits](https://github.com/xcalibur73/webaudits) is the unified open-source technical diagnostics suite powering [WebAudits.pro](https://webaudits.pro), covering Crawl Forensics, SSR/Hydration Parity, Knowledge Graphs, Runtime Performance, and AI-Search Citability. It integrates the 10 specialized engines below and includes empirical production case studies:

- Architecture & Suite Hub: [github.com/xcalibur73/webaudits](https://github.com/xcalibur73/webaudits)
- Interactive Suite & Tools Hub: [webaudits.pro/tools](https://webaudits.pro/tools)
- Production Case Study: [AestheticArches Technical Remediation](https://github.com/xcalibur73/webaudits/blob/main/case-studies/aesthetic-arches.md)
- Public Benchmark Dataset: [100 URLs across 5 Web Frameworks](https://github.com/xcalibur73/webaudits/blob/main/benchmarks/DATASET.md)

## Specialized diagnostic engines

| Engine | Focus & Architecture | Interactive Web Tool |
| --- | --- | --- |
| [DOMHydrate](https://github.com/xcalibur73/dom-hydrate) | Compares server-rendered HTML with the hydrated DOM and traces rendering differences that affect search visibility. | [webaudits.pro/tools/hydration-audit](https://webaudits.pro/tools/hydration-audit) |
| [IndexTrace](https://github.com/xcalibur73/index-trace) | Diagnoses indexability, redirect chains, crawler behavior, and RFC 9309 robots.txt conflicts. | [webaudits.pro/tools/index-trace](https://webaudits.pro/tools/index-trace) |
| [LinkBleed](https://github.com/xcalibur73/link-bleed) | Maps internal links, calculates PageRank, and finds orphaned pages. | [webaudits.pro/tools/link-bleed](https://webaudits.pro/tools/link-bleed) |
| [ContextSilo](https://github.com/xcalibur73/context-silo) | Audits anchor-text relevance, topical contiguity, and keyword cannibalization. | [webaudits.pro/tools/context-silo](https://webaudits.pro/tools/context-silo) |
| [SchemaGraph](https://github.com/xcalibur73/schema-graph) | Builds and validates cross-page Schema.org JSON-LD graphs. | [webaudits.pro/tools/schema-graph](https://webaudits.pro/tools/schema-graph) |
| [CitationPulse](https://github.com/xcalibur73/citation-pulse) | Audits AI-search citability and creates llms.txt recommendations. | [webaudits.pro/tools/geo-audit](https://webaudits.pro/tools/geo-audit) |
| [PayloadSniper](https://github.com/xcalibur73/payload-sniper) | Profiles JavaScript cost, INP risks, and Core Web Vitals under device constraints. | [webaudits.pro/tools/payload-sniper](https://webaudits.pro/tools/payload-sniper) |
| [ImgSpec](https://github.com/xcalibur73/img-spec) | Tests responsive-image delivery, viewport behavior, and LCP image configuration. | [webaudits.pro/tools/img-spec](https://webaudits.pro/tools/img-spec) |
| [OverflowTrace](https://github.com/xcalibur73/overflow-trace) | Finds mobile horizontal overflow and identifies the elements responsible. | [webaudits.pro/tools/overflow-trace](https://webaudits.pro/tools/overflow-trace) |
| [ProseLint](https://github.com/xcalibur73/prose-lint) | Deterministic editorial compiler, deslop quality gate, and multi-channel content transpiler. | [webaudits.pro/tools/prose-lint](https://webaudits.pro/tools/prose-lint) |

Each project ships as a Python package with a CLI, machine-readable output, and tests.

## Production work

| Project | Scope |
| --- | --- |
| [WebAudits.pro](https://webaudits.pro) | Technical SEO and performance auditing platform. |
| [AestheticArches.com](https://aestheticarches.com) | Architectural and interior-design publication with custom WordPress tooling. |

## Stack

Python, TypeScript, Chromium DevTools Protocol, Playwright, Next.js, WordPress, structured data, and web performance APIs.

## Contact

[@xcalibur73](https://github.com/xcalibur73) | [WebAudits.pro](https://webaudits.pro)
