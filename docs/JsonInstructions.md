# Json Instructions class
Saves and loads Json files in the game. 
## Accessible Methods
#### `loadJsonArray<T>(string nameOfFile, out T ArrayThatLoaded)`
Loads the select Json file of said name and type passed through the function based on the current value of `filePath`. Outputs the result as `ArrayThatLoaded`
#### `SaveAsJsonArray<T>(T ArrayToSave, string nameOfFile)` 
Saves the Json file of class type <T\>(T meaning can be anything like`FastTravelPoints`) and saves as the specific name in set `filePath`
## Accessible Values 
#### `string filePath`
Included in both methods locally and sets the location to load and save the file. Default is set to [`Application.persistentDataPath`](https://docs.unity3d.com/6000.3/Documentation/ScriptReference/Application-persistentDataPath.html) + the name of the file.