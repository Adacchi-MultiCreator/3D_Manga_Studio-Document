# <i class="bi bi-menu-button-fill"></i>   Manga Tone Shader Specifications
![MTS Object](assets/img/EN/MTS section.png)

"Manga Tone Shader" is a toon shader specialized for manga/comic expressions, designed specifically for toon rendering.

## <i class="bi bi-exclamation-diamond-fill"></i>  Characteristics
Unlike typical toon shaders, it allows color assignment per highlight region using dedicated lighting.

It uses three lights (Key, Fill, Back) colored red (#ff0000), green (#00ff00), and blue (#0000ff). The shader extracts the contribution from each and maps colors or patterns per region.

!!! note "Note"
	- The three lights are created in the light collection under "B: Lighting".
	- The light regions depend not only on offset values but also on light strengths in the light collection. Adjust light strengths first, then tweak offsets.

Each lit side has its own color input. Drag & drop paid materials onto the material inputs below the color fields to project patterns onto those regions.

## <i class="bi bi-stack"></i>  Structure
Manga Tone Shader has the following structure:

![Layer structure](assets/img/EN/MTS layer.png)

## <i class="bi bi-list-task"></i>  Property list and effects

### Property Index

  - <a href="#base-tone">Base Tone</a>
  - <a href="#key-tone">Key Tone</a>
  - <a href="#fill-tone">Fill Tone</a>
  - <a href="#back-tone">Back Tone</a>
  - <a href="#shadow">Shadow</a>
  - <a href="#sub-outline">Sub Outline</a>
  - <a href="#ao">AO (Ambient Occlusion)</a>
  - <a href="#soft-shadow-tone">Soft Shadow Tone</a>
  - <a href="#hard-shadow-tone">Hard Shadow Tone</a>
  - <a href="#gloss">Gloss</a>
  - <a href="#anisotropy">Anisotropy</a>
  - <a href="#mat">Mat</a>
  - <a href="#rim-light">Rim Light</a>

<div style="display: flex !important; gap: 5px !important; align-items: flex-start !important;">

<div style="flex: 0 0 50% !important; padding: 0 !important; margin: 0 !important;">
<h3 style="margin-top: 0 !important;">Node image</h3>
<img src="/assets/img/EN/MTS%20property%20list.png" alt="Manga Tone Shader node image" style="width: 100% !important; display: block !important; margin: 0 !important; padding: 0 !important;">

</div>

<div style="flex: 0 0 50% !important; padding: 0 !important; margin: 0 !important; padding-left: 5px !important;">

<h3 id="property-list" style="margin-top: 0 !important;">Property list</h3>

<h4 id="base-tone">Base Tone</h4>
<ul>
<li><strong>Color</strong>: Base color.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
</ul>

<h4 id="key-tone">Key Tone</h4>
<ul>
<li><strong>Color</strong>: Color for the key-lighted area. Drag & drop a material in the slot to overlay a pattern.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
<li><strong>Key Light Offset</strong>: Offset for key light.</li>
<img src="/assets/img/compare/key_offsets.png" alt="Key light offset comparison">
</ul>

<h4 id="fill-tone">Fill Tone</h4>
<ul>
<li><strong>Color</strong>: Color for the fill-lighted area. Drag & drop a material to overlay a pattern.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
<li><strong>Fill Light Offset</strong>: Offset for fill light.</li>
<img src="/assets/img/compare/fill_offsets.png" alt="Fill light offset comparison">
</ul>

<h4 id="back-tone">Back Tone</h4>
<ul>
<li><strong>Color</strong>: Color for the back-lighted area. Drag & drop a material to overlay a pattern.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
<li><strong>Back Light Offset</strong>: Offset for back light.</li>
<img src="/assets/img/compare/back_offsets.png" alt="Back light offset comparison">
</ul>

<h4 id="shadow">Shadow</h4>
<p>Shadow settings.</p>
<ul>
<li><strong>Color</strong>: Shadow color.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
<li><strong>Shadow Opacity</strong>: Shadow opacity.</li>
<img src="/assets/img/compare/shadow_oppacity.png" alt="Shadow opacity comparison">
<li><strong>Brightness</strong>: Shadow brightness.</li>
<img src="/assets/img/compare/shadow_strong.png" alt="Shadow brightness comparison">
<li><strong>Contrast</strong>: Shadow contrast.</li>
<img src="/assets/img/compare/shadow_contrast.png" alt="Shadow contrast comparison">
</ul>

<h4 id="sub-outline">Sub Outline</h4>
<p>Inner outline settings.</p>
<ul>
<li><strong>Color</strong>: Inner outline color.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
<li><strong>Opacity</strong>: Sub outline opacity.</li>
<img src="/assets/img/compare/sub_outline_opacity.png" alt="Sub outline opacity comparison">
<li><strong>Size</strong>: Sub outline size.</li>
<img src="/assets/img/compare/sub_outline_size.png" alt="Sub outline size comparison">
<li><strong>Shadow Size</strong>: Shadow size.</li>
<img src="/assets/img/compare/sub_outline_shadow size.png" alt="Shadow size comparison">
</ul>

<h4 id="ao">AO (Ambient Occlusion)</h4>
<p>Ambient occlusion settings.</p>
<ul>
<li><strong>Opacity</strong>: AO opacity.</li>
<img src="/assets/img/compare/AO_opacity.png" alt="AO opacity comparison">
<li><strong>Shadow Opacity</strong>: AO shadow opacity.</li>
<img src="/assets/img/compare/AO_shadow_opacity.png" alt="AO shadow opacity comparison">
<li><strong>Mask</strong>: Mask to limit AO. Create a grayscale image with the New button in the image selector below.</li>
<img src="/assets/img/compare/AO_mask.png" alt="AO mask comparison">
<li><strong>Soft/Hard Switch</strong>: Balance between soft and hard shadows.</li>
<img src="/assets/img/compare/soft_hard_switch.png" alt="Soft/Hard switch comparison">
</ul>

<h4 id="soft-shadow-tone">Soft Shadow Tone</h4>
<ul>
<li><strong>Soft Intensity</strong>: Soft shadow intensity.</li>
<img src="/assets/img/compare/soft_strong.png" alt="Soft shadow intensity comparison">
</ul>

<h4 id="hard-shadow-tone">Hard Shadow Tone</h4>
<ul>
<li><strong>Hard Intensity</strong>: Hard shadow intensity.</li>
<img src="/assets/img/compare/hard_strong.png" alt="Hard shadow intensity comparison">
</ul>

<h4 id="gloss">Gloss</h4>
<p>Gloss settings.</p>
<ul>
<li><strong>Color</strong>: Gloss color.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
<li><strong>Opacity</strong>: Gloss opacity.</li>
<img src="/assets/img/compare/gloss_opacity.png" alt="Gloss opacity comparison">
<li><strong>Brightness</strong>: Gloss brightness.</li>
<img src="/assets/img/compare/gloss_strong.png" alt="Gloss brightness comparison">
<li><strong>Contrast</strong>: Gloss contrast.</li>
<img src="/assets/img/compare/gloss_contrast.png" alt="Gloss contrast comparison">
<li><strong>Spread</strong>: Gloss spread.</li>
<img src="/assets/img/compare/gloss_spread.png" alt="Gloss spread comparison">
<li><strong>Offset X</strong>: Gloss X offset.</li>
<img src="/assets/img/compare/gloss_offsets_x.png" alt="Gloss X offset comparison">
<li><strong>Offset Z</strong>: Gloss Z offset.</li>
<img src="/assets/img/compare/gloss_offsets_z.png" alt="Gloss Z offset comparison">
</ul>

<h4 id="anisotropy">Anisotropy</h4>
<p>Anisotropic highlight settings.</p>
<ul>
<li><strong>Color</strong>: Color for hair-like sheen; can drop a material to overlay a pattern.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
<li><strong>Opacity</strong>: Anisotropy opacity.</li>
<img src="/assets/img/compare/anisotropy_oapcity.png" alt="Anisotropy opacity comparison">
<li><strong>Brightness</strong>: Anisotropy brightness.</li>
<img src="/assets/img/compare/anisotropy_strong.png" alt="Anisotropy brightness comparison">
<li><strong>Contrast</strong>: Anisotropy contrast.</li>
<img src="/assets/img/compare/anisotropy_contrast.png" alt="Anisotropy contrast comparison">
<li><strong>Density</strong>: Anisotropy density.</li>
<img src="/assets/img/compare/anisotropy_density.png" alt="Anisotropy density comparison">
<li><strong>Shadow Opacity</strong>: Anisotropy shadow opacity.</li>
<img src="/assets/img/compare/anisotropy_shadow_opacity.png" alt="Anisotropy shadow opacity comparison">
<li><strong>Shadow Contrast</strong>: Anisotropy shadow contrast.</li>
<img src="/assets/img/compare/anisotropy_shadow_contrast.png" alt="Anisotropy shadow contrast comparison">
<li><strong>Offset Z</strong>: Anisotropy Z offset.</li>
<img src="/assets/img/compare/anisotropy_ofssets_z.png" alt="Anisotropy Z offset comparison">
<li><strong>Camera View Offset</strong>: Offset relative to camera view.</li>
<img src="/assets/img/compare/anisotropy_camera_ofssets.png" alt="Camera view offset comparison">
</ul>

<h4 id="mat">Matte</h4>
<p>Texture used to simulate material traits.</p>
<ul>
<li><strong>Color</strong>: Color; use the image chooser to create a new grayscale texture.</li>
<img src="/assets/img/compare/mat_color.png" alt="Matte color comparison">
<li><strong>Opacity</strong>: Matte opacity.</li>
<img src="/assets/img/compare/mat_opacity.png" alt="Matte opacity comparison">
<li><strong>Brightness</strong>: Matte brightness.</li>
<img src="/assets/img/compare/mat_strong.png" alt="Matte brightness comparison">
<li><strong>Contrast A</strong>: Matte contrast A.</li>
<img src="/assets/img/compare/mat_contrast_a.png" alt="Matte contrast A comparison">
<li><strong>Contrast B</strong>: Matte contrast B.</li>
<img src="/assets/img/compare/mat_contrast_b.png" alt="Matte contrast B comparison">
</ul>

<h4 id="rim-light">Rim Light</h4>
<p>Rim light settings.</p>
<ul>
<li><strong>Color</strong>: Color for the inner outline; can drop a material to overlay a pattern.</li>
<li><strong>Material</strong>: Drop slot for an Asset Browser material.</li>
<li><strong>Opacity</strong>: Rim light opacity.</li>
<img src="/assets/img/compare/rim_light_oapcity.png" alt="Rim light opacity comparison">
<li><strong>Contrast</strong>: Rim light contrast.</li>
<img src="/assets/img/compare/rim_light_contrast.png" alt="Rim light contrast comparison">
<li><strong>Width</strong>: Rim light width.</li>
<img src="/assets/img/compare/rim_light_width.png" alt="Rim light width comparison">
<li><strong>Offset X</strong>: Rim light X offset.</li>
<img src="/assets/img/compare/rim_light_offsets_x.png" alt="Rim light X offset comparison">
<li><strong>Offset Z</strong>: Rim light Z offset.</li>
<img src="/assets/img/compare/rim_light_offsets_z.png" alt="Rim light Z offset comparison">
</ul>

</div>

</div>
