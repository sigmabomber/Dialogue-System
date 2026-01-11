<img width="330" height="183" alt="image" src="https://github.com/user-attachments/assets/1f79aac3-c544-4812-b005-06d64ec858bb" /># Getting Started 

## 1. Creating a Dialogue Tree
Right-click in your Project window
Select Create > Dialogue System > Dialogue Tree
Name your dialogue asset (e.g., "GreetingDialogue")
<img width="803" height="352" alt="image" src="https://github.com/user-attachments/assets/808c9bae-d692-4194-bbfd-d23c4afc1e3e" />


## 2. Setting Up Basic Dialogue

In the Inspector for your Dialogue Tree:

Speaker Info (Optional)

Speaker Name: The name displayed in the dialogue UI (e.g., "Merchant", "Guard")

Dialogue Setup

Dialogue > Dialogue Text: The text that will be displayed
Dialogue > Voice Line: Optional AudioClip to play when this dialogue appears
Dialogue > Typewriter Speed: Characters per second (0 uses default from DialogueUI)

<img width="432" height="564" alt="image" src="https://github.com/user-attachments/assets/ddfa5e07-8664-45c6-86bc-a14f1ef78f8b" />

### Writing Dialogue with Effects

Basic Text
Just type normally:
#### Hello, traveler! Welcome to my shop.

<img width="408" height="162" alt="image" src="https://github.com/user-attachments/assets/2c53cc75-4deb-44a4-a551-b36d502ca76f" />
<img width="307" height="98" alt="image" src="https://github.com/user-attachments/assets/a4a87f98-703f-42e4-94fc-5e9e07f4a712" />

### Text Effects
You can combine multiple effects in a single tag:

### Highlight (Color)

