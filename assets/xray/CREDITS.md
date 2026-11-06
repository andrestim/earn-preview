# X-ray key visuals (trial)

Shown only with `?kv=xray` (C, the manifold), `?kv=xray-a` (the connector) or `?kv=xray-d` (the lock); see `src/site/theme.ts` `keyVisual()`.

- Source: generated, `asset-requests/xray/output/api-broker-xray-{c,a,d}.png` (Codex image_gen, 2026-10-30).
- Export: `python scripts/export_xray.py <src> public/assets/xray/api-broker xray-<v> --pad 1.8 --shift 0.85` (C: `--pad 1.3 --shift 1.0`, larger and bleeding off the right edge). Blacks are lifted to the page background, the object sits on a 1.8x canvas, and a 2400px retina set is written.

Round 8 (2026-10-31): xray-turbofan (market-maker), xray-vaultdoor and xray-safe (otc), xray-rowing2 (affiliate), xray-chip and xray-gpu (api-broker, comparison only). OpenAI image_gen via Codex; sources in asset-requests/xray/output, exported with scripts/export_xray.py --pad 1.5 --shift 1.0.
xray-bridge (api-broker): round 8 follow-up, copper accent desaturated and dimmed to match the series, exported --pad 1.5 --shift 1.0.
xray-rowing2large (pad 1.2, shift 0.85) and xray-rowing2vertical (rotated 90°, bow up, top 30% cropped, placed right) from affiliate-xray-rowing-v2.png.
Gold theme: every plate also graded to gold/ (gold body, bronze accent) by scripts/gold_xray.py; rerun it after any new export.

## Round 11 (2026-11-01)

| File | Source | Treatment |
| --- | --- | --- |
| `otc/xray-vaultclosed-*` | `asset-requests/xray/output/otc-xray-vault-closed.png` | `export_xray.py --pad 1.45 --shift 0.88 --portrait 0.33,1.0`; now the OTC default |
| `otc/xray-fig-{binoculars,bell,key}-{720,1080}.webp` | `otc-xray-binoculars.png`, `otc-xray-bell.png` (round 10), `otc-xray-key.png` (round 10) | black lifted to #0b0c0e, resized; shown in X-ray mode in place of the loupe, bell and key vignettes |
| `market-maker/xray-fig-metronome-{720,1080}.webp` | `market-maker-xray-metronome.png` | as above; replaces the metronome figure in X-ray mode |

Gold versions under `gold/` from `scripts/gold_xray.py`. The round-3 section figures (Broker market/support/commission, Affiliate payouts/team, OTC block) are not used: they fail the silhouette test.

## Round 12 (2026-11-01)

| File | Source | Treatment |
| --- | --- | --- |
| `api-broker/xray-fig-{plug,headset,hourglass}-{720,1080}.webp` | `asset-requests/xray/output/api-broker-xray-{plug,headset,hourglass}.png` | black lifted to #0b0c0e, resized; the plug recentred and scaled to 84% of the width. Replace the market, support and commission vignettes in X-ray mode |
| `affiliate/xray-fig-{megaphone,pen}-{720,1080}.webp` | `affiliate-xray-megaphone.png`, `affiliate-xray-pen.png` | as above; the pen recentred at 78% width. Replace the payouts and team figures |
| `otc/xray-fig-hook-{720,1080}.webp` | `otc-xray-hook.png` | as above. Replaces the block figure in Execution |

Gold versions under `gold/` from `scripts/gold_xray.py`. All six passed the silhouette test.

## Institutions (2026-11-01)

| File | Source | Treatment |
| --- | --- | --- |
| `institution/xray-lighthouse-*` | `asset-requests/institution/output/institution-xray-lighthouse.png` | `export_xray.py --pad 1.12 --shift 1.0 --portrait 0.40,0.95`; the X-ray hero |
| `institution/xray-fig-card-kv-{otc,market-maker,caas}-{720,1080}.webp` | `institution-xray-kv-card-{otc,market-maker,caas}.png` | `export_xray.py --figure --pad 1.08 --bg #101114`: black lifted to the card surface, centred. Each card is its programme's X-ray key visual in miniature (vault door, turbofan, rack with a drawn module) |
| `institution/xray-fig-card-kv-vip-*` | `institution-xray-kv-card-vip-v4.png` | as above; v4 (solid stepped mass) after the floating-tread versions read as a sparse diagram |
| `institution/xray-fig-card-kv-api-*` | `institution-xray-kv-card-api-v3.png` | as above; v3 (large tilted connector head) after v1 and v2 read as a thin strip |

