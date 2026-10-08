# Brag Plan: DevAtlas — multi-variant promo system (8 videos)

Operator: Super Z · Task 26 · Commissioned by Ansari Bilal ("bring in more customers")

## What is this app?
DevAtlas (https://devtomb.netlify.app/) is a searchable index of 30,000+ curated
developer tools, APIs, datasets and OSS, refreshed daily from GitHub awesome-lists,
with daily trending leaderboards and hidden gems.

## The angle
GitHub maintains the lists; DevAtlas turns them into a searchable, daily-ranked atlas.
The video treats "30,000+" as the star number and shows the real product verbs:
search → compare → rank → discover. Not a feature tour — a working-app demo.

## Source grounding (all claims below come from the live site bundles)
- "Search 30,000+ curated developer tools, APIs, datasets, and open source software
  from GitHub awesome lists. Daily trending leaderboards and hidden gems." (meta)
- "Curated from the best awesome-lists on GitHub. Quality over quantity."
- "Automated crawlers update star counts, forks, and trends daily."
- "Developer tools gaining the most GitHub stars right now."
- "Search developer resources..." (search placeholder)
- "Instant Search" · "Hidden Gems" · "Hottest Tools" · "Always Fresh"
- "Automated discovery" · "Compare Developer Tools" · "Browse by Category"
- "Get weekly trends in your inbox" · "Explore Developer Resources"
- Real index entries seen in bundle: Apache Airflow, Apache Kafka, Animation,
  API-First Backend, Authentication, Backend Dev, Mobile App Toolkit, ETL pipelines.
- og:image exists at https://devtomb.netlify.app/og-image.png (1920x1080)

## Visual identity (extracted from the site's CSS custom properties — exact)
- Background: hsl(0 0% 4.3%)  → #0b0b0b
- Card/surface: hsl(0 0% 7.1%) → #121212
- Border: hsl(0 0% 14%)        → #242424
- Text: hsl(220 13% 91%)       → #e4e7ee
- Muted text: hsl(220 9% 56%)  → #8b93a4
- Accent: hsl(239 84% 67%)     → #6467f2 (indigo)
- Support: #22c55e (green, stars/up), #eab308 (yellow), #ef4444 (red)
- Radius: 12px (site uses 0.75rem)
- Display font: Archivo Black (embedded, heavy display) — hooks/logo
- Data font: JetBrains Mono (embedded, mono) — everything product-UI: search bar,
  stats, labels, chips. Register story: terminal truth vs. atlas scale.
- Never weight 700/900 on Archivo Black (ships 400 only).

## Audio system
- Music (bundled, ende.app, CC-licensed for use): vol-1 = default/longer/detailed/reels;
  vol-10 = chaotic/twitter; vol-12 = cinematic/producthunt. Volume 0.30-0.38.
- Cue presets exist for all three tracks (strong cues + beat grids) — 1-3 locks per video.
- SFX: keyboard keypresses for typing; card/drop for UI reveals; impactSoft for scene
  slams; impactBell for logo; glitch/dice accents only in chaotic. SFX 0.55-0.8.
- Audio-reactive: subtle per brag law — hero ghost numerals + accent glow breathe with
  RMS (extract-audio-data.py output; numpy present). No equalizer bars, no waveforms.
- Determinism: per-frame tl.call sampling on the shared paused timeline.

## Shared product-UI recreations (the "show the thing" inventory)
1. Search bar: rounded-12 card, 2px border, magnifier glyph, mono placeholder
   "Search developer resources...", caret blink during typing, dropdown result rows.
2. Leaderboard row: rank chip (#1/#2/#3), tool name (mono), star count with ▲,
   green delta. Numbers are illustrative mock data (labeled in plan) — grounded in
   "star counts, forks, and trends daily" copy; no invented superlatives.
3. Category chips: rounded-full bordered pills — real category names.
4. Compare tray: two mini tool cards + "Compare Developer Tools" real button copy.
5. Ghost atlas numeral field: oversized "30,000+" mono ghost at 6-8% opacity drift.

## Variant roster (all: landscape 1920x1080 unless noted; 15-25s law)
| Dir          | Tone       | Dur | Format      | Hook | Beat locks (track)      |
|--------------|-----------|------|-------------|------|--------------------------|
| main/        | default   | 20s  | landscape   | "30,000+ developer tools." | 3.02, 12.0, 16.02 (vol-1) |
| longer/      | default+  | 25s  | landscape   | same, + compare scene + newsletter scene | 3.02, 17.02 (vol-1) |
| cinematic/   | cinematic | 22s  | landscape   | "Every tool. One atlas." | 8.74, 17.47 (vol-12) |
| chaotic/     | chaotic   | 16s  | landscape   | "STOP DIGGING THROUGH AWESOME LISTS." | 15.28→logo, vol-10 grid |
| detailed/    | app-store | 25s  | landscape   | 4 feature cards + categories + compare | 8.74, 17.47 (vol-12) |
| reels/       | default   | 18s  | 1080x1920   | vertical: hook → type → rows → gems → CTA | 3.02, 16.02 (vol-1) |
| producthunt/ | app-store | 20s  | landscape   | "DevAtlas is live" launch framing | 17.47 (vol-12) |
| twitter/     | chaotic-lite | 15s | landscape | "Still grepping awesome lists?" fast cut | 15.28 (vol-10) |

Reading-time floors respected: headline ≥1.2s settled; rows snap to every other beat
when text; fast-in + hold, never flash.

## Mock-data discipline
Tool names shown in recreated UI: Apache Airflow, Apache Kafka (seen in bundle) plus
neutral dev-tool names (Postman, pgAdmin, MinIO style) presented as generic entries.
Star counts are demonstrative UI, never framed as real claims; no numbers attributed
to a real tool beyond the site's own claims.

## Share copy (canonical per dir in <dir>/share-copy.txt; variants below)
- main: "GitHub made the awesome lists. DevAtlas makes them searchable — 30,000+ dev
  tools, APIs and datasets with daily trending leaderboards."
- reels: "POV: you find the perfect dev tool in 9 seconds. 30,000+ tools, one atlas."
- twitter: "Still digging through awesome lists? DevAtlas indexes 30,000+ tools with
  daily trending leaderboards. Search it:"
- producthunt: "DevAtlas — daily trending leaderboards for 30,000+ developer tools,
  curated from GitHub awesome lists. Today: launching on the atlas itself."
- chaotic: "30,000+ DEV TOOLS. ONE ATLAS. ZERO EXCUSES."
- cinematic: "Every tool. One atlas. DevAtlas."
- longer/detailed: variants of main with CTA to devtomb.netlify.app

## Delivery contract
1. Per dir: composition-brief.md + composition/ (index.html, assets/) + brag.mp4 + brag.jpg + share-copy.txt
2. Gate: `npx hyperframes check` = 0 errors before any render.
3. Render `--quality looks` (delivery if time allows for reels/twitter), verify
   duration via ffprobe, poster-bake frame 0, sendVideo to Telegram chat
   1263089875 immediately after each render.
4. Then: git release push + worklog/brain updates per §23-28 closing protocol.
