# InventorySlot Struct
![](Images/InventorySlot.png)
A structure that defines an inventory item like a sword or currency

## Variables
#### `public ItemObject item`
(More details in the ItemObjects page)
#### `private int amountOfItem`
#### `public bool spawnAtStart`
will spawn this object at the start of the game if it has an IEquipable interface and is set to true

## Accessible Methods

#### `public void AddAmount(int amount)`
Add more of this item when called for example 
`coin.AddAmount(5)`
#### `public void SetScriptInGame(IEquipable script)`
Adds the script that allows the item to be used
#### `public IEquipable GetItemScriptInGame()`
Lets you access the script that allows the item to be used and therefore equip said item using the `equip() method`