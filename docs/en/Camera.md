# <i class="bi bi-camera-fill"></i>  Camera Settings
![Section](assets/img/EN/camera section.png)

This section describes camera settings.

## <i class="bi bi-journal-richtext"></i>  Steps

### Camera Type
![Camera type](assets/img/EN/camera type.png)

Two projection types are available: Perspective (with depth) and Orthographic (parallel, good for isometric views).
 
- Perspective: Great for action scenes and environments; emphasizes depth.

    ![Perspective](assets/img/EN/camera perse.png)

- Orthographic: Good for top/side views of characters and backgrounds; no depth, suitable for stylized looks.

    ![Orthographic](assets/img/EN/camera orthographic.png)

### Focal Length and View Scale  <i class="bi bi-patch-check-fill">NEW@1.0.1</i>
Focal length adjusts the strength of perspective. The shorter the focal length, the stronger the perspective; the longer the focal length, the weaker the perspective.
Ortho scale adjusts the magnification. Increasing the scale narrows the visible area, while decreasing the scale widens it.

![Focal length properties](assets/img/EN/camera scale perse.png)
![Ortho scale properties](assets/img/EN/camera scale orthographic.png)

### Camera Size
![Camera size](assets/img/EN/camera size.png)

Set the render size. Presets for common manga sizes are provided.

- Resolution X: Width in pixels.
- Resolution Y: Height in pixels.
- Percentage: Scale of render resolution.
- Presets: Choose from common manga sizes.

    ![Presets](assets/img/EN/camera size presets.png)

- Safe Areas: Toggle safe areas. They help ensure important content isn’t cut at print. When enabled, you can configure:
  
    ![Safe areas](assets/img/EN/camera safearea.png)
    
    1. Safe Area Mode: Choose Uniform or Separate.
        ![Mode](assets/img/EN/camera type select.png)

        1. Uniform: Same margin on all sides.

            ![Uniform](assets/img/EN/camera type uniform.png)

            - Margin (px): Margin from the render area edge in pixels.

        2. Separate: Different values for horizontal and vertical sides.

            ![Separate](assets/img/EN/camera type separate.png)

            - Left/Right (px): Horizontal margins in pixels.
            - Top/Bottom (px): Vertical margins in pixels.

    2. Line Width: Thickness of safe area lines.

        ![Width](assets/img/EN/camera safearea width.png)

    3. Color: Color and alpha of safe area lines.

        ![Color](assets/img/EN/camera safearea color.png)


!!!note "About presets"
	The following presets are available.
    
    When Safe Areas are enabled, choosing a preset sets 50 px margins on each side automatically.

    Note: Values are 100x for convenience (pixel-based).

    <div style="display:flex; gap:2rem; align-items:flex-start; flex-wrap:wrap; margin:0 0 1rem 0;">
      <div>
        <h4>A Series</h4>
        <table>
          <thead>
            <tr><th>Preset</th><th>Ratio (W×H)</th></tr>
          </thead>
          <tbody>
            <tr><td>A</td><td>21000×29700</td></tr>
            <tr><td>A half (portrait)</td><td>21000×14850</td></tr>
            <tr><td>A third (portrait)</td><td>21000×9900</td></tr>
            <tr><td>A quarter (portrait)</td><td>21000×7425</td></tr>
            <tr><td>A fifth (portrait)</td><td>21000×5940</td></tr>
            <tr><td>A half (landscape)</td><td>10500×29700</td></tr>
            <tr><td>A third (landscape)</td><td>7000×29700</td></tr>
            <tr><td>A quarter (landscape)</td><td>5250×29700</td></tr>
            <tr><td>A fifth (landscape)</td><td>4200×29700</td></tr>
            <tr><td>A sixth (landscape)</td><td>3500×29700</td></tr>
          </tbody>
        </table>
      </div>

      <div>
        <h4>B Series</h4>
        <table>
          <thead>
            <tr><th>Preset</th><th>Ratio (W×H)</th></tr>
          </thead>
          <tbody>
            <tr><td>B</td><td>25700×36400</td></tr>
            <tr><td>B half (portrait)</td><td>25700×18200</td></tr>
            <tr><td>B third (portrait)</td><td>25700×12133</td></tr>
            <tr><td>B quarter (portrait)</td><td>25700×9100</td></tr>
            <tr><td>B fifth (portrait)</td><td>25700×7280</td></tr>
            <tr><td>B half (landscape)</td><td>12850×36400</td></tr>
            <tr><td>B third (landscape)</td><td>8566×36400</td></tr>
            <tr><td>B quarter (landscape)</td><td>6425×36400</td></tr>
            <tr><td>B fifth (landscape)</td><td>5140×36400</td></tr>
            <tr><td>B sixth (landscape)</td><td>4283×36400</td></tr>
          </tbody>
        </table>
      </div>
    </div>

### Layout Guides
![Layout guides](assets/img/EN/camera layout.png)

Toggle layout guides, which help with paneling and character placement. When enabled:

- Column Guides: Vertical splits from 2 to 100 columns.

    ![Columns](assets/img/EN/camera layout  column.png)

- Row Guides: Horizontal splits from 2 to 100 rows.

    ![Rows](assets/img/EN/camera layout  row.png)
 
- Guide Line Width: Thickness of guide lines.

    ![Width](assets/img/EN/camera layout  width.png)

- Guide Color: Color and alpha of guide lines.

    ![Color](assets/img/EN/camera layout color.png)
