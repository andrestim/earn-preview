# market-maker — image sources

The images on this page are AI-generated, made 2026-10-30 by Codex (built-in image generation; the model is not disclosed) from the approved art direction (`ART-DIRECTION.md`) and the prompts in `asset-requests/v2/prompts/`. The raw files and the generation log are in `asset-requests/v2/output/` (`LOG.md`). They are material or architectural metaphors only: they depict no product, interface, data, person, brand or logo, and they make no claim. Confirm that the generator's output terms match your organisation's agreement before launch.

| File | Subject | Raw source | Processing |
| --- | --- | --- | --- |
| `hero-*.webp` | Two machined faces meeting, the gap as one lit line across the frame (the spread) | `asset-requests/v2/output/market-maker-hero-v2.png` | `grade_images.py --crush 9`, widths 1000 and 1536; the line sits at 66% height (`hero--horizon`) |
| `hero-portrait-*.webp` | Same | Same | Crop 0.25–0.89 width, widths 800 and 980 |

## Section figures (reused from v1)

| File | Subject | Raw source | Processing |
| --- | --- | --- | --- |
| `figures/capital.webp` | Flush-fitted inserts, cropped (Schedule A) | `asset-requests/output/market-maker-vignette-capital.png` (v1) | crop (814, 276, 1294, 636) px, then crush 13 and gamma 1.6 to match the v2 key, graphite grade; native size, not upscaled |

These v1 images were re-cropped into the v2 language (cropped, low-key, edges only) and used as single section figures, not as a vignette row.

The raw output is 1536 × 1024, so the largest export is 1536 px (not upscaled). Other v1 images (`asset-requests/output/`) remain unused.

## Hero, 2026-10-30 (replaces the horizon hero)

- `hero-*.webp` and `gold/hero-*.webp`: generated (asset-requests/mm-engine, `market-maker-hero-engine-a`), graded with `grade_images.py` (crush 8; gold edition `--palette gold`).
  - The landscape set is padded 1.25x with feathered edges so the blades clear the headline.
  - The portrait crop is x 0.30–0.94 of the unpadded source.
- The previous horizon hero is backed up outside the repo and can be restored from `asset-requests/v2/output/market-maker-hero-v2.png`.
- Revised the same day for contrast: `python scripts/grade_engine_hero.py asset-requests/mm-engine/output/market-maker-hero-engine-a.png 1.25 0.9 14 195 1.2` (levels 14-195, gamma 1.2, both palettes). The page also turns off the shared hero glow (`--hero-light: transparent`), which fogged the blades.
- Replaced the same day by `market-maker-hero-engine-c` (the same engine, reframed to show the spinner and blade roots): `python scripts/grade_engine_hero.py asset-requests/mm-engine/output/market-maker-hero-engine-c.png 1.12 1.0 14 195 1.2 0.40 1.0` (flush right, mobile crop centred on the hub).
- Softened the same day for detail and elegance: levels 4-250, gamma 0.8 (`... engine-c.png 1.12 1.0 4 250 0.8 0.40 1.0`).
- Polished and warmed the same day: edge-preserving smoothing (2.5px), a 1.6x Lanczos upscale with a light unsharp mask, a 2400px retina set, and the new calm-gold palette.
- Replaced the same day by `market-maker-hero-engine-d` (sharper blades, smooth polish): `python scripts/grade_engine_hero.py asset-requests/mm-engine/output/market-maker-hero-engine-d.png 1.3 1.0 8 250 1.1 0.40 1.0` (wider left feather, so the brighter blades stay clear of the headline).
- Replaced the same day by `market-maker-hero-engine-f` (18 wide-chord blades, chosen over the frontal engine-e): `python scripts/grade_engine_hero.py asset-requests/mm-engine/output/market-maker-hero-engine-f.png 1.3 1.0 8 250 1.1 0.40 1.0`.

## Section figure (2026-11-01)

| File | Use | Source | Treatment |
| --- | --- | --- | --- |
| `figures/metronome-720.webp` | Metronome mid-beat (Benefits and perks, beside the heading) | `asset-requests/output/market-maker-vignette-metronome.png` | `grade_images.py --crush 12 --crop 0.312,0.161,0.971,0.903 --widths 720`, graphite; `gold/figures/` with `--palette gold` |

| `figures/kit-720.webp` | A fitted instrument case, each perk in its own cut-out (Benefits and perks; replaces the metronome, 2026-11-02) | `asset-requests/output/market-maker-figure-kit.png` | `grade_images.py --crush 12 --widths 720`, full 4:5 frame; `gold/figures/` with `--palette gold` |
