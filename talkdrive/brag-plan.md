# Brag Plan: TALKDRIVE — 7-variant promo set

Operator: Super Z · Task 27 · Commissioned by Ansari Bilal ("bring in more customers").
Part of the 10-project rest-of-portfolio run (DevAtlas 8-cut set shipped as Task 26).

## What is this?
TALKDRIVE — Turn any portrait into a talking-head video. Canonical link: https://github.com/Bilal140202/TalkDrive_by_BilalAnsari

## Source grounding (FACT)
Copy comes from the user's own llms.txt + me.json + live site bundles + project README.
- Site copy mined from the deployed bundle; claims on screen are verbatim or near-verbatim.
- Illustrative UI (mock rows, wizard steps, chat text) depicts the product's real features;
  specific row contents are demo data, labeled in the brief where invented.
- Stats on screen: 2 inputs — photo + audio · 512px FlashHead output clip · 16:9 final compositor.

## Visual identity
- Palette: bg #0a0a12, surface #12121e, accent #d946ef — grounded in the
  site's theme-color / bundle CSS (privacythink pure #000; convertfilesnow light indigo; others dark).
- Fonts (hyperframes font registry): display "Archivo Black", sans-serif, data "Space Mono", monospace.
- Register: display for hooks/wordmarks; mono for everything product-UI.

## Audio system
- Music (ende.app, CC, bundled): longer/detailed/reels = vol-1; chaotic/twitter = vol-10;
  cinematic/producthunt = vol-12. Bed 0.30–0.36. SFX 0.38–0.75 (keyboard typing, UI drops,
  impact slams, logo bell). Cue plan: scene entrances land on sfx; no audio-reactive sampling
  (v0.8.141 tl.call TDZ bug — ambient tweens instead, per DevAtlas finding).

## The angle
One photo. One talking head. — the video shows the real product verbs, not a feature tour.
Every cut: hook in the first 2-3s, at least one real product-UI recreation, outro with the canonical link.

## The 7 cuts
| File | Len | Format | Shape |
|------|-----|--------|-------|
| `brag-longer.mp4` | 25s | 1920×1080 | longer — hook → d1 → d2 → d3 → chips → outro |
| `brag-detailed.mp4` | 25s | 1920×1080 | detailed — hook → d1 → d2 → d3 → stats → outro |
| `brag-cinematic.mp4` | 22s | 1920×1080 | cinematic — hook → stats → d1 → quote → outro |
| `brag-producthunt.mp4` | 20s | 1920×1080 | producthunt — launch → d1 → d2 → checklist → outro |
| `brag-reels.mp4` | 18s | 1080×1920 | reels — hook → d1 → d2 → stats → outro |
| `brag-chaotic.mp4` | 16s | 1920×1080 | chaotic — hook → d1 → d2 → d3 → outro |
| `brag-twitter.mp4` | 15s | 1920×1080 | twitter — hook → d1 → stats → outro |

## "Show the thing" inventory
- d1: pipeline — Photo + audio in, video out
- d2: grid — Colab-native
- d3: grid — The parts that used to break
- stats wall: THE RUN, IN NUMBERS
- chips: One notebook. Zero setup.
- checklist: WHY TALKDRIVE
- launch card: TalkDrive
