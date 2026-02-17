# Fast Travel System class
A small class that teleports you from one point to another. Relies on the [Manager class](Managers.md) 
## Accessible Variables

#### `string fileNameForFTSystem` 
A value that deterines the name of the json file that stores all the fast travel points in your game. Can be modified only within the class. Default value is `VaniaKitFastTravelPoints.json`

#### `public static List<FastTravelData> allPoints;`
A list containing all the fastTravelPoints in the game. Uses the managers class to request this info

#### Accessible Methods
#### `teleportToPoint(FastTravelData point)`
Teleports the player to the point included the parameter when triggered. Goes well with the `allPoints` list