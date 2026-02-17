# <i class="bi bi-noise-reduction"></i>  Manga Tone Shader
![Section](assets/img/EN/MTS section.png)

Finally, fine-tune the look of tone materials. This dedicated toon shader is designed to represent manga-like strokes and shadows.

## <i class="bi bi-journal-richtext"></i>  Steps
1. Select objects that have the "Manga Tone Shader" assigned.
2. Open the Manga Tone Shader section under the 3D Manga Studios tab.
3. Tweak parameters to match your artistic intent.

!!! warning "Note"
    Manga Tone Shader works only with the EEVEE render engine. It will not display correctly with Cycles.

## <i class="bi bi-columns"></i>  Key properties
### Light Offsets
| Enabled | Disabled |
| --- | --- |
|![Before](assets/img/EN/MTS key offsets.png)|![After](assets/img/EN/MTS key offsets after.png)|

Adjust highlight spread for Key/Fill/Back lights.

### Boolean toggles
| On | Off |
| --- | --- |
|![On](assets/img/EN/MTS boolean.png)|![Off](assets/img/EN/MTS boolean off.png)|

Toggle features like Shadow, AO, and Gloss. Disabling hides their child parameters and disables the effect.

### RGBA / Material drop slots
| Before | After |
| --- | --- |
|![Before](assets/img/EN/MTS DD.png)|![After](assets/img/EN/MTS DD after.png)|

Use the color inputs and the drop slots to assign tone materials from Screen tones. Drag & drop materials to place patterns in specific regions.

!!! warning "Caution"
    Assigning too many materials across multiple drop slots may cause issues:

    | Freeze | Broken material |
    | --- | --- |
    |![Freeze](assets/img/EN/freeze.png)|![Broken](assets/img/EN/error.png)|

    - Blender may freeze
    - Materials may fail to display (pink/purple)

    For stability, use up to around four drop slots as a guideline.
    
### Properties of dropped materials
| Before | After |
| --- | --- |
|![Before](assets/img/EN/MTS DD property.png)|![After](assets/img/EN/MTS DD property after.png)|

Adjust scale, rotation, etc. of dropped tone textures.

[Learn more about Screen tone materials](OptionMaterial.md)

## <i class="bi bi-flag-fill"></i>  Done!
That completes the five steps to build a manga scene. Even Blender beginners can construct a manga-like 3D scene in a few clicks. Now:

**Use composition and camera work to draw your world.**

Refer to the summary below.

## <i class="bi bi-rainbow"></i>   Summary

| Step | Feature | Purpose |
|:---:|:---|:---|
| 1 | Generate 3D Manga Collection | Prepare collections/outliner for production |
| 2 | Camera Settings | Configure the render camera |
| 3 | Light Collection Management | Set up the lighting environment |
| 4 | Material & Outline Generation | Create materials and outlines |
| 5 | Tone Shader Tuning | Finalize tone rendering |
