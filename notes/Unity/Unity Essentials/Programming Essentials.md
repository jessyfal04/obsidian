# Add a movement script
## Review
Explain how code is edited in a Unity project.
Make a new script component.
Add a script component to a GameObject.
Open the IDE from the Unity Editor.
Assign a camera as a child GameObject that follows the player.
 Adjust component properties temporarily in Play mode (Game view). 

# Create a rotating collectible
## Review
Explain the using statements at the top of a Unity script.
Identify a class declaration in a script.
Explain the MonoBehaviour class in Unity scripts.
Explain the Start() and Update() functions in a Unity script.
Call a transform function in the Update() method to transform a GameObject over time.
Apply correct data types in code, including integers and floats.
Declare new custom variables in a script.
Explain how public variables in a script behave in Unity.
Describe common naming conventions including PascalCase and camelCase.
Apply correct naming conventions to variables and methods.

# Collect the collectible
## Review
Set up a collider as a trigger instead of a physical boundary.
Apply the OnTriggerEnter() function to detect collisions with other objects.
Devise comments that describe a given block or line of code.
Apply the Destroy() function to remove objects from a scene.
Code quickly using the autocomplete feature of the IDE.
Explain how visual effects (VFX) can be used to give the user visual feedback.
Declare a variable with the data type of GameObject.
Apply the Instantiate() function to spawn prefab instances in a scene.
Apply snapping with the Move tool to align and evenly space out GameObjects.
Apply if statements to control the logic and flow of a script.
Apply tags to GameObjects in order to identify them in a script.

# Quizz
## Question 1

Which of the following are true about scripting in Unity?

Select the three correct answers.

Select all correct answers

An external script editor must be used for coding, since you can’t write code directly inside the Unity Editor.

Unity only supports JavaScript for game development and interaction logic.

C# is the default scripting language used in Unity for creating game logic and interactions.

Scripts attached to GameObjects can control their behavior, animations, and interactions within the game.

Correct

- "Unity only supports JavaScript for game development and interaction logic." — This statement is incorrect. While Unity previously supported a variant of JavaScript (UnityScript), it has since been deprecated in favor of C#, which is now the only officially supported scripting language in Unity.
    

  

## Question 2

What is the purpose of the Update() function, which appears by default in any new script you create in Unity?

Select the one correct answer.

Select only one

To initialize variables and set up game state before the game starts.

To save game data when exiting the game or application.

To manage the loading and unloading of game assets and scenes dynamically.

To handle actions that need to occur on a frame-by-frame basis.

Correct

- "To initialize variables and set up game state before the game starts." — This statement is incorrect. Initialization and setup are typically handled in the Start() function, not the Update() function.
    
- "To save game data when exiting the game or application." — This statement is incorrect. Saving tasks are not the purpose of the Update() function; these are usually handled in other specific event functions or by explicitly calling methods for saving data.
    
- "To manage the loading and unloading of game assets and scenes dynamically." — This statement is incorrect. While the Update() function can trigger asset or scene loading based on certain conditions, its primary purpose is not to manage assets or scenes but to perform regular updates to game logic.
    

  

## Question 3

There are two errors in the line of code below. What are the errors?

transform.Rotate(0, 0.25, 0) >

Select the two correct answers.

Select all correct answers

The number 0.25 should have an "f" suffix to explicitly indicate it is a float (0.25f).

The transform object needs to be capitalized (Transform) to be correctly referenced in Unity.

The Rotate method does not accept three arguments.

The line of code should end with a semicolon (;) instead of a greater than sign (>).

Correct

- "The Rotate method does not accept three arguments.” — This statement is incorrect. The Rotate method in Unity can indeed accept three arguments, representing the Euler angles to rotate the object in the X-, Y-, and Z-axes, respectively.
    
- "The transform object needs to be capitalized (Transform) to be correctly referenced in Unity.” — This statement is incorrect. In Unity scripts, the transform property of a GameObject is correctly referred to in lowercase to access its Transform component.
    

  

## Question 4

Which statements are true about variables in C# programming?

Select the three correct answers.

Select all correct answers

Variables in C# can be of any data type, including integers, floats, and even GameObjects.

Variables must be declared within the Start() function of a script.

Variables in C# often use camelCase notation, where the first letter of the first word is lowercase, and the first letter of each subsequent word is capitalized.

Variables can appear in the Unity Inspector window if they are declared as public within the script.

Correct

- "Variables must be declared within the Start() function of a script. " — This statement is incorrect. Something called local variables can be declared within a specific function like Start(), but these variables can be declared in any function, not just the Start() function. Global variables that can be used anywhere in the script must actually be declared outside of the Start function.
    

  

## Question 5

You have the code below in a Collectible script, but for some reason, when the Player GameObject collides with the collectible, the collectible doesn’t disappear. What could explain this?

  

    private void OnTriggerEnter(Collider other) {   
           if (other.CompareTag("Player")) {
                Destroy(gameObject);
           }
    }

Select the two correct answers.

Select all correct answers

Instead of “OnTriggerEnter”, it should say “OnPlayerEnter”.

The Player GameObject does not have the Player tag applied.

There is a missing semicolon in the code snippet above.

The collectible object with this script attached does not have Is Trigger enabled in its Collider component.

Correct

- “There is a missing semicolon in the code snippet above.” — this statement is incorrect. C# uses the semicolon as a statement terminator. There are no other semicolons required in that code.
    
- “Instead of “OnTriggerEnter”, it should say ‘OnPlayerEnter’” — this statement is incorrect. “OnTriggerEnter” is a standard Unity event that is called when one object enters the trigger area of another object.
    

  

## Question 6

What does the Instantiate() method do in a Unity script?

Select the one correct answer.

Select only one

It deletes a specified GameObject from the scene after a delay.

It compiles the script at runtime, allowing for dynamic code changes.

It creates a new GameObject or a copy of an object at runtime, including all its components and properties.

Pauses the execution of the script for a specified amount of time.

Correct

- "It compiles the script at runtime, allowing for dynamic code changes." — This statement is incorrect. The Instantiate() method is used to create new instances of objects, not to compile scripts.
    
- "Deletes a specified GameObject from the scene after a delay." — This statement is incorrect. Deleting objects is the purpose of the Destroy method, not Instantiate.
    
- "Pauses the execution of the script for a specified amount of time." — This statement is incorrect. Pausing script execution is achieved with the WaitForSeconds function within coroutines, not with Instantiate.