# FireSaints Controller Skin — Design Specification

## Target

- Platform: GamePad Viewer 2
- Base skin: Xbox One
- Use: OBS Browser Source
- Input mapping: retain the existing Xbox layout and GPV input detection

## Visual identity

| Component | Direction |
|---|---|
| Main shell | Predominantly matte black |
| Tribal artwork | Deep metallic purple, flowing across the grips and upper shell |
| Secondary trim | Brushed silver |
| A/B/X/Y | Silver button faces with restrained purple legends or rings |
| D-pad | Dark metal with silver edge highlights |
| Thumbsticks | Black caps, silver edge detail, purple accent rings |
| Bumpers/triggers | Black with silver trim |
| Xbox logo area | Neutral silver/white; avoid overpowering the FireSaints branding |
| Active state | Purple glow on the individual control while pressed |
| Ambient lighting | Soft purple halo around the shell, not a permanent overpowering neon outline |

## Interaction goals

1. Each digital control lights independently when GPV reports it pressed.
2. Glow transitions should be smooth and readable at stream scale.
3. Analog triggers should retain their input visualization rather than becoming static decorations.
4. Thumbstick movement and click states must remain visible.
5. Disconnected/idle presentation should remain clean and unobtrusive.

## Technical constraints

- Do not replace the GPV controller markup or interfere with its Gamepad API input handling.
- Prefer CSS overrides on the existing Xbox One skin.
- Confirm actual GPV 2 selectors and DOM structure before implementing selectors.
- Keep artwork as transparent PNG/SVG layers where practical.
- Test in the GPV preview before changing the OBS Browser Source.
- Do not assume selectors from GamePad Viewer Classic are compatible with GPV 2.

## Palette (initial)

- Shell: #09090D
- Deep tribal purple: #32105C
- Primary purple: #8B35D6
- Highlight purple: #C58BFF
- Silver: #BFC3CC
- Dark silver: #666B76
- Glow: rgba(155, 70, 255, 0.75)

These are starting values and can be adjusted during visual review.
