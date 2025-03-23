# Set up a 2D room

## Review
Switch between 2D view and 3D view of a scene.
Explain the differences between navigating in 2D space vs. 3D space.
Define sprite.
Adjust the aspect ratio of Game view to playtest using the same view that users will see.
Use the Rect tool to move and scale 2D objects.
Explain the differences between 2D colliders and 3D colliders.
Duplicate a GameObject.
# Complete your 2D Puzzle Game
## Review
Set the Order in Layer property to control how objects appear in a 2D scene.
Explain how 9-sliced sprites work.
Adjust Rigidbody properties, including mass and damping, to control how objects respond to physical forces.
Explain why scripts for 2D interactions use 2D functions.

# Add an animated pet
## Review
Define sprite sheet.
Explain how a sprite sheet can be used to create animated 2D objects.
Slice sprite sheets into individual images using the Sprite Editor.
Make an animated sprite sheet that loops through frames.

# Quizz
Question 1
What happens when you turn on 2D mode in the Scene view? 
Select the one correct answer. 
Select only one


Locks the Scene view camera to a fixed position, preventing any movement or rotation.
Enables the physics simulation to run in two dimensions, disabling the Z-axis.
Automatically converts all 3D models in the scene to 2D sprites.
Turns off perspective and orients the camera to look towards positive Z, with the X-axis pointing right and the Y-axis pointing up.
Correct

"Automatically converts all 3D models in the scene to 2D sprites." — This statement is incorrect. The 2D mode affects the Scene view's camera perspective only and does not convert 3D models into 2D sprites.
"Locks the Scene view camera to a fixed position, preventing any movement or rotation." — This statement is incorrect. While the camera in 2D mode is optimized for 2D space navigation, users can still move and zoom within the Scene view.
"Enables the physics simulation to run in two dimensions, disabling the Z-axis." — This statement is incorrect. The physics simulation mode (2D or 3D) is determined by the components used (Rigidbody2D vs. Rigidbody) and is independent of the Scene view mode. 

Question 2
Which of the following are actually built-in Unity components optimized for 2D development? 
Select the two correct answers. 
Select all correct answers


Rigidbody 2D
Square Renderer 2D
Layer Adjuster 2D
Circle Collider 2D
Correct

"Square Renderer 2D" — This statement is incorrect. While Unity provides components for rendering 2D shapes, such as the Sprite Renderer, there is no specific "Square Renderer 2D" component. 2D shapes are typically handled by using sprites or meshes with appropriate materials.
"Layer Adjuster 2D" — This statement is incorrect. There is no built-in Unity component named "Layer Adjuster 2D." Layering in Unity is typically managed through camera settings, sorting layers, and the Z-position of objects for 2D games, or through the use of 3D components and positioning for 3D games.

Question 3
Which of the following are true about the Rect tool in Unity? 
Select the two correct answers. 
Select all correct answers


It's designed for creating and editing physical materials for 2D objects.
It adjusts the transparency and color settings of UI elements.
It is used for manipulating the position and scale of 2D objects in the scene.
The Rect tool can be activated using the T key as a shortcut in the Scene view.
Correct

"It adjusts the transparency and color settings of UI elements." — This statement is incorrect. The Rect tool is focused on spatial manipulation (position, rotation, scale) rather than visual properties like transparency and color, which are adjusted in the Inspector window through component properties.
"It's designed for creating and editing physical materials for 2D objects." — This statement is incorrect. The Rect tool does not deal with materials or textures directly; it's used for spatial manipulation of objects in the scene, particularly UI elements and 2D sprites. 

Question 4
What does the Order in Layer property do in the Sprite Renderer component? 
Select the one correct answer. 
Select only one


Controls the level of detail that the sprite is rendered with, improving performance for distant objects.
Determines the rendering order of sprites, allowing some to appear in front of or behind others. 
Adjusts the sprite's color intensity based on its position in the scene. 
Sets the physical layer the sprite belongs to for collision detection purposes.
Correct

"Adjusts the sprite's color intensity based on its position in the scene." — This statement is incorrect. The Order in Layer property affects the sprite's rendering order, not its color intensity.
"Controls the level of detail that the sprite is rendered with, improving performance for distant objects." — This statement is incorrect. The Order in Layer property does not affect the level of detail or the performance optimization of sprites; it solely determines their rendering order.
"Sets the physical layer the sprite belongs to for collision detection purposes." — This statement is incorrect. The Order in Layer property is used for rendering order, not for setting physical layers for collision detection, which is managed by the Layer property in the GameObject's settings.

Question 5
Which of the following is true about writing scripts for 2D GameObjects in Unity?
Select the one correct answer.
Select only one


To work with 2D GameObjects in Unity, you must create a special kind of script asset from the Project window’s create menu named a “Script2D”, which is distinct from those used in 3D development.
All scripting methods and components used for 3D GameObjects are incompatible with 2D GameObjects, requiring separate libraries. 
Unity will not allow you to apply a script that has references to 2D components or methods onto a 3D object. 
Writing scripts for 2D GameObjects is largely the same as for 3D, but there are some methods optimized for 2D development, such as OnTriggerEnter2D instead of OnTriggerEnter. 
Correct

"To work with 2D GameObjects in Unity, you must create a special kind of script asset from the Project window’s create menu named a “Script2D”, which is distinct from those used in 3D development." — This statement is incorrect. Scripts in Unity can generally be used for both 2D and 3D development, with the main differences being in the specific components and methods used rather than the script's fundamental structure.
"Unity will not allow you to apply a script that has references to 2D components or methods onto a 3D object." — This statement is incorrect. Unity does allow the application of scripts referencing 2D components to 3D objects, though the 2D-specific components and methods may not function as intended on 3D objects without corresponding 2D components.
"All scripting methods and components used for 3D GameObjects are incompatible with 2D GameObjects, requiring separate libraries." — This statement is incorrect. Many scripting methods and components are compatible or have analogous versions across 2D and 3D development in Unity, allowing for a cohesive development experience without needing entirely separate libraries.