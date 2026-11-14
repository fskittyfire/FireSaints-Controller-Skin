# FireSaints Controller Skin — Design Specification

## Target
- Platform: GamePad Viewer 2 (app.gpv.gg)
- Base skin: Xbox One
- Use: OBS Browser Source
- Input mapping: preserve GPV's existing Xbox input detection and geometry

## Visual identity
- Main shell: predominantly matte black, retaining the native Xbox silhouette.
- Tribal artwork: deep metallic purple, mirrored across both grips.
- Secondary trim: brushed silver pinstriping.
- A/B/X/Y: silver-toned faces, purple glow while pressed.
- D-pad: silver-toned, purple glow while pressed.
- Thumbsticks: dark metallic finish with subtle purple edge lighting.
- Bumpers and triggers: silver-tinted details, independent purple active glow.
- Branding: small FS insignia in the lower bridge area.
- Ambient lighting: restrained purple shadow, stronger reactive glow on active controls.

## Interaction goals
1. Each digital control lights independently when GPV marks it .pressed.
2. Glow transitions remain smooth and readable at stream scale.
3. Analog trigger indicators retain their GPV input behaviour.
4. Stick movement and stick-click states remain visible.
5. The disconnected state remains identifiable.

## Technical approach
- Override the existing .controller.xbox skin rather than replacing GPV markup.
- Use GPV's existing control classes: .button, .face, .stick, .bumper, .trigger, .back, and .start.
- Add transparent decorative artwork using a controller ::before overlay.
- Keep pointer-events disabled on decorative artwork so it cannot interfere with controls.
- Verify actual browser rendering and pressed-state behaviour before using the stylesheet in OBS.
- Do not assume GamePad Viewer Classic and GPV 2 are identical; the current CSS is based on a community stylesheet explicitly documented for app.gpv.gg.

## Initial palette
- Shell: #09090D
- Deep tribal purple: #32105C
- Primary purple: #8B35D6
- Highlight purple: #C58BFF
- Silver: #BFC3CC
- Dark silver: #666B76
- Glow: rgba(155, 70, 255, .78)