<table>
<tr>
<th>Highlight</th>
<th></th>
<th>Examples</th>
</tr>
<tr>
<td>Color name</td>
<td></td>
<td><code>&lt;highlight(yellow) This text will be yellow&gt;</code></td>
</tr>
<tr>
<td>RGB color</td>
<td></td>
<td><code>&lt;highlight(255,0,0) RGB values&gt;</code> or <code>&lt;highlight(1,0,0) RGB values&gt;</code> or <code>&lt;highlight(rgb(255,0,0)) RGB values&gt;</code></td>
</tr>
<tr>
<td>RGBA color</td>
<td></td>
<td><code>&lt;highlight(255,0,0,128) RGBA values&gt;</code> or <code>&lt;highlight(1,0,0,0.5) RGBA values&gt;</code> or <code>&lt;highlight(rgba(255,0,0,128)) RGBA values&gt;</code></td>
</tr>
<tr>
<td>Hex color</td>
<td></td>
<td><code>&lt;highlight(#FF6B35) Custom hex color&gt;</code></td>
</tr>
</table>


### Supported Color Names
<table>
<tr>
<th>Color Name</th>
<th>RGB Values</th>
</tr>
<tr>
<td>red</td>
<td>(255, 0, 0)</td>
</tr>
<tr>
<td>green</td>
<td>(0, 255, 0)</td>
</tr>
<tr>
<td>blue</td>
<td>(0, 0, 255)</td>
</tr>
<tr>
<td>yellow</td>
<td>(255, 255, 0)</td>
</tr>
<tr>
<td>cyan</td>
<td>(0, 255, 255)</td>
</tr>
<tr>
<td>magenta</td>
<td>(255, 0, 255)</td>
</tr>
<tr>
<td>white</td>
<td>(255, 255, 255)</td>
</tr>
<tr>
<td>black</td>
<td>(0, 0, 0)</td>
</tr>
<tr>
<td>gray / grey</td>
<td>(128, 128, 128)</td>
</tr>
<tr>
<td>orange</td>
<td>(255, 128, 0)</td>
</tr>
<tr>
<td>purple</td>
<td>(128, 0, 128)</td>
</tr>
<tr>
<td>pink</td>
<td>(255, 192, 203)</td>
</tr>
<tr>
<td>brown</td>
<td>(153, 76, 0)</td>
</tr>
</table>

<img width="401" height="182" alt="image" src="https://github.com/user-attachments/assets/f502b730-c9a0-40ff-83bd-63eb249f3771" />
<img width="320" height="126" alt="image" src="https://github.com/user-attachments/assets/ab257fc5-036d-4e1f-a632-70242188aef7" />

### Shake Effect

<table>
<tr>
<th>Shake</th>
<th></th>
<th>Examples</th>
</tr>
<tr>
<td>Example one</td>
<td></td>
<td><code>&lt;shake(2,20) This text shakes!&gt;</code></td>
</tr>
<tr>
<td>Example two</td>
<td></td>
<td><code>&lt;shake(5,30) Intense shaking&gt;</code></td>
</tr>
<img width="402" height="155" alt="image" src="https://github.com/user-attachments/assets/9279cc23-df3b-4517-a5d2-3d838ae71847" />
</table>

![gif](https://github.com/user-attachments/assets/1fb1eaeb-0287-4470-ba66-50da1936da72)

- #### First number: intensity (how far characters move)
- #### Second number: speed (how fast they shake)

### Delay

<table>
<tr>
<th>Delay</th>
<th></th>
<th>Examples</th>
</tr>
<tr>
<td>Example</td>
<td></td>
<td><code>&lt;delay(0.5) Wait for 0.5 seconds&gt;</code></td>
</tr>
</table>

<img width="406" height="164" alt="image" src="https://github.com/user-attachments/assets/d0a71fa5-2ae3-4ca5-bca1-7c587ab08ce8" />

- #### Adds a pause before the text appears

### Combining Effects

<table>
<tr>
<th>Shake</th>
<th></th>
<th>Examples</th>
</tr>
<tr>
<td>Example one</td>
<td></td>
<td><code>&lt;highlight(red) shake(3,25) DANGER AHEAD!&gt;</code></td>
</tr>
<tr>
<td>Example two</td>
<td></td>
<td><code>&lt;highlight(yellow) delay(1) Here's a hint...&gt;</code></td>
</tr>
<img width="402" height="155" alt="image" src="https://github.com/user-attachments/assets/9279cc23-df3b-4517-a5d2-3d838ae71847" />
</table>

<img width="404" height="150" alt="image" src="https://github.com/user-attachments/assets/51dd5099-6e24-48e8-809b-0a9c45aee5e6" />

- The order of the tags doesn't matter


### Using Flags (Conditions)
Flags let you control which dialogue and options appear based on player progress.

- Conditions are optional and are used for specific interactions

Current working flags are "Has[ItemName] 

### Example: HasRevolver

#### Dialogue Tree Example:

<img width="402" height="111" alt="image" src="https://github.com/user-attachments/assets/d6f2a654-a7f9-485d-8174-064511577cab" />

#### Player Option Example:

<img width="381" height="223" alt="image" src="https://github.com/user-attachments/assets/538b5b2c-c7e0-407c-be7c-827561b7b3b4" />

### Negative Flags (NOT condition)

Use ! prefix to check if a flag does NOT exist:




#### Dialogue Tree Example:

<img width="398" height="121" alt="image" src="https://github.com/user-attachments/assets/1cf4a07c-7e31-4ea3-bee5-ea79c1da4fa1" />

#### Player Option Example:

<img width="396" height="235" alt="image" src="https://github.com/user-attachments/assets/7447aabd-8a01-44a7-817e-126f244d922b" />

## Available Items

<table> <tr><th>Item Available</th></tr> <tr><td>Sodacan</td></tr> <tr><td>Battery</td></tr> <tr><td>Ammo</td></tr> <tr><td>Fencekey</td></tr> <tr><td>Revolver</td></tr> <tr><td>Pistol</td></tr> </table>

## Creating Player Choices

### Basic Options

- In your DialogueNode, expand the Options list and add choices:

- Click the + button to add an option
- Fill in Option Text: What the player sees as a choice
- Assign Next Dialogue: The DialogueTree that plays when chosen (leave empty to end conversation)

<img width="405" height="121" alt="image" src="https://github.com/user-attachments/assets/42ba1874-0592-4fa6-ac21-59021c672149" />
<img width="382" height="458" alt="image" src="https://github.com/user-attachments/assets/7435f207-2ccd-4878-b45a-5b2ae416b270" />
<img width="779" height="163" alt="image" src="https://github.com/user-attachments/assets/46bef0fb-2368-4013-9d8b-59360cc3691e" />


## Dialogue Action
#### Action like flags are optional and doesn't need to be added

<p>Actions let dialogue trigger gameplay events. In any DialogueOption, expand <strong>Actions</strong> and add actions:</p>

<table>
<tr>
<th>Action Type</th>
<th>Description</th>
<th>Required Fields</th>
</tr>
<tr>
<td>Give Item / Remove Item</td>
<td>Give or remove items from player inventory</td>
<td><strong>Item</strong> (ItemData reference)<br><strong>Item Quantity</strong></td>
</tr>
<tr>
<td>Teleport Player</td>
<td>Moves player to a specific location</td>
<td><strong>Teleport Location</strong> (Transform in scene)</td>
</tr>
<tr>
<td>Play Sound</td>
<td>Plays an audio clip</td>
<td><strong>Sound To Play</strong> (AudioClip)</td>
</tr>
<tr>
<td>Start Quest / Complete Quest</td>
<td>Integrates with quest system (if you have one)</td>
<td><strong>Quest Id</strong> (string identifier)</td>
</tr>
<tr>
<td>Spawn Object</td>
<td>Instantiates a GameObject</td>
<td><strong>Target Object</strong> (prefab)<br><strong>Spawn Location</strong> (Transform)</td>
</tr>
<tr>
<td>Destroy Object / Enable Object / Disable Object</td>
<td>Removes or toggles GameObjects in scene</td>
<td><strong>Target Object</strong> (GameObject reference)</td>
</tr>
<tr>
<td>Load Scene</td>
<td>Loads a different Unity scene</td>
<td><strong>Scene Name</strong> (string)</td>
</tr>
<tr>
<td>Custom</td>
<td>Triggers a UnityEvent you define, it requires you to make a script for it to work</td>
<td><strong>Custom Action</strong> (configure with any methods).</td>
</tr>
</table>

<img width="325" height="320" alt="image" src="https://github.com/user-attachments/assets/7700047a-dada-4475-8beb-e249ea646204" />

## Tutorials for some actions

## Give/Remove Item Action

### Requirements for it to work:

- Item Data
- Quantity (optional)

####  Item Data is a scriptable object and can be created the same way as dialogue tree

<img width="440" height="100" alt="image" src="https://github.com/user-attachments/assets/6510303d-e49f-4752-bfc8-d7862da9af00" />

<img width="331" height="195" alt="image" src="https://github.com/user-attachments/assets/6206d12b-adab-48c7-a9ee-59be6a9c6abd" />

## Teleport Player

### Requirements for it to work:

- Transform (an object to where the player is teleported

<img width="329" height="174" alt="image" src="https://github.com/user-attachments/assets/ef043e78-fb44-4ba5-b9dc-9f00908c6266" />


## Play Sound

### Requirements for it to work:

- Audio Clip (sound)

<img width="321" height="149" alt="image" src="https://github.com/user-attachments/assets/571cfd12-46c3-40ec-bdfc-287ac0f26bc6" />

## Start Objective

### Requirements for it to work: 

- Objective Name
- Objective Type

### Objective Types

#### Boolean
Boolean objectives are like for example: talk to someone, it will stay false until it's  true

#### Count
Count objectives are like for example: Kill certain enemy 0/10

#### Collective
Collective objectives are like for example: Collect these items.

<img width="340" height="229" alt="image" src="https://github.com/user-attachments/assets/73553ec4-672c-4063-aecb-9b66abcc7bb9" />


## Progress Objective

### Requirements for it to work:

- Objective name
- Amount to progress

#### If objective doesn't exist when it's called then it won't do anything.

#### It will also complete boolean objectives

<img width="318" height="194" alt="image" src="https://github.com/user-attachments/assets/0bbc81de-34fa-4863-9cc7-55eefcb0dae0" />


## Complete Objective

### Requirements for it to work:

- Objective name

#### It will auto complete any objective.

<img width="312" height="157" alt="image" src="https://github.com/user-attachments/assets/d118d221-7fc5-446c-8a26-8f34daebcbbe" />


## Spawn Object

### Requirements for it to work:

- Gameobject
- Transform

#### Transform is for position and won't do anything if not assigned.

<img width="330" height="183" alt="image" src="https://github.com/user-attachments/assets/4cf6ff99-6ec9-4169-8afa-9ad7b77c81f1" />


## Destroy Object

### Requirements for it to work:

- Gameobject


#### It will destroy any gameobject assigned without fail.

<img width="323" height="178" alt="image" src="https://github.com/user-attachments/assets/fdf06da7-0d32-4328-8a7c-fbc3a9c58e2e" />

## Enable Object

### Requirements for it to work:

- Gameobject

#### It will enable any gameobject assigned without fail. 

<img width="326" height="185" alt="image" src="https://github.com/user-attachments/assets/97997ec5-000b-493a-a766-7acda1aa20f7" />

## Disable Object

### Requirements for it to work:

- Gameobject

#### It will disable any gameobject assigned without fail. 


<img width="322" height="190" alt="image" src="https://github.com/user-attachments/assets/c3537835-707f-467b-a5dd-53213813019f" />


## Load Scene

### Requirements for it to work:

- Scene Name (string)

  #### It will load a new unity scene, name is needed. To Check Name: File > Build Settings and pick any scene to load

<img width="327" height="196" alt="image" src="https://github.com/user-attachments/assets/238e7f93-527b-44c1-9cca-368ef0ee523d" />



## Custom Action 

```csharp
public class CustomAction : MonoBehaviour
{
    void KillPlayer()
    {
        // Kill Player logic here
    }
}
```












