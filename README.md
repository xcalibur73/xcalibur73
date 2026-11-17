# Sadikeen Firoz

Founder & Systems Engineer at [WebAudits.pro](https://webaudits.pro) based in Dhaka, Bangladesh. Specializing in client-side web performance forensics, Core Web Vitals telemetry engines, Chromium Manifest V3 architecture, and Model Context Protocol (MCP) tooling for AI-assisted engineering.

[![WebAudits.pro](https://img.shields.io/badge/Platform-WebAudits.pro-blue.svg)](https://webaudits.pro)
[![Chrome Web Store](https://img.shields.io/badge/Chrome_Web_Store-VitalsSniper-4285F4?logo=googlechrome&logoColor=white)](https://chromewebstore.google.com/detail/vitalssniper-proof-of-flaw/ohabpnaccigjhkkebjofhpmebofgpbeb)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## Flagship Open-Source Ecosystem

### [VitalsSniper](https://github.com/xcalibur73/vitalssniper)
Production Manifest V3 browser extension for forensic in-browser DOM complexity scanning, Google web-vitals v4 3-phase INP latency attribution, and W3C Long Animation Frames (LoAF) correlation directly in Chromium browsers with zero external runtime dependencies.
- Subpart INP attribution: separates Input Delay, Processing Duration, and Presentation Delay against the 8ms VSYNC boundary.
- Script culprit isolation: identifies the exact invoker function, source URL, and character offset causing main-thread execution pauses.
- Session-isolated crawler emulator: evaluates rendering under Googlebot Smartphone, Googlebot Desktop, Bingbot, and GPTBot personas using `chrome.declarativeNetRequest` session rules.

### [webaudits-cli](https://github.com/xcalibur73/webaudits-cli)
Zero-dependency command-line utility for automated CI/CD performance testing and terminal auditing. Evaluates raw origin server response latency (TTFB), edge CDN infrastructure, modern wire compression (Brotli), and Schema.org structured data graphs in under 2 seconds.
```bash
npx webaudits https://example.com
```

### [webaudits-mcp](https://github.com/xcalibur73/webaudits-mcp)
Official Model Context Protocol (MCP) server enabling AI development environments (Cursor, Claude Desktop, Windsurf) to execute real-time web audits, inspect DOM bloat, evaluate AI crawler readiness (`/llms.txt`), and debug performance bottlenecks directly from editor workflows.

### [webaudits-seo-extractors](https://github.com/xcalibur73/webaudits-seo-extractors)
Zero-dependency ESM forensic extractors for sitemap XML hierarchies, robots.txt AI scraper governance (RFC 9309 compliance), and tracking pixel / Google Tag Manager tag contention audits.

---

## Technical Focus & Systems Architecture

- Browser Engine Telemetry: Chromium Blink internals, W3C PerformanceObserver, Long Animation Frames (LoAF), Event Timing API, Layout Instability API, and memory lifecycle analysis.
- Extension Architecture: Manifest V3 service workers, `declarativeNetRequest` session rules, linear memory pooling (`ArrayPool`), and read/write storage synchronization barriers (`AsyncLock`).
- Full-Stack Web Infrastructure: Next.js 14, TypeScript, Node.js ESM, Cloudflare Pages & D1 edge databases, Tailwind CSS, and Remotion video synthesis.
- Machine-Readable Knowledge Graphs: Advanced Schema.org JSON-LD `@graph` architecture and generative engine optimization (GEO / llms.txt).

---

## Connect & Collaborate

- Platform: [https://webaudits.pro](https://webaudits.pro)
- Chrome Web Store: [VitalsSniper Extension](https://chromewebstore.google.com/detail/vitalssniper-proof-of-flaw/ohabpnaccigjhkkebjofhpmebofgpbeb)
- Direct Email: [sfs@webaudits.pro](mailto:sfs@webaudits.pro)
