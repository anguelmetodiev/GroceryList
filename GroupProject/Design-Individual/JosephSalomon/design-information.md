1. A grocery list consists of items the users want to buy at a grocery store. The application must allow users to add items to a list, delete items from a list, and change the quantity of items in the list (e.g., change from one to two pounds of apples).

        Included is a class List which allows users to add, delete and change quantities 

2. The application must contain a database (DB) of ​items​ and corresponding ​item types​.

        DB is not neccesary for the diagram

3. Users must be able to add items to a list by picking them from a hierarchical list, where the first level is the item type (e.g., cereal), and the second level is the name of the actual item (e.g., shredded wheat). After adding an item, users must be able to specify a quantity for that item.

        Included is a class that goes to the type and only after can you find items of that type, when you add the type to the list you will include the amount (done when you implement)

4. Users must also be able to specify an item by typing its name. In this case, the application must look in its DB for items with similar names and ask the users, for each of them, whether that is the item they intended to add. If a match cannot be found, the application must ask the user to select a type for the item and then save the new item, together with its type, in its DB.

        In the class list there is a method to search for an item directly that will allow you to have this function when implemented

5. Lists must be saved automatically and immediately after they are modified.

        Not neccesary for the diagram

6. Users must be able to check off items in a list (without deleting them).

        Method in class List to check individual items

7. Users must also be able to clear all the check-off marks in a list at once.

        method in class List to uncheck all checked off items

8. Check-off marks for a list are persistent and must also be saved immediately.

        Not neccesary for the diagram

9. The application must present the items in a list grouped by type, so as to allow users to
shop for a specific type of products at once (i.e., without having to go back and forth
between aisles).

        Not neccesary for the diagram

10. The application must support multiple lists at a time (e.g., “weekly grocery list”, “monthly
farmer’s market list”). Therefore, the application must provide the users with the ability to
create, (re)name, select, and delete lists.

        Class manager allows you to create, rename, select and delete lists. 

11. The User Interface (UI) must be intuitive and responsive.

