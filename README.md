# FireSaints Controller Skin

A custom FireSaints-branded Xbox One controller skin for GamePad Viewer 2 (GPV 2), intended for OBS Browser Source.

## Design direction

- Matte black controller shell
- Deep-purple tribal graphics
- Brushed-silver accents
- Silver A/B/X/Y button faces
- Purple illuminated rings and reactive pressed states
- Black thumbsticks with purple detailing
- Subtle ambient purple glow
- Preserve the Xbox controller layout and GPV input behaviour

## Project status

**In development.** The visual specification is established. The next implementation step is to verify the exact GPV 2 Xbox skin selectors and component structure before adding styling rules. This avoids applying CSS written for the older GamePad Viewer interface.

## Planned files

- style.css — GPV 2 skin overrides
- assets/ — original controller artwork and transparent graphic layers
- DESIGN.md — visual and implementation notes

## Use

The stylesheet will be hosted with GitHub Pages and its public CSS URL will be entered in GPV 2's **Edit CSS URL** field. The existing GPV overlay URL remains the OBS Browser Source URL.
