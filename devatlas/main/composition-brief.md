# Hyperframes Composition Brief: DevAtlas — main (default tone)

## Objective
20s landscape launch brag for DevAtlas showing the working-app flow:
search → trending → freshness → logo. Customer-acquisition framing.

## Output
- Composition: /home/z/my-project/builds/brag-devatlas/main/composition/
- Render: main/brag.mp4 · 1920x1080 · 20.0s · 30fps

## Source Material
- Live site bundles (fetched): title/meta/copy per brag-plan.md
- Product name: DevAtlas · URL: devtomb.netlify.app
- Copy verbatim: "Search developer resources...", "Hottest Tools",
  "Developer tools gaining the most GitHub stars right now.", "Hidden Gems",
  "Curated from the best awesome-lists on GitHub. Quality over quantity.",
  "Always Fresh", "Automated crawlers update star counts, forks, and trends daily.",
  "Instant Search", "30,000+ indexed"
- Recreated UI: search card + result rows (Apache Kafka / Apache Airflow /
  Apollo GraphQL — demonstrative rows; star counts illustrative)

## Creative Direction
- Tone preset: default · Direction: "the quiet power of a searchable atlas"
- Hook (0-2s): "30,000+ developer tools." slams over ghost numerals
- Outro: wordmark slam beat-locked 16.02 (vol-1 strong cue) + tagline + URL

## Visual Identity
Per brag-plan.md palette block. Fonts: Archivo Black (display), JetBrains Mono (all
product UI). Accent #6467f2 large-only; #8a8cf7 for small accent text.

## Storyboard
1. HOOK 0-3.5 — headline slam, ghost "30,000+" drift, sub "Searchable. Ranked. Daily."
2. SEARCH FLOW 3.5-8.5 — card in, "ap" typed char-by-char (keypress SFX), 3 rows
   beat-locked 5.53/6.03/6.52
3. TRENDING 8.5-12.5 — "Hottest Tools" rank rows 9.02/9.52/10.02 w/ count-ups +
   "Hidden Gems" quality-over-quantity card
4. ALWAYS FRESH 12.5-16 — refresh spin, verbatim crawler copy, 5 category chips
   13.01→15.02 (every other beat)
5. OUTRO 16-20 — wordmark slam @16.02, tagline, URL chip

## Audio
- Role: warm upbeat bed, product-UI SFX · Music: bed-main.mp3 (vol-1, trimmed 20s,
  fade 18.2→20 baked) · volume 0.34 · track 10
- Cue guidance: assets/music/cues vol-1 preset — locks: 5.53/6.03/6.52 (grid),
  9.02/9.52/10.02 (grid), 16.02 (strong)
- Audio-reactive: subtle — ghost numerals scale ±3% on bass; ambient glow opacity
  ±10% on overall RMS via audio-data.js per-frame tl.call sampling
- SFX: keypress typing, drop/click rows+chips, impactSoft hook, impactBell logo
- Track allocation: music 10, SFX 11+ unique indices, ids unique

## Hyperframes Instructions
Per brag step-3: local gsap.min.js; single paused timeline at window.__timelines
["devatlas-main"]; no CSS/GSAP transform conflicts (fromTo only); no autoAlpha on
clips; every audio has id; no crossorigin; finite repeats only; check gate before
render; render --quality looks → poster bake → share copy.
