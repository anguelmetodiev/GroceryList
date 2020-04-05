Christopher Shepherd

1. A grocery list consists of items the users want to buy at a grocery store. The application must allow users to add items to a list, delete items from a list, and change the quantity of items in the list (e.g., change from one to two pounds of apples).
  - There exists a user class to represent a user, an availableItemsList class that acts as the grocery store's database of items and itemTypes, as well a groceryList class that the user can add items to.
2. The application must contain a database (DB) of ​items​ and corresponding ​item types​.
  - This design contains a class called availableItemsList that contains many items that are categorized by their corresponding itemType. Users will be able to filter for itemTypes or a particular item specifically.
3. Users must be able to add items to a list by picking them from a hierarchical list, where the first level is the item type (e.g., cereal), and the second level is the name of the actual item (e.g., shredded wheat). After adding an item, users must be able to specify a quantity for that item.
  - The user class contains many useful functions. Some of which include search, searchType, and searchItem. The search function allows a user to access and simply browse through a grocery's availableItemsList to select items, which will be sorted by their itemTypes. The function searchType allows a user to filter the complete list to only show items with a certain type. The searchItem function allows a user to enter a specific item name to search for. At this point, the user can simply add that single item to their groceryList.
4. Users must also be able to specify an item by typing its name. In this case, the application must look in its DB for items with similar names and ask the users, for each of them, whether that is the item they intended to add. If a match cannot be found, the application must ask the user to select a type for the item and then save the new item, together with its type, in its DB.
  - As stated in previous requirement info, the user class contains addToList, search, searchType, and searchItem, all of which allow the user to type in and search for an item or an itemType. If an item doesn't exist, the availableItemsList can run a function to request for a new item to be added, and ask for the user to give the new item an itemType as well.
5. Lists must be saved automatically and immediately after they are modified.
  - The groceryList class has an autosave attribute that is boolean (basically is autosave ON or OFF). If on, the list will save after every change, otherwise the user will have to run the saveList function to manually save their groceryList.
6. Users must be able to check off items in a list (without deleting them).
  - The itemsAdded class (items that are added to a groceryList) has a boolean attribute called selected, where an itemAdded can be selected or unselected (useful for deleting multiple items from a groceryList).
7. Users must also be able to clear all the check-off marks in a list at once.
  - The user class contains a checkOff function (to check off an item) as well as a clearChecked function that will remove the checked-off items from the user's groceryList.
8. Check-off marks for a list are persistent and must also be saved immediately.
  - AUTOSAVE function for the list can be set to ENABLED.
9. The application must present the items in a list grouped by type, so as to allow users to
shop for a specific type of products at once (i.e., without having to go back and forth
between aisles).
  - As stated under the search function description for requirement 3, the user will be able to simply browse through the availableItemsList, which is sorted by itemTypes.
10. The application must support multiple lists at a time (e.g., “weekly grocery list”, “monthly farmer’s market list”). Therefore, the application must provide the users with the ability to create, (re)name, select, and delete lists.
  - The user class has a "one-to-many" relationship with the groceryList class, meaning they can have multiple groceryLists. The newGroceryList function allows them to create a new list with a user-inputted name. The removeGroceryList function allows a user to remove a groceryList. The renameList function allows a user to rename a groceryList that already exists.
11. The User Interface (UI) must be intuitive and responsive.
  - UI not yet designed.
