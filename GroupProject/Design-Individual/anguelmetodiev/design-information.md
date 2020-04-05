1. A grocery list consists of items the users want to buy at a grocery store.
The application must allow users to add items to a list, delete items from a list,
and change the quantity of items in the list (e.g., change from one to two pounds of apples).

List class holds all items and has ability to create them.
addItem() adds items already in GLDataBase into lists.
removeItem() removes items from lists, but this does not affect the GLDataBase.
updateItemQuantity() updates # of items in lists.


---------------

2. The application must contain a database (DB) of items and corresponding item types.

GLDataBase is the application database that holds items, lists, item types.


---------------

3. Users must be able to add items to a list by picking them from a hierarchical list, where
the first level is the item type (e.g., cereal), and the second level is the name of the 
actual item (e.g., shredded wheat).
After adding an item, users must be able to specify a quantity for that item.

All instances of Item inherit a type from their parent ItemType and hold a name.
When users use AddItem() within their lists, they're asked to choose how they want to look for the items
they want to add to their lists from database.
Options include: searching through item type, or through item name.
Both options would access application database.
When users choose to add an item to their lists through item type, they are shown a list of item types.
After they choose the desired item type, they are shown all the items of that type that are stored in the
application database.
Once an item is added to a list, updateItemQuantity() is called, and users must provide a quantity
for items they're adding in their lists.


---------------

4. Users must also be able to specify an item by typing its name. In this case, the
application must look in its DB for items with similar names and ask the users, for each
of them, whether that is the item they intended to add. If a match cannot be found, the
application must ask the user to select a type for the item and then save the new item,
together with its type, in its DB.

All of Item's instances inherit a type from their parent ItemType and hold a name.
When users use AddItem() within their lists, they are prompted to choose how they want to look for the items
they intend to add to their lists from the database.
The options: search through item type or through item name.
Both options access the application database.
When users choose option to add an item to their lists through name, a search field appears on the screen asking the
users for a String input.
After typing and confirming the item's name which the users are looking for, their lists access
the database (via ItemManager), that is responsible to look for items that are stored in the database that
have similar names to what the users have typed as input in the search field.
This is made possible by searchItem() in ItemManager.
The users are then shown a list of results, or no results if ItemManager can't find any match for users' input in database.
In addition, an option to create a new item will show up at the screen's bottom.
If users choose one of the results shown on the screen, the selected item will be added to users' list.
Once an item is added to a list, updateItemQuantity() is called, and users must provide a quantity
for the item they are adding in their lists.
If no results are shown, or if users don't find what they're looking for among results, they'll have the
option to create a new item at the screen's bottom, as previously mentioned.
When users choose option of creating new product, createItem() in ItemManager is called.
So the users will be asked to provide a type and name for whichever product they want stored in the database.
Once the new item is added to a list, the updateItemQuantity() is called, and users must choose a quantity
for the item they're adding in their lists.


---------------

5. Lists must be saved automatically and immediately after they are modified.

Every time anything is modified in a list, GroceryListManager saves the modifications in the GLDataBase using the
function updateList(i:List).


---------------

6. Users must be able to check off items in a list (without deleting them).

Each Item object has checkBox, with is a boolean attribute.
checkBox can be switched from false to true, or true to false from checkItem().
When checkItem() is called in an Item object, checkBox is set to true if it's false, or set to false if it's true.
This allows for users to freely check/uncheck the items in their lists whenever they want.


---------------

7. Users must also be able to clear all the check-off marks in a list at once.

clearAllCheckItem() is in every List object. This function scrolls through all items it is keeping tracking of,
and sets their checkBox to false.


---------------

8. Check-off marks for a list are persistent and must also be saved immediately.

GroceryListManager saves any changes in GLDataBase using updateList(i:List) whenever something is changed in a list
(this includes when the checkBox is set from one state to another one).


---------------

9. The application must present the items in a list grouped by type, so as to allow users to
shop for a specific type of products at once (i.e., without having to go back and forth between aisles).

arrangeList() is called each time an Item object is added to a List object. arrangeList() sorts them in alphabetical order.
Items of type grains would come before items of type meat.
Same type items would also be in alphabetical order.
This means in the group of items of type meat, the item "bacon" comes before item "chicken".


---------------

10. The application must support multiple lists at a time (e.g., “weekly grocery list”, “monthly
farmer’s market list”). Therefore, the application must provide the users with the ability to
create, (re)name, select, and delete lists.

GroceryListManager has functions that create and can change type List objects.
createList() creates new lists. Before they are saved in GLDataBase, users can choose names for them.
deleteList() deletes lists from GLDataBase.
nameList() names and/or renames type List objects.
selectList() lets you select which lists to open out of all created.


---------------

11. The User Interface (UI) must be intuitive and responsive.
Doesn't affect design so not considered.