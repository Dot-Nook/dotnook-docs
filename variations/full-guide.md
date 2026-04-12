# Full guide

## Name

Use the Name section to set the name of the duplicated comp(s).

**New**: the duplicate comp's name will match the input text exactly.

**Variant**: build the name dynamically from the original comp's name using one of three options:

- **Replace Text**: find and replace text from the original comp's name
- **Add Before**: add text before the original comp's name
- **Add After**: add text after the original comp's name

## Location

Use the Location section to set the folder location of the duplicated comp(s). Standard URL path notation defines the folder hierarchy.

**New**: define the location from the root of the project panel hierarchy.

Example: `/folder-name/inner-folder/new-folder/`

**Variant**: define the location relative to the original comp's location.

Example: `../../new-folder/inner-folder/`

> **Note:** `..` is standard notation for ascending to the parent folder. Leading and trailing `/` are optional. The path doesn't need to already exist: any new folders are created automatically.

## Frame rate

Use the Frame Rate section to set the frame rate of the duplicated comp.

> **Note:** If you are changing both the frame rate and duration of a new comp, the frame rate is adjusted first. Set the new duration in terms of the new frame rate. For example, if you want to add 10 frames to a 6s 19f comp and also change it from 25fps to 30fps, the new comp will be 6s 29f (not 7s 4f).

## Duration

Use the Duration section to set the duration of the duplicated comp. Duration should be written in `hh:mm:ss:ff` format.

**New**: define the exact duration of the new comp.

**Variant**: define the duration as an addition or subtraction from the original. Use the + or - switch to add or subtract time. Useful for making a version with or without an end card.

## Dimensions

Use the Dimensions section to set the width and height of the duplicated comp.

**New**: define exact width and height values.

**Variant**: define width and height as additions or subtractions from the original using the + or - switch.

## Pre-comps

Use the Pre-comps section to control how precompositions inside your comp are handled.

Choose whether to duplicate and relink precomps. When duplicating precomps, you can define a new folder location for them using the same path notation as the Location section: either from the project root (New) or relative to the original precomp's location (Variant).

Frame rate, duration and dimension changes configured above can also be applied to the duplicated precomps.
