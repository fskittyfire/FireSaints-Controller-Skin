# FireSaints Controller Skin

A custom FireSaints-branded Xbox One controller skin for GamePad Viewer 2 (GPV 2), intended for OBS Browser Source.

## Design direction

- Matte-black Xbox shell
- Deep-purple tribal graphics
- Brushed-silver accents
- Silver A/B/X/Y faces with reactive purple glow
- Dark thumbsticks with purple edge lighting
- Independently illuminated D-pad, bumpers, triggers, and menu buttons
- Preserve the existing Xbox layout and GPV input behaviour

## Project files

- `style.css` — GPV 2 skin overrides
- `assets/tribal-overlay.svg` — transparent FireSaints tribal and silver overlay
- `DESIGN.md` — visual and implementation notes

## Enable GitHub Pages

1. Open this repository's **Settings**.
2. Select **Pages** in the sidebar.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/(root)**.
5. Click **Save** and wait for GitHub Pages to finish deploying.

After deployment, the stylesheet URL will be:

`https://fskittyfire.github.io/FireSaints-Controller-Skin/style.css`

Enter that URL in GPV 2's **Edit CSS URL** field. Keep your existing GPV overlay URL for OBS.

## Important testing note

The stylesheet is an initial implementation and must be preview-tested in GPV 2 before it is treated as finished. If the skin does not load or controls render incorrectly, remove the custom CSS URL to return to the original Xbox skin while we troubleshoot.

## Project status

**First implementation committed; awaiting GitHub Pages activation and GPV 2 preview testing.**