Gold versions under `institution/gold/` from `scripts/gold_xray.py`, which grades `xray-fig-card-*` to the gold card surface #14120d. All passed the silhouette test.

## Round 13 (2026-11-01)

| File | Source | Treatment |
| --- | --- | --- |
| `api-broker/xray-bridge-*` | `asset-requests/xray/output/api-broker-xray-bridge-v2.png` (Codex attempt 1 of 3, adopted after review) | Top 5% and bottom 18% faded to black so the pylon head and piers recede instead of ending in a hard edge; then `export_xray.py --pad 1.5 --shift 1.0`. Replaces the round-8 bridge, whose short back-span left the pylon unbalanced and the deck ending in mid-air: the new one has an inclined pylon balancing the span by its weight, parallel harp stays, and the deck's left end on its own end pier |

Gold version under `api-broker/gold/` from `scripts/gold_xray.py`.

## Round 14 (2026-11-01)

| File | Source | Treatment |
| --- | --- | --- |
| `otc/xray-fig-level-{720,1080}.webp` | `asset-requests/xray/output/otc-xray-level.png` | `export_xray.py --figure`: black lifted to #0b0c0e, centred. A heavy weight resting on a spirit level supported only at its ends, bubble dead centre: a large trade, no market impact. Replaces the hook in Execution, which read as unclear |

Gold version under `otc/gold/` from `scripts/gold_xray.py`.

`affiliate/xray-rowing2vertical-{1000,1536,2400}` (and gold): content shifted right by 4% of the width (2026-11-01), so the port oar blades clear the headline at 1280–1440.

`institution/xray-lighthouse-*` (and gold), re-exported 2026-11-01 by a one-off script: a 1.28:1 canvas with the lighthouse at 88.3% of the height, 10% clear above it and 16% clear on the right, so the contained plate is height-bound on laptops (about 1.12x taller on screen). The portrait crop is x 0.40-0.95 of the same plate, leaving room above the lamp on phones. See DESIGN-GUIDE §6.4, X-ray spec.

2026-11-02:
- xray-fig-kit (market-maker): `market-maker-xray-kit.png`, `--figure` (4:5 kept); replaces the metronome in X-ray.
- xray-fig-studio-mic (affiliate): `affiliate-xray-studio-mic.png`, `--figure`; "How to become an affiliate." in X-ray (the pen was removed 2026-11-01).
- xray-rack (caas): `caas-xray-rack.png` (Codex attempt 4 of 4, copied by Claude; its drawn module reached 26% and its top margin 4%, both corrected by `--pad 1.4 --shift 1.0`: object now from 47%, 17% clear above, lit pixels 14.7%), `--portrait 0.35,1.0`.
- xray-carabiners (referral): `referral-xray-carabiners.png`, no pad (it bleeds off the top by design; lit pixels 13.0%), `--portrait 0.35,1.0`.
- `gold_xray.py affiliate market-maker caas referral`, then `grain_halo.py` on every hero plate it rewrote (affiliate rowing2vertical gold, market-maker turbofan gold, caas rack, referral carabiners, silver and gold).
- Retired: `institution/xray-fig-card-kv-*` and `institution/mono/` (the cards are photographs in every combination); `caas/xray-interim-*`.
- xray-fig-plug (caas): the API Broker plug figure, copied unchanged (silver and gold) into `caas/`; "End-to-end crypto rails." in X-ray.

