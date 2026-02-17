# <i class="bi bi-cart-plus-fill"></i>   About Paid Screen Tone Materials
3D Manga Studios provides optional paid screen tone materials to broaden your expression. These are sold as paid assets on SUPERHIVE (formerly Blender Market). By purchasing, you can achieve richer manga styles.

!!! warning "Notes"
    - You can use non-dedicated materials, but Manga Tone Shader effects may not work correctly and the following issues could occur:
    
    | Freeze | Broken material |
    | --- | --- |
    |![Freeze](assets/img/EN/freeze.png)|![Broken](assets/img/EN/error.png)|

    - Blender may freeze
    - Materials may fail to display (pink/purple)
    
    For stability, using the dedicated materials is strongly recommended.

## Registering Screen Tone Materials to the Asset Browser
1. Extract the downloaded "Manga Tone Shaders.zip".
2. The structure will be:

        Manga Tone Shaders/
                ├──── ★Shader Screen tones/
                │  ├──── JP/
                │  │  └──── Screen shader tones/
                │  │      ├── Screen shader tones.blend
                │  │      └── Readme_JP.txt
                │  └──── US_UK/
                │      └──── Screen shader tones/
                │          ├── Screen shader tones.blend
                │          └── Readme_JP.txt
                ├──── ★UnShader Screen tones/
                │  ├──── JP/
                │  │  └──── Screen tones/
                │  │      ├── Screen tones.blend
                │  │      └── Readme_US_UK.txt
                │  └──── US_UK/
                │      └──── Screen tones/
                │          ├── Screen tones.blend
                │          └── Readme_US&UK.txt
                └──────── Manga Tone Shader/
                        ├── Manga Tone Shader.blend
                        ├── Readme_JP.txt
                        └── Readme_US&UK.txt

3. Go to Edit > Preferences.
4. Open File Paths tab.
5. Scroll to Asset Libraries and click Open Folders.
6. In the extracted folder, open the "★UnShader Screen tones" folder, then choose JP (Japanese) or US_UK (English) and select the path under "Screen tones". Click Open Folder.
7. Save preferences and close.
8. Split an area and change the editor to Asset Browser.
9. From the Library dropdown, select the newly registered "Screen tones" library.

## Screen Tone Materials List
Available dedicated screen tones:

| Material | Preview | Description |
|:---|:---:|:---|
| Faded Crosshatch Tone | ![Faded Crosshatch Tone](assets/img/screen tones/0006.png) | Crosshatch with faded analog feel. |
| Halftone Dots | ![Halftone Dots](assets/img/screen tones/0001.png) | Basic halftone dots for shadows or clothing patterns. |
| Hatch Tone A | ![Hatch Tone A](assets/img/screen tones/0003.png) | Simple diagonal hatch. |
| Hatch Tone B | ![Hatch Tone B](assets/img/screen tones/0004.png) | Denser than Hatch A. |
| Hatch Tone C | ![Hatch Tone C](assets/img/screen tones/0005.png) | Even denser; suitable for darker shadows. |
| Noisy Halftone | ![Noisy Halftone](assets/img/screen tones/0007.png) | Irregular noisy halftone for gritty feels. |
| Parallel Lines Tone | ![Parallel Lines Tone](assets/img/screen tones/0009.png) | Parallel lines; good for backgrounds and speed effects. |
| Sand Grain Tone | ![Sand Grain Tone](assets/img/screen tones/0010.png) | Sand-like grains for rough textures or light shadows. |
| Pencil-like Overlap Tone | ![Pencil-like Overlap Tone](assets/img/screen tones/0008.png) | Pencil-styled overlapping hatch for hand-drawn looks. |
| 4-Way Hatch Tone | ![4-Way Hatch Tone](assets/img/screen tones/0002.png) | Four-way hatch for very dense tone or special textures. |

## <i class="bi bi-journal-richtext"></i>   Using with Manga Tone Shader
These materials work best combined with Manga Tone Shader.

### Steps
1. Open the Asset Browser.
2. Choose a material in the Screen tones library.
3. Open the `Manga Tone Shader` properties on the object.
   Drag & drop the material into the drop slot below a target color input (Shadow, Highlight, etc.).

    | Before | After |
    | --- | --- |
    |![Before](assets/img/EN/MTS DD.png)|![After](assets/img/EN/MTS DD after.png)|

4. Adjust dropped material properties (scale, rotation, etc.) as needed.

    | Before | After |
    | --- | --- |
    |![Before](assets/img/EN/MTS DD property.png)|![After](assets/img/EN/MTS DD property after.png)|

See also: [Manga Tone Shader docs](mangaToneShader.md).
