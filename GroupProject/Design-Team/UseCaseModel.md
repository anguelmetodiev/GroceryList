# Use Case Model

**Author**: \<Team 5\>

## 1 Use Case Diagram


![UseCaseDiagram-img](/GroupProject/Design-Team/Images/GroceryListApp_UseCaseDiagram.jpeg)

## 2 Use Case Descriptions

Add an item: This case must allow a user to add an item to a given grocery list to keep track of it. The precondition is that there must be a grocery list already created to be able to add the item to. The post condition is to save the item to the grocery list and properly display it in the correct grocery list and type. The way to achieve this would be to choose a grocery list from the main screen, hit the ‘Add’ button and go through the item type search (and optionally the item name search) if the user finds the item they will select it and it will be added to their list.

Rename List: This case must allow a user to rename an already existing item list. The precondition is that there are already created grocery list(s). The post condition is to update the grocery list with the new name and display the new name. The way to achieve this would be to hold down on the grocery list, then the user can edit the list or delete, once they decide to edit and then do so the updated name should save to the db.

Delete List: This case must allow a user to delete an already existing item list. The precondition is that there are already created grocery list(s). The post condition is to delete that list and all item present in it. The way to achieve this would be to hold down on a grocery list choose  the ‘Delete’ option on the gui and confirm the choice.

Add List: This case must allow a user to add a non existing grocery list. The precondition is that there are no previously created lists with the same name. The post condition is to to have no duplicated lists and a new list. The way to achieve this would be to choose hit the ‘Add’ button on the main screen and type in a name for your new grocery list, the user can then save.

Remove Item: This case must allow a user to remove an item from a given grocery list. The precondition is that there must be a grocery list already created and at least one item on the list. The post condition is to remove the item and not display it in the home screen of lists. The way to achieve this would be to choose a grocery list and from the main screen, once the user is looking at the contents within the list, he can check the checkbox next to the item he/she wants to delete and click the 'trash can' icon at the top of the screen.

Item Search: This case must allow a user to search for an item from the database. The precondition is that there must be a database to extract the data from. The post condition is to search the item and see if it's in the database or not. The way to achieve this would be to enter a grocery list and then choose to add an item to that list. The user will then navigate through the item type search selection and optionally the item name search to find an item.

Type Search: This case must allow a user to search an item type from the database. The precondition is that there must be a database to extract the data from. The post condition is to search the item type and see if it's in the database or not. The way to achieve this would be to enter a grocery list and then choose to add an item to that list. The user will then begin searching for an item by type.

Select Quantity: This case must allow a select a quantity when adding an item. The precondition is that the user has gone through all the steps to add an item and then get up to the screen where the user can select a quantity for the item. The post condition is to select a quantity for the item. The way to achieve this would be to choose add an item to the grocery list and once they are at the screen that prompts the user to give a quantity, they would type in a quantity.

Check Off Box: This case must allow a user to check/uncheck off items. The precondition is that there must be an existing item in a grocery list. The post condition is to check/uncheck the item off and change its boolean value to true or false, depending on what it was previously. The way to achieve this would be to choose an item from the grocery list screen and then check or uncheck a box.

Add Item To Database: This case must allow users to add items to the database. The precondition is that the users must have tried to add an item to the grocery list and expensed both search options. The post condition is that the item is now apart of the database and the user's list. The way to achieve this would be to already have a list created and now the user is trying to add items to the list. While they are attempting to add an item, they exhausted both search options and did not find the item so they are now adding it to the database. They will insert an item name and select an item type, then hit add and the item will be added to our database and to the user's list.
