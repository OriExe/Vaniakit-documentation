# Inventory Class
![alt text](Images/Inventory.png)

Manager script that manages the inventory for your player and should be added as a child to the main managers game object see info **[here](/Managers)** 

You don't need to make your own Inventory script that inherits from Inventory you can just use the main Inventory script already provided

**Note:This page will tell you what each element is showing [InventorySlot](/InventorySlot)**
## Accessible Methods

#### `static void addItemToInventory (InventorySlot itemToGive)`
Gives the select item to the player
#### `static List<InventorySlot> getAllItems()`
Returns all items that are in the player's inventory

