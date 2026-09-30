# Settings and layouts

## Panel menu

Open the panel menu (**≡** at the top-right of the panel) for D-Pad's settings. Your choices are remembered.

**Keyframes**

- **Shift All** (default): when a layer has Position keyframes, every keyframe moves by the same amount and your easing is kept
- **Current Frame Only**: only the current frame changes (a keyframe is added there if needed)

**Anchor: Keep Layer in Place** (on by default): turn off to move the anchor point without compensating Position, so the layer shifts.

**Position: Comp Edges / Title Safe / Action Safe**: which frame Position mode uses. Title Safe is 90% of the comp, Action Safe 80%.

**Align Layers To: Selection / Top Layer / Bottom Layer**: what Position mode lines multiple layers up with. Selection uses the bounds of all selected layers; Top and Bottom use one layer as the reference and leave it where it is.

**Layout: Auto / D-Pad / Horizontal / Vertical**: see below.

**Bake & Disconnect Parent**: for layers parented to something (for example an animated null). Records the layer's full on-screen movement as its own keyframes, one per frame, then unparents it so it moves exactly as before without the parent. Works on 2D layers.

**User Guide**: opens this page.

## Layouts

D-Pad fits into whatever space you give it.

- **D-Pad**: the classic 3 × 3 pad
- **Vertical**: everything in one column, for narrow panels
- **Horizontal**: everything in one row, for short panels

With **Auto** (the default), D-Pad stays on the pad whenever it can. It switches to **Vertical** when the panel is narrower than 150 px and taller than 200 px, and to **Horizontal** when it is shorter than 90 px.

If a row or column is longer than the panel, scroll it with your mouse wheel.

To always use one layout, pick it in the panel menu.
