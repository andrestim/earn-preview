# Institutions imagery

All sources generated with OpenAI image_gen via Codex (2026-11-01); raw files and prompts in
`asset-requests/institution/` (`output/LOG.md` records each generation and its silhouette test).

| File | Use | Source | Treatment |
| --- | --- | --- | --- |
| `hero-*.webp`, `hero-portrait-*.webp` | Hero: a fluted titanium column, cropped top and bottom (`standard` layout) | `output/institution-hero.png` | `grade_images.py --crush 9`, widths 1000 and 1536; portrait crop at 0.42–0.96 of the width, widths 800 and 980 |
| `cards/otc-*.webp` | Ways in: OTC (the OTC key visual: light slit between stone walls) | `output/institution-kv-card-otc.png` | `grade_images.py --crush 12 --black #101114` (the card surface, `--bg-raised`), full 4:3 frame, widths 720 and 1080 |
| `cards/market-maker-*.webp` | Ways in: Market Maker Programme (the MMP key visual: fan blades) | `output/institution-kv-card-market-maker.png` | as above |
| `cards/vip-*.webp` | Ways in: VIP Portal (basalt steps rising toward daylight) | `output/institution-kv-card-vip-v4.png` | as above. v4 after a premium pass: v1 to v3 read as generic rendered stairs |
| `cards/caas-*.webp` | Ways in: Crypto as a Service (one long module drawn out of a machined wall) | `output/institution-kv-card-caas-v2.png` | as above. v2 after a premium pass: v1 read as wall tiles |
| `cards/api-*.webp` | Ways in: Exchange API (machined titanium fibre connector) | `output/institution-kv-card-api-v3.png` | as above. v3 after a premium pass: v1 and v2 read as a consumer patch cable |
| `gold/…` | The same images, gold | Same | As above, plus `--palette gold`; cards with `--black #14120d` (the gold `--bg-raised`) |

X-ray editions (`?kv=xray`) are under `public/assets/xray/institution/`; see that folder's CREDITS.

## Cards v5 (2026-11-02): physical objects, every combination

The five `cards/*` and `gold/cards/*` files are replaced by v5: one physical metal object each, photographed in the left of a 3:2 frame with the right third dark and a light corner grain (`asset-requests/institution/prompts/institution-card-v5-*.txt`). They are shown in photo and X-ray, silver and gold; the X-ray card plates (`xray/institution/xray-fig-card-kv-*`, `mono/`) are retired. Previous files: scratchpad backup only.

| File | Object | Source | Treatment |
| --- | --- | --- | --- |
| `cards/otc-*` | A bank vault door | `output/institution-card-v5-otc-vault.png` | `grade_images.py --crush 26 --black #101114 --widths 720,1080`; `gold/cards/` the same graphite grade with `--black #14120d` (silver object on the gold card, no copper) |
| `cards/market-maker-*` | A jet engine, intake facing right | `output/institution-card-v5-market-maker-engine.png` | as above |
| `cards/vip-*` | A modern leather lounge chair with its footrest (2026-11-02; replaced the raw crystal) | `output/institution-card-v5-vip-chair-v3.png` (the owner's third revision) | as above |
| `cards/caas-*` | A rack server (NAS) lying flat | `output/institution-card-v5-caas-nas.png` | as above |
| `cards/api-*` | A processor chip | `output/institution-card-v5-api-chip.png` | as above |


## v6 cards (2026-11-02)

Every object straight-on or in a true 90-degree side profile; generated as gold photographs (`asset-requests/institution/prompts/institution-card-v6-*.txt`), with an X-ray edition of the same objects and views. Previous v5 files: scratchpad `backup-cards-v5/`.

| File | Object, view | Source | Treatment |
| --- | --- | --- | --- |
| `cards/{otc,market-maker,vip,api}-*`, `gold/cards/…` | Vault door face-on; jet engine side profile; lounge chair and ottoman side profile; chip plan view | `output/institution-card-v6-{otc-vault,market-maker-engine,vip-chair,api-chip}.png` | `grade_images.py --crush 20 --widths 720,1080`: silver `--black #101114` (graphite), gold `--palette gold --black #14120d`. VIP at `--crush 32`, then its lit ground flattened to the card colour (dark pixels only) |
| `cards/caas-*`, `gold/cards/caas-*` | Still v5 (rack server, three-quarter view) | — | Interim: the v6 photo failed (top showing, a thin 1U strip); a 4U prompt is out (`institution-card-v6-caas-server-4u.txt`) |
| `xray/institution/xray-fig-card-{otc,market-maker,vip,caas,api}-*` and `gold/` | The same objects in X-ray | `output/institution-card-v6-xray-*.png` (vault and engine: Codex attempts marked NOT SAVED, copied by Claude with the owner's approval) | `export_xray.py --figure --bg #101114`; gold via `gold_xray.grade`, its ground re-levelled to the gold card colour #14120d. CaaS is the thin 1U interim until the 4U prompt returns |

VIP chair mirrored (owner, 2026-11-02): `asset-requests/institution/derived/institution-card-v6{,-xray}-vip-chair-mirrored.png`, the v6 sources flipped horizontally and shifted back so the object starts at the same left edge (about 4%), the opened strip filled with the ground colour and feathered; then the same exports as above. New prompts out: CaaS as a tall NAS drive tower (`institution-card-v6{,-xray}-caas-nas-tower.txt`, replacing the 4U server) and a sparser X-ray engine (`institution-card-v6b-xray-market-maker-engine.txt`, six parts at most).

X-ray cards updated (owner, 2026-11-02): `xray-fig-card-caas-*` from `output/institution-card-v6-xray-caas-nas-tower.png` (a six-drive NAS tower; Codex attempt marked NOT SAVED, copied with approval), scaled to 80% about its left edge (`derived/…-fit.png`) so it sits inside the plate like the others; `xray-fig-card-market-maker-*` from `output/institution-card-v6b-xray-market-maker-engine.png` (the sparse engine, six large parts). Same export and gold re-levelling as above.
