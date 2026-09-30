# Full guide

D-Pad measures layers by what you actually see: the bounds of the text, shape or footage, including rotation, scale, parenting and 3D. Keyframed Position is shifted keyframe by keyframe, keeping your easing and curves.

## Anchor Point

Move the anchor point to one of nine points on each selected layer.

**Click**: moves the anchor point. The layer stays exactly where it is on screen: D-Pad adjusts Position to compensate, on every Position keyframe.

**Opt/Alt + click**: moves the anchor point and **freezes** it there with a lightweight expression. The expression is evaluated once and then held, so it costs nothing per frame.

### Footer: Reset

**Click**: moves the anchor point back to the centre of the layer.

**Opt/Alt + click**: removes a D-Pad freeze but keeps the anchor point where it is.

> **Tip:** to move the anchor point *and* let the layer shift, turn off **Anchor: Keep Layer in Place** in the [panel menu](settings.md).

## Position

Move layers to a point of the comp, or line them up with each other.

**One layer selected**: moves the layer so its anchor point sits on that point of the comp. If the layer has a parent, it moves to that point of the **parent's** bounds instead.

**Two or more layers selected**: aligns the layers to each other by their visible edges. For example, the top-left button lines up every layer's top-left corner with the top-left of the whole selection. Choose what they line up to in the [panel menu](settings.md): the selection, the top layer or the bottom layer.

**Opt/Alt + click**: moves each layer's anchor point to that point of the comp, even when parented.

> **Tip:** switch the comp reference to **Title Safe** or **Action Safe** in the [panel menu](settings.md) to align to the safe margins instead of the comp edges.

### Footer: Center / Distribute

The two footer buttons work horizontally and vertically.

- **One or two layers**: centres each layer in the comp (or in its parent). **Opt/Alt + click** always centres in the comp.
- **Three or more layers**: distributes them so the gaps between them are equal. **Opt/Alt + click** spaces their centres evenly instead.

## Attach Null

Create null objects to control your layers.

**Click**: creates one null per selected layer, sized to the layer and placed at the point you pressed. The layer is parented to the null and doesn't move. If the layer already had a parent, the null slots in between, so the parent still works.

**Opt/Alt + click**: creates one null around the whole selection, at the point you pressed, and parents every selected layer to it.

**Nothing selected**: drops a null at that point of the comp.

3D layers get 3D nulls.

### Footer: Unparent

**Click**: unparents the selected layers without moving them. If that leaves a null with no children (and no animation of its own), the null is removed.

**Opt/Alt + click**: dissolves the null completely, releasing all of its children, not just the selected ones.

> **Note:** D-Pad only ever deletes nulls, never other layers.

## Before D-Pad changes anything

If some of the selected layers need a decision, D-Pad asks **before** it does anything:

- **Locked layers**
- **Layers with an expression** on a property D-Pad would change
- **Layers that already have a parent** (when grouping under one null)

Choose:

- **Skip those layers**: do everything else, leave these alone
- **Apply anyway**: unlock them just for the change (they're locked again afterwards) and remove the conflicting expression, keeping its current value so nothing jumps
- **Cancel**: do nothing

Tick **Remember my choice** to skip the question until After Effects restarts.

Cameras, lights, empty layers and layers with an animated Anchor Point can't be changed and are always skipped.

## Good to know

- Every press is a single undo step.
- Layers with an animated Anchor Point are skipped.
- With animated rotation or scale, D-Pad's compensation is exact at every Position keyframe. Between keyframes the pivot has genuinely changed, so the motion can differ slightly.
- 3D layers are aligned on X and Y. Z is left alone.
- Unparenting from a parent that is both rotated and unevenly scaled can't keep the exact look. After Effects has the same limit.