- xray-bridge (api-broker), 2026-11-02: re-exported larger at the owner's request (the bridge read smaller than the other pages' objects). Same source; top 5% faded, and the bottom now fades from 80% to nothing at 92% so the piers dissolve under the deck and clear the "Built for" row at 1280; `export_xray.py --pad 1.18 --shift 1.0` (was 1.5, so about 1.3× larger), then `gold_xray.py api-broker` and `grain_halo.py` on the gold bridge plates. Previous files: scratchpad `backup-bridge-1102/`.
- xray-server (caas), 2026-11-02: `caas-xray-ai-server-v2.png` (Codex attempt marked NOT SAVED, copied with the owner's approval), `export_xray.py --pad 1.4 --shift 0.92 --portrait 0.30,1.0` to clear the headline and the right edge; `gold_xray` grade and `grain_halo.py` on both. Replaces xray-rack in `theme.ts`.
- xray-fig-card-* (institution), 2026-11-02: the v6 X-ray cards; see `institution/CREDITS.md`.
- xray-lighthouse-motion.{webm,mp4} (institution/gold), 2026-11-02: image-to-video by the owner on Luma (Ray) from `asset-requests/xray/motion/institution-gold-xray-lighthouse-start-frame.png` (the gold plate itself); source `asset-requests/xray/motion/X_Ray_Lighthouse_Locked-off_static_camera_Only_the_lighthouse_lamp_3ToYsonM.mp4`, 1628x1272, 8 s at 24 fps. Audio removed; everything outside 5-50% of the height blacked out (the page masks the overlay to 4-47%); VP9 CRF 36 (197 KB) and H.264 CRF 24 (386 KB). Aligned to the still at offset 0,0. Known: the beams tilt a little as they turn; the owner chose it as the best compromise so far.
- xray-turbofan-motion.{webm,mp4} (market-maker/gold) and xray-vaultclosed-motion.{webm,mp4} (otc/gold), 2026-11-02: image-to-video by the owner (Luma) from `asset-requests/xray/motion/{market-maker-gold-xray-turbofan,otc-gold-xray-vault}-start-frame.png` with the prompts in `asset-requests/xray/motion/video-prompts.md`; 1764x1176, 8 s, 24 fps. Audio removed, everything outside the moving area blacked out; VP9 CRF 36 / H.264 CRF 24 (about 0.5-0.75 MB each). Aligned to the stills within 1 px. Known: the engine spins up over its first two seconds; the vault turns its whole eight-spoke wheel (the prompt asked for the centre handle only), the second turn about twice as fast as the first. Masks per programme in `theme.ts` (`XRAY_MOTION`).
- Motion overlays re-encoded at 1440 px wide (2026-11-02, performance pass): a third fewer pixels to decode, files 20-40% smaller (turbofan 552/390 KB, vault 374/386 KB, lighthouse 162/247 KB, WebM/MP4); no visible difference at 2x. Previous files: scratchpad `perf/old/`.

2026-11-02 (run m):
- `affiliate/xray-rowing2vertical-*` (silver and gold, all sizes): the one accented rigger link copied onto the same link of all eight oars (mirrored for the port side, each placed by template match). Originals kept in `asset-requests/xray/derived/rowing2vertical-single-accent/`.
- `caas/xray-fig-usbc-{720,1080}` (silver and gold): the API Broker USB-C plate cropped 4:3 (x from 760/2400), replacing the plug figure on "End-to-end crypto rails." (owner: no traditional plug).
- `caas/xray-fig-gpu-{720,1080}` (silver and gold): the API Broker GPU plate, recentred on a padded canvas and cropped 4:3 with the card at 80%; replaces the USB-C figure, which did not read at figure size.
- Gold accent recoloured platinum → orange (owner): all `*/gold/*.webp` plates (214; the pen figure has no accent) and the three gold motion overlays, by `scripts/gold_accent_orange.py` / `gold_accent_orange_video.py` (luminance-preserving, soft mask; overlays re-encoded VP9 CRF 37 / H.264 CRF 25). Backups in `asset-requests/xray/derived/gold-platinum-accent-backup/`.
- Silver motion overlays `institution/xray-lighthouse-motion`, `market-maker/xray-turbofan-motion`, `otc/xray-vaultclosed-motion` (.webm/.mp4): the gold clips recoloured to the silver plates by `scripts/gold_to_silver_video.py` (a gold→silver colour table learned from each clip's start frame against its silver plate), so the silver pages keep the owner's chosen takes. Same masks; `motionFor` now serves both metals.
- 2026-11-02 (owner-approved rescue of strict-check rejects; see the LOG rows): `caas/xray-rackfront-*` (front-view rack, brightened, placed at 73% / 84% height; lights blink in code), `referral/xray-satellite-*` (three-quarter satellite, placed at 72%), `otc/xray-fig-flowgauge-*` (flow meter with gauge, replaces the level on "Liquidity, settlement and price."), plus `affiliate/xray-rowing6-*` from the owner's `affiliate-xray-rowing-six-pairs-downward-no-ripples.png`. Silver by `export_xray.py`, gold by `gold_xray.grade` (orange accent). No grain.
- 2026-11-02, motion and grain:
  - Overlays prepared by `scripts/prepare_motion.py` (alignment, audio removed, black outside the moving box, 1440 wide): `referral/gold/xray-chess-motion` (Luma, light passing from the queen to the pawns), `affiliate/gold/xray-rowing2vertical-motion` (Luma clip made from the accent-free plate; the eight orange rigger accents laid back into every frame), `api-broker/gold/xray-bridge-motion` (Luma light pulses; the mast-top accent is the still's, as Luma distorted it). Silver editions by `gold_to_silver_video.py`.
  - Grain (owner: every KV gets the bridge's grain): `grain_halo.py` on the silver bridge, turbofan, lighthouse, vault, rack, rowing and chess plates and on the gold lighthouse, vault, rack and chess plates (the gold bridge, turbofan and rowing already had it); `scripts/add_grain_video.py` adds the same grain to the matching overlays. Clean plates kept in `asset-requests/xray/derived/pre-grain-backup/`.
  - `api-broker/xray-fig-transceiver-{720,1080}` (silver, gold): the transceiver plate cropped 4:3 from x 1080/2400, replacing the plug on "Market access for your users".
  - `affiliate/xray-rowingclean-*`: the four-pair shell with every accent removed (silver recoloured from its own luminance map, gold regraded); kept as an alternative.
- 2026-11-02 (later): accent edits by `scripts/recolour_accent.py` (backups in `asset-requests/xray/derived/broker-accent-backup/` and `rack-orange-backup/`):
  - `api-broker/xray-bridge-*` (silver, gold): accent removed into the body; the bridge overlays rebuilt from the same Luma clip with the new plate (`prepare_motion.py --still`), silver by `gold_to_silver_video.py` plus `add_grain_video.py`.
  - `api-broker/xray-fig-{transceiver,headset,hourglass}-*` (silver, gold): accent made blue-white ("Built for the platforms traders already use.").
  - `caas/xray-rackfront-*` (silver, gold): the 48 lights made green; in code they now breathe slowly in a checkerboard (`XRAY_LIGHTS`, pattern 'alternate'). Interim until `caas-xray-rack-v2` is generated.
- 2026-11-02 (owner): the three "Built for the platforms traders already use." figures back to their orange accents (from `asset-requests/xray/derived/broker-accent-backup/`), then extended: every port of the transceiver bank carries the accent (the accented module copied to each port, placed by template match), the headset's ear cushion is orange as well as the microphone, and all of the hourglass's sand is orange (the grains only; the empty glass and the centre rod keep the body colour). The orange comes from each plate's own accent, so silver stays copper-orange and gold stays orange.
- `caas/xray-rackv3-*` (silver, gold), 2026-11-02: the owner's modern edit `caas-xray-rack-v3-modern.png` (half-height rack, four servers of twelve bays), placed at 72% / 46% wide; grain halo; 48 neutral lights measured into `XRAY_LIGHTS`, which breathe green in a checkerboard. Replaces `rackfront`.
- 2026-11-02 (owner, later): `otc/xray-fig-binoculars-*` mirrored (objective lenses to the right; originals in `derived/binoculars-unmirrored/`). `affiliate/xray-fig-megaphone-*` object scaled to 78%, centred (originals in `derived/megaphone-full/`). `api-broker/xray-fig-transceiver-*`: the bank completed (the left mounting plate mirrored onto the right end after the seventh port, scaled to 86% and centred), and the three Broker figures' orange desaturated by 45% towards grey. `referral/xray-fig-studio-mic-*`: copied from Affiliate for "Take your friends further.". CaaS rack lights white, each on its own slow cycle (5-8 s).
- 2026-11-02 (owner): `referral/xray-chess-*` plates and `xray-chess-motion` overlays scaled to 90%, anchored at the right-edge centre so the pawns still run off the edge (mask scaled to match; originals in `derived/chess-full-size/`). `referral/xray-fig-studio-mic-*` and the photo `referral/figures/team.webp` scaled to 80%, centred (originals in `derived/referral-figure-full/`).
- `api-broker/xray-fig-{access,support,commission}-{720,1080}` (silver, gold), 2026-11-02: the v3 figures (`api-broker-xray-fig-access-v3-a1`, `-support-v3-a2`, `-commission-turbine-a1`), placed at 80% on a 4:3 plate, `export_xray.py --figure`, gold by `gold_xray.grade`, accent softened 45% towards grey. Replace the transceiver bank, the headset and the hourglass on "Built for the platforms traders already use."
- 2026-11-02 (review pass, owner-approved; backups under `asset-requests/xray/derived/`):
  - Key visual scale by `scripts/scale_kv.py` (plates and overlays together, masks moved to match): `caas/xray-rackv3-*` to 92.5% about (0.720, 0.500) (`rackv3-full-size/`); `otc/xray-vaultclosed-*` to 105% about (0.726, 0.481) and `affiliate/xray-rowing2vertical-*` to 103% about (0.472, 0.553) (`kv-before-scale/`).
  - Institutions card images (`institution/xray-fig-card-{otc,market-maker,vip,caas,api}-*`, silver and gold) brightened 10% over the background, `bg + (px - bg) × 1.10` (`cards-before-brighten/`).
  - `referral/xray-fig-studio-mic-*`: accent desaturated 45% towards grey, like the Broker figures.
  - All six silver motion overlays (lighthouse, turbofan, vault, bridge, rowing, chess) re-converted with the smooth mode of `gold_to_silver_video.py`: two 1-D tables keyed by luminance, blended by how orange each pixel is, replacing the 32-step 3-D colour table that broke soft glows and grain into visible patches. Grain re-added by `add_grain_video.py`. Previous files in `derived/silver-motion-table/`.
- 2026-11-03 (owner):
  - Reverted to the pre-review state (commit 7199967): the OTC vault and Affiliate rowing key visuals at their former size, with their former overlays and masks. The CaaS rack stays at 92.5% (owner's own request).
  - Grain removed from the dark ground of every hero plate by `scripts/denoise_kv.py` (it did not survive the overlays' video compression, so it vanished and returned as the motion passed). Backups in `derived/kv-before-denoise/` and git.
  - Every motion overlay rebuilt by `scripts/lock_overlay.py`: each frame is the still plus what changes in the clip (`light` for the lighthouse, bridge and chess, `move` for the turbofan, vault and oars), so the overlay's ground equals the still's: no seam at the mask edge, no compression patches. The silver overlays are converted from the gold ones by `gold_to_silver_video.py` (smooth mode) before locking. Previous files in `derived/motion-before-lock/`.
  - `referral/xray-chess-*` (landscape, both metals) and its overlays moved 6% to the left, the right 12% of the width eased to the ground (`scripts/shift_kv.py`); mask centre moved to match.
  - New figures from the v2/v7/v4 prompts, placed at 80% on a 4:3 (cards 3:2) plate, `export_xray.py --figure`, gold by `gold_xray.grade`, accent softened 45%: `market-maker/xray-fig-perks` (caliper, `market-maker-xray-fig-perks-v2-a3`), `caas/xray-fig-rails` (linear guide, `caas-xray-fig-rails-v2-a3`), `referral/xray-fig-radios` (two radios, `referral-xray-fig-radios-v2-a2`), `institution/xray-fig-card-api` (`institution-xray-card-api-v7-a1`) and `xray-fig-card-caas` (`institution-xray-card-caas-v7-a2`), both brightened 10% like the other cards, and `api-broker/xray-fig-access` (`api-broker-xray-fig-access-v4-a1`). Previous card and access files in `derived/figs-before-v7/`.
  - `api-broker/gold/xray-fig-{access,support,commission}-*` and `referral/gold/xray-fig-radios-*`: paled towards yellow-white gold, the accent redrawn in the megaphone figure's orange (`scripts/pale_gold_figure.py`; previous Broker files in `derived/broker-gold-before-pale/`).
- 2026-11-03 (later, owner):
  - Motion overlays rebuilt again from the pre-review clips (commit 7199967) by the new `scripts/lock_overlay.py`: the clip itself, its dark ground smoothed and shifted to the still's ground level. The previous build added the clip's changes to the still, which left the still's own beams and resting oars behind as ghosts. Silver overlays converted from the gold ones (`gold_to_silver_video.py`, smooth) before matching.
  - Grain as its own layer (`scripts/grain_layer.py`: `grain.webp`, `grain-warm.webp`, one `xray-<variant>-grain-mask.webp` per key visual), not in the files.
  - `referral/xray-chess-*` and overlays: moved 6% left, the row's cut end faded over 82-94% of the width (`shift_kv.py`); the hero bleeds past the viewport so 1440 px cuts where the fade begins.
  - Institutions card images moved from the raised-card ground to the page ground (cards are open entries now); 360 px editions of every X-ray figure and card for 1x screens (fine lines aliased when a 720 px file was drawn at about 260 px).
