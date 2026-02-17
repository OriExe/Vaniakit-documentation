#PlayerController Class

The PlayerController holds important data used by other player scripts and controls the player healthbar.

- health data
- player [Rigidbody2D](https://docs.unity3d.com/ScriptReference/Rigidbody2D.html)
## Events
#### `onPlayerHit(int damageTaken)`
Triggers when the player takes damage from an enemy
#### `onPlayerHitCritical(int damageTaken)`
Triggers when the player takes damage from a trap and therefore requires them to teleport to another location. (by default it does not do that but the functionally can be added using the <span style="color: red;"> Vaniakit.Generic.TeleportToNearestCheckpoint class [Missing Link]</span>)
#### `onPlayerInteractedWithObject(string nameOfObject)`
Triggers when the player interacts with a gameobject that has an IInteractable interface. Includes the name of the type of object they interacted with as `nameOfObject` such as interacted with `itemPickup`.
## Accessible Variables (In Code)
#### `int currentHealth` 
Access and modify the currentHealth of the player during game.
#### `delegate onPlayerDead` (Should be changed)
Is called when the player dies in game, Can be added onto any script using 

    Vaniakit.Player.PlayerController.onPlayerDead+=yourMethod() //Vaniakit.player can be removed if already referenced in your script 

## Accessible Variables (In Unity Editor)

#### `Rigidbody2D rb`
The main ridigbody for the player that can be accessed from any script by running
    
     Vaniakit.Player.PlayerController.getPlayerRigidbody() //Vaniakit.player can be removed if already referenced in your script 


#### `int startingHealth`
Amount of health player starts with, only affects the start of the game and doesn't change player's health after that unless you restart the game.
