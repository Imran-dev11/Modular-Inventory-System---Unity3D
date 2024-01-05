# Modular-Inventory-System---Unity3D
An Inventory System that can be integrated to any unity game.


Follow the Steps To Integrate this system to your project:

1- Import "InventorySystem.unitypackage" to your unity project.
2- Run the demo scene "" to confirm the things are working perfectly.
3- From Demo Scene, Copy the 'InventoryPanel' from canvas to your Game Scene Canvas.
4- From Demo Scene, Copy the 'InventoryManager' to your scene.
5- Find and open the 'InventoryItemData' script and modify or extend the 'ItemGroup' & 'ItemType' Enum values.
   'ItemGroup' should contain all the possible categories your Inventory Items can be divided to.
   'ItemType' is used to achieve the required purpose for an item.Or What action will be performed on Using an item from Inventory.
    For Example an item 'Apple' defined as a 'Food' ItemType. And in InventoryManager we have written the functionality of Food item type 
    to increase the player's health. You can create your new item type and can define its purpose in the "InventoryManager" script.
6- Now Create your InventoryDatabase. Assets -> Create -> ModularInventory -> New General Inventory
7- Add Item group elements to your inventory and add their required details. There should be a separate element for each "ItemGroup".
8- Now Create your Inventory Items. Assets -> Create -> ModularInventory -> New Inventory Item
    OR you can duplicate the already created Items in "InventoryItems" Folder, and alter the information
9- Now create a Pickup object for each inventory item by duplicating pickup prefabs in DemoScene. 
   Now assign the sprite, adjust the collider size and reference the InventoryItemData on 'PickupItem' Script.
   This Pickup object design will vary from game to game. In Demo, I have used 2D objects with collider.  
10-Now add 'PickUpsCollector' script to your player character, it will make your player pick an item as soon as it will collide to it.
   Note: If you are working on a 2D Game 'PickUpsCollector' will work fine but it will require rewriting for other types. 
         OR If you don't want to use colliders for interaction.
11-Now make sure that your 'InventoryManager' has the reference of your InventoryPanel and MyInventory Object.And your Player Character.
12-Play your game and now you should be able to pick the created item pickup. Open the inventory panel and use or drop the item. 
  
