# otc — image sources

The images on this page are AI-generated, made 2026-10-30 by Codex (built-in image generation; the model is not disclosed) from the approved art direction (`ART-DIRECTION.md`) and the prompts in `asset-requests/v2/prompts/`. The raw files and the generation log are in `asset-requests/v2/output/` (`LOG.md`). They are material or architectural metaphors only: they depict no product, interface, data, person, brand or logo, and they make no claim. Confirm that the generator's output terms match your organisation's agreement before launch.

| File | Subject | Raw source | Processing |
| --- | --- | --- | --- |
| `hero-*.webp` | Two monumental slabs and a slit of light, in deep perspective (the private room) | `asset-requests/v2/output/otc-hero-v2.png` | `grade_images.py --crush 10`, widths 1000 and 1536; the slit sits at 66% width (`hero--tall`) |
| `hero-portrait-*.webp` | Same | Same | Crop 0.40–0.96 width, widths 800 and 980 |
| `plate/plate-1536.webp` | The same slabs face-on and symmetrical: wall, light, wall | `asset-requests/v2/output/otc-plate-v2.png` | Graded with `--crush 14`, cropped to the central 50% width at 2.25:1 so the side columns hold the lit slab edges, resized to 1536 px (soft gradients only), sliced in CSS into three columns |

## Section figures (reused from v1)

| File | Subject | Raw source | Processing |
| --- | --- | --- | --- |
| `figures/stillness-{720,1080}.webp` (v3, 2026-11-02: `asset-requests/output/otc-figure-stillness-v3.png`, lit water, same treatment; the row below describes v2) | A heavy titanium block on still black water, a small ripple far behind it (Liquidity, settlement and price): large size, no market impact | `asset-requests/output/otc-figure-stillness-v2.png` (Codex, 4 attempts) | `grade_images.py --crush 14 --widths 720,1080`, full 4:3 frame; gold with `--palette gold`. Replaces the block on glass (v1 of this figure read the water as a floor) |

These v1 images were re-cropped into the v2 language (cropped, low-key, edges only) and used as single section figures, not as a vignette row.

The raw output is 1536 × 1024, so the largest export is 1536 px (not upscaled). Other v1 images (`asset-requests/output/`) remain unused.

## Solution vignettes (AI-generated)

`benefits/{portal,desk,api}-*.webp` and `gold/benefits/…`: generated with ChatGPT (asset-requests/output/otc-vignette-*.png), 4:3 crop (0.391, 0.161, 0.990, 0.835), `--crush 12`, graphite grade; gold edition `--palette gold`. They replace the sliced plate in "Solutions for every playbook" (2026-10-31).

Round 2 (2026-10-31): `benefits/{loupe,bell,key}-*.webp` are live; `lever`, `seal` and `coupling` are graded backups. Same crop and grades. Sources: asset-requests/output/otc-vignette-*.png (prompts in asset-requests/prompts, README "OTC solutions, round 2").
