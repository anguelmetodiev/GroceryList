1. A grocery list consists of items the users want to buy at a grocery store. The application must allow users to add items to a list, delete items from a list, and change the quantity of items in the list (e.g., change from one to two pounds of apples).

To realize these requirements I created a groceryList class with association classes createList and deleteList which will respectively allow the user to create and delete a list. Under the groceryList class I added a changeQuantity() method to allow the user to change the quantity of the items in the list.

2. The application must contain a database (DB) of ​items​ and corresponding ​item types​.

To realize this requirement I created a class Item with attributes cost and expirationDate. There is a hierarchical list where the first level item is the itemType and then the itemName, where itemName has the attribute of brand. This creates the database of items and separates them by type so the user can search them, which is why we have a search relation between the user and itemName class.
    
3. Users must be able to add items to a list by picking them from a hierarchical list, where the first level is the item type (e.g., cereal), and the second level is the name of the actual item (e.g., shredded wheat). After adding an item, users must be able to specify a quantity for that item.

To realize these requirements, as mentioned previously,  I created a class Item with attributes cost and expirationDate. There is a hierarchical list where the first level item is the itemType and then the itemName, where itemName has the attribute of brand. There is a relationship between Item and groceryList that has the associated classes addItem which has a quantity, thus allowing users to add an item to a list and specify how many they'd want.

4. Users must also be able to specify an item by typing its name. In this case, the application must look in its DB for items with similar names and ask the users, for each of them, whether that is the item they intended to add. If a match cannot be found, the application must ask the user to select a type for the item and then save the new item, together with its type, in its DB.

5. Lists must be saved automatically and immediately after they are modified.

Under the groceryList class I created a method called autoSaveList(), which will save the list as it is modified

6. Users must be able to check off items in a list (without deleting them).

Under the groceryList class I created a method called checkOffItem() which will check off an item at the users request without deleting it

7. Users must also be able to clear all the check-off marks in a list at once.

Under the groceryList class I created a method called clearChecks(), which will clear all check-off marks in a list at once.

8. Check-off marks for a list are persistent and must also be saved immediately.

This will be handled by the autoSaveList(), the entire list, including it's checkmark states, will be saved automatically.

9. The application must present the items in a list grouped by type, so as to allow users toshop for a specific type of products at once (i.e., without having to go back and forth
between aisles).

Handle this by allowing users to search via item name and can also access them by itemType

10. The application must support multiple lists at a time (e.g., “weekly grocery list”, “monthlyfarmer’s market list”). Therefore, the application must provide the users with the ability tocreate, (re)name, select, and delete lists.

The groceryList class has the attributes listName and listType to allow for different lists. Also, the groceryList has the methods renameList(), selectList() which will allow the users to do what their respective names say. As well as the associated classes createList and deleteList which will respectively allow the user to create and delete lists.

11. The User Interface (UI) must be intuitive and responsive.

Created a utility class called User Interface, but not necessary for this UML.