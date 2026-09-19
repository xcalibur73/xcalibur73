# xcalibur73

[WebAudits.pro](https://webaudits.pro) | [AestheticArches.com](https://aestheticarches.com)

---

## Featured Tools & Production Projects

### [DOMHydrate](https://github.com/xcalibur73/dom-hydrate)
Forensic CSR vs SSR SEO diff engine. Compares raw server HTML against fully hydrated client DOM using native Chromium (`--headless=new --dump-dom`). Detects dropped Schema.org JSON-LD scripts, client-injected noindex directives, and internal link graph discrepancies before deployment.

### [CitationPulse](https://github.com/xcalibur73/citation-pulse)
Generative Engine Optimization (GEO) and AI citability auditor. Implements empirical scoring rules from Princeton University KDD 2024 research. Evaluates optimal passage length (134-167 words), statistical evidence (+37%), attribution markers (+40%), robots.txt permissions for search retrieval bots (OAI-SearchBot, Claude-SearchBot, PerplexityBot), and /llms.txt syntax.

### [IndexTrace](https://github.com/xcalibur73/index-trace)
Google Search Console emergency triage utility and RFC 9309 crawler tracer. Follows redirect chains hop by hop, detects circular loops, flags SSL protocol downgrades, and pinpoints the exact line number of blocking directives in robots.txt using standard longest-match precedence. Classifies soft-404 patterns on HTTP 200 responses and outputs ordered developer remediation steps.

### [OverflowTrace](https://github.com/xcalibur73/overflow-trace)
Mobile viewport horizontal overflow and layout breakage tracer. Emulates mobile screens (iPhone SE 375px, iPhone 14/15 390px, compact 320px) using native headless Chromium via CDP. Isolates exact bounding client rect spills, diagnoses rogue 100vw container offsets and unconstrained flex children, and outputs drop-in CSS remediation recipes.

### [SchemaGraph](https://github.com/xcalibur73/schema-graph)
Cross-page entity and knowledge graph integrity tracer. Constructs in-memory directed graphs across multi-page site clusters, detects broken @id URI references, circular loops, orphan entity nodes, publisher metadata drift, and missing sameAs Knowledge Graph disambiguation signals.

### [ImgSpec](https://github.com/xcalibur73/img-spec)
Responsive viewport breakpoint and Largest Contentful Paint (LCP) image auditor. Emulates 5 responsive viewports via Chromium CDP, detects oversized desktop hero images served to mobile screens, calculates pixel waste ratios, audits fetchpriority and lazy-loaded hero defects, and generates drop-in responsive <picture> markup with calibrated srcset breakpoints.

### [PayloadSniper](https://github.com/xcalibur73/payload-sniper)
Edge-cached code split, INP and Core Web Vitals bloat-tracer. Profiles JavaScript hydration delays, main-thread Long Tasks (>50ms), and third-party script congestion (GTM, Meta, Hotjar, Klaviyo) using Chrome DevTools Protocol performance timelines.

### [VitalsSniper PRO](https://github.com/xcalibur73/vitalssniper-portal)
Manifest V3 Chrome extension for in-browser web performance audits. Scans DOM depth, serialized document markup size, mobile viewport scaling restrictions, and Schema.org syntax in under 50ms without third-party API dependencies. Generates technical audit teardowns and exportable CSV summaries.

### [WebAudits.pro](https://webaudits.pro)
Technical performance intelligence and audit platform. Houses 115 pre-rendered static Next.js routes with zero layout shift, sub-2.5s mobile LCP, and 143 validated Schema.org JSON-LD instances across technical articles, reviews, and interactive diagnostic tools.

### [AestheticArches.com](https://aestheticarches.com)
Architectural and interior design publication built on GeneratePress with native Gutenberg blocks, LiteSpeed server caching, and Cloudflare CDN. Maintained with a zero-CLS layout budget and structured semantic topical clusters.

---

## Empirical Benchmarks & Field Studies

Each diagnostic tool includes documented empirical benchmarks and case studies gathered while beta testing on random sites:
- [DOMHydrate 12-Site SSR vs CSR Study](https://github.com/xcalibur73/dom-hydrate/blob/main/BENCHMARKS.md): Measures DOM node inflation (+13% to +30% on client-rendered SPAs) and critical link parity losses gathered while beta testing on random sites.
- [CitationPulse 12-Site GEO Index](https://github.com/xcalibur73/citation-pulse/blob/main/BENCHMARKS.md): Audits crawler access policies (41.7% of surveyed sites block training scrapers while permitting search retrieval bots) and Princeton KDD citability factors evaluated while beta testing on random sites.
- [IndexTrace Forensic Case Studies](https://github.com/xcalibur73/index-trace/blob/main/BENCHMARKS.md): Analyzes line-level RFC 9309 collisions (such as line 238 on GitHub), 4,100ms+ cumulative redirect latency, and soft-404 heuristics captured while beta testing on random sites.
- [OverflowTrace Mobile Viewport Benchmarks](https://github.com/xcalibur73/overflow-trace/blob/main/BENCHMARKS.md): Evaluates horizontal scroll overflow and containment across production layouts and synthetic breakages gathered while beta testing on random sites.
- [SchemaGraph 12-Site Entity Integrity Study](https://github.com/xcalibur73/schema-graph/blob/main/BENCHMARKS.md): Audits cross-page @id reference resolution (58.3% of surveyed sites contain broken references), orphan entity node rates, and publisher metadata drift.
- [ImgSpec 12-Site Viewport & LCP Study](https://github.com/xcalibur73/img-spec/blob/main/BENCHMARKS.md): Measures mobile pixel waste (58.4% of downloaded image pixels discarded on media sites), site-wide lazy-loaded LCP anti-patterns, and modern format adoption.
- [PayloadSniper 12-Site Hydration & INP Study](https://github.com/xcalibur73/payload-sniper/blob/main/BENCHMARKS.md): Audits main-thread execution costs (third-party tracking tags account for 71.4% of total blocking time on publishing properties) and synthetic INP vulnerability.

---

## Technical Stack

| Domain | Tooling and Technologies |
|---|---|
| Core Web Vitals | INP optimization, LCP acceleration, 0-CLS layouts, DOM profiling, TTFB tuning, edge caching |
| Frontend | Next.js App Router, TypeScript, React, Tailwind CSS, Chrome Extensions (Manifest V3) |
| Technical SEO | Schema.org JSON-LD, Google Search Console, llms.txt, entity graphs, crawl log analysis |
| CMS Architecture | GeneratePress, Gutenberg custom blocks, LiteSpeed Cache, Redis object cache, Cloudflare CDN |
| Automation & Headless | Chromium CDP automation, Chrome DevTools profiling, Python, Firecrawl |

---

## GitHub Statistics

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=xcalibur73&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=xcalibur73&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" />
</div>

---

## Platforms

- [WebAudits.pro](https://webaudits.pro): Technical performance intelligence and audit platform.
- [AestheticArches.com](https://aestheticarches.com): Architecture publication with zero-CLS layout budget.

