# <i class="bi bi-lightbulb-fill"></i>  Light Collection Management
![Section](assets/img/EN/light section.png)

After applying materials and outlines, manage light collections. You can add, toggle visibility, and remove them.

## <i class="bi bi-journal-richtext"></i>  Steps

### Add a Light Collection
![Added](assets/img/EN/light add.png)

1. Ensure that within "3D Manga Collection" there is a collection named "B: Lighting".
2. In the Light Collection section, click the "+ Add" button.
3. Enter a name for the light collection and click OK.
4. A new light collection is added under "B: Lighting".

	![Collections](assets/img/EN/light collection.png)

	The light collection includes three lights, a collection, and a target empty.

	- Key Light: The main light for illuminating the subject.
	- Fill Light: A secondary light to soften shadows from the key light.
	- Back Light: A rim/back light to separate the subject from the background.
	- Light Linking: Configure which objects a light affects. For example, make a light affect only the background but not the character.

		!!! note "Note"
			Drag and drop collections containing objects into the LightLink collection with ++ctrl++ held to limit a light's influence to objects inside the dropped collection.
    	!!! warning "Caution"
            To use Light Linking, you must create one or more collections under "1: Characters / Objects".

	- Target: An empty that all three lights aim at.
    	!!! note "Note"
    		Moving the target empty changes the direction of all lights together.
!!! warning "Important"
	You must press "Create 3D Manga Collection" in the "Generate 3D Manga Collection" section first. Otherwise, you cannot add a light collection.
	Always create the dedicated collections first, then add a light collection.
	
	![Generated](assets/img/EN/collection generated.png)

### Toggle Light Collection Visibility
1. The Light Collection List shows all light collections.
2. Use the checkbox at the left of each collection to toggle its visibility. Unchecked collections are hidden and do not affect renders.

| Visible | Hidden |
| --- | --- |
| ![On](assets/img/EN/light on.png) | ![Off](assets/img/EN/light off.png) |

### Light Strength
1. Select the light collection to adjust from the list.
2. The "Light Strengths" section appears below.
3. Adjust the sliders for Key, Fill, and Back to control the overall strength.

	![Strengths](assets/img/EN/light property.png)

### Remove a Light Collection
1. Select a light collection in the list.
2. Click "- Remove".

	![Remove](assets/img/EN/light remove.png)
