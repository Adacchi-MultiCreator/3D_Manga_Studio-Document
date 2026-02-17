# <i class="bi bi-question-circle-fill"></i>   Help

Frequently asked questions about the 3D Manga Studios add-on.

## 1. Installation

### Q1-1: The add-on doesn’t show in Blender.

A1-1: Check the following:

- Did you extract the ZIP? Install the ZIP directly without extracting.
- Is your Blender version supported? Confirm the version in `bl_info` matches your Blender.
- Is the add-on enabled? In Preferences > Add-ons, turn on the checkbox for 3D Manga Studios.

### Q1-2: Errors when installing.

A1-2: Read the error message. Common causes include incompatible Blender version, corrupt ZIP, or environment issues. Try restarting Blender or re-downloading the file.

## 2. Features

### Q2-1: Clicking "Create 3D Manga Collection" does nothing.

A2-1: Check the following:

- Are you in the 3D Viewport side bar (N key)? The panel is in the "3D Manga Studios" tab there.
- Any errors in the console? See Window > Toggle System Console. For messages like "B: Lighting Collection does not exist.", required collections may have been removed.

### Q2-2: "Apply Manga Tone Shader" doesn’t assign the shader.

A2-2: Check the following:

- Are objects selected? Select target mesh objects.
- Does a material named "Manga Tone Shader" exist? If not found, the add-on shows an error. Drag it once from Asset Browser to load it in the scene.

### Q2-3: Outline is not as expected.

A2-3: Check the following:

- Are mesh objects selected?
- Is a Solidify modifier named something like "MangaOutline" added? Verify its thickness, offset, and material offset values.
- Is a material named "Manga Line" assigned for outlines?

### Q2-4: Light Linking doesn’t work.

A2-4: Check the following:

- Does "B: Lighting" exist? Light linking depends on it and its children.
- Is your Blender version new enough to support Light Linking?
- Any console errors during initialization?

## 3. Translation

### Q3-1: UI is still in English.

A3-1: In Preferences > Interface > Translation, enable Interface and Tooltips and set the language to Japanese.

### Q3-2: Some text isn’t translated.

A3-2: The translation files (e.g., `translation/UI words.json` or `translation/Manga Tone Shader parameter.json`) may be missing a key. See the developer guide to add new entries.

## 4. Others

### Q4-1: How do I uninstall?

A4-1: Go to Preferences > Add-ons, search 3D Manga Studios, disable the checkbox, then click Remove. Restart Blender.

## Feedback

- **Email**: <mailto:arstchi.multidesigner@gmail.com>
- **Forum/Community**: <https://github.com/Adacchi-MultiCreator/3D-Manga-Studios-Issues>
- **SUPERHIVE Market (formerly Blender Market)**: <https://superhivemarket.com/products/3d-manga-studios--3d>
