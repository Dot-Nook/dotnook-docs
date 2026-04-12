# Pseudo-effect

After Square Peg creates a shape layer, a pseudo-effect appears on that layer in After Effects' effect controls. The pseudo-effect has three sections: Sizing, Corners and Colors.

## Sizing

- **Width**: adjusts the width of the shape
- **Height**: adjusts the height of the shape
- **Anchor Point**: sets the anchor point for the shape. This operates independently from the layer's transform anchor point, allowing the shape to grow and shrink from different points without squashing or stretching the corner curvature.

## Corners

- **Link Corners**: when checked, the radius and curvature sliders adjust all four corners together. Uncheck to access individual corner controls.
- **All Radii**: sets the radius for all corners at once (visible when Link Corners is checked)
- **All Curvature**: adjusts the curvature for all corners at once. Curvature bends corners from square, to squircle, to rounded, to bevelled, to inverted and even notched.
- **Individual corner sliders**: eight separate controls (radius and curvature) for each of the four corners, visible when Link Corners is unchecked.
- **Unlock Corners**: normally, corner radius is restricted to half the shortest side's length. Checking this removes that restriction.

> **Note:** Unlocking corners can cause unexpected visual results due to limitations in After Effects expressions.

## Colors

- **Use FX Colors**: when checked, the shape uses the colour pickers in the pseudo-effect rather than the standard shape layer properties. Useful for saving specific colours with a preset.
- **Enable Fill**: toggles fill visibility (opacity-based)
- **Enable Stroke**: toggles stroke visibility (opacity-based)
- **Fill Color**: sets the fill colour when Use FX Colors is active
- **Stroke Color**: sets the stroke colour when Use FX Colors is active
- **Stroke Width**: controls stroke thickness
