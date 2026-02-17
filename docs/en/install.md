# <i class="bi bi-cloud-download-fill"></i>   Installation and Uninstallation

This section explains how to install the 3D Manga Studios add-on.

## <i class="bi bi-file-earmark-zip-fill"></i>   Download the add-on

Purchase the add-on on SUPERHIVE (formerly BlenderMarket).
After purchase, go to the downloads page and download the file named "3D_Manga_Studios.zip".

## <i class="bi bi-file-earmark-zip-fill"></i>   Download the paid materials (optional)

There are optional paid materials dedicated to this add-on on SUPERHIVE (formerly BlenderMarket).
After purchase, go to the downloads page and download the file named "Manga Tone Shader Assets.zip".
The archive contains both Japanese and English asset files. Materials are identical, so you can use either.

!!! note "Download page"
    Add-on product page

    <i class="bi bi-arrow-up-right-circle-fill"></i>   [3D Manga Studios Download page](https://superhivemarket.com/products/3d-manga-studios)

## <i class="bi bi-file-earmark-arrow-down-fill"></i>   Install the add-on in Blender

### Method 1
1. Keep the downloaded "3D_Manga_Studios.zip" as-is without extracting.
2. Launch Blender and drag & drop the ZIP file into the Blender window. The 3D Manga Studios add-on will appear in the N-panel.

!!! note "The side panel (N-panel) is not visible"
    - In Preferences > Add-ons, search for "3D Manga Studios" and make sure the checkbox is ON.

    - Press ++n++ to toggle the N-panel on the right side of the 3D Viewport. If many add-ons are listed, scroll to find it.

### Method 2
1. Launch Blender and go to Edit > Preferences.
2. Click the Add-ons tab on the left.
3. Click Install, select the downloaded ZIP file, and press Install Add-on.
4. After installation, the add-on appears in the list. Enable it by turning on its checkbox.

!!! note "The add-on cannot be found"
    If you cannot find it, search for "3D Manga Studios" in the search box.

!!! note "The side panel (N-panel) is not visible"
    - In Preferences > Add-ons, search for "3D Manga Studios" and make sure the checkbox is ON.

    - Press ++n++ to toggle the N-panel on the right side of the 3D Viewport.

### Registering Manga Tone Shader assets to the Asset Browser
1. Extract the downloaded "Manga Tone Shaders.zip".
2. After extracting, it should have the following structure:

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
4. Click the File Paths tab.
5. Scroll to Asset Libraries, click "Open Folders".
6. Select the path to the "Manga Tone Shader" folder you extracted and click "Open Folder".
7. Save preferences and close.
8. Split an area and change the editor type to Asset Browser.
9. Use assets from the newly registered library.

## <i class="bi bi-file-earmark-x-fill"></i>   Uninstall
1. Go to Edit > Preferences.
2. Open Add-ons tab.
3. Find "3D Manga Studios", expand details, and click Remove.
