# TEST REPORT — United 18 Clothing Co
> Date: 2026-09-10 | Tester: Senior Engg | Segment: Retail / Clothing store

## Build
- [x] `npm install` PASS (87 packages)
- [x] `npm run build` PASS (vite 5.4.21, 4 modules, 0 warnings)
- dist sizes: index.html 14.27 kB (gzip 3.68) / CSS 12.33 kB (gzip 3.33) / JS 1.20 kB (gzip 0.63) — dist total 40K, well under perf budget (<200KB JS, <1.5MB total)

## Static checks (all PASS)
- [x] tel:+919164686886 present (7 refs: hero + mobile Call Now + contact + FAQ)
- [x] Google Maps URL present (7 refs: Directions + reviews + contact + footer)
- [x] JSON-LD ClothingStore schema present (application/ld+json ×1, rating 4.5)
- [x] H1 present, semantic sections, skip link, aria-expanded on nav toggle, year hook
- [x] No lorem ipsum, no invented hours/prices (call-CTA fallback)
- [x] Images have alt / placeholders labeled, lazy-ready

## Pending (requires preview + device lab before Deployed)
- [ ] Lighthouse CI mobile+desktop (target 90/95/95/95)
- [ ] Playwright E2E + axe (0 serious) + linkinator
- [ ] Screenshots 360/768/1440 attached to PR
- [ ] GitHub Pages deploy verify (200 + base path assets)

## Verdict: BUILT + STATIC QA PASS → ready for full QA + separate repo deploy

## Maps embed + README (2026-09-15)
- [x] Google Maps iframe embed added to #visit panel (lazy-loaded, `output=embed`, query fused from page's own Maps URL)
- [x] Per-site README.md added (live link, owner update guide)
