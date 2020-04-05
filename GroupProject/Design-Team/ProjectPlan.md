# Project Plan

**Author**: Team 5

## 1 Introduction

We are developing an Android app that manages grocery lists for a user. You should be able to search for different items grouped by Item Type, and add them to your personal list. You can also have more than one grocery list in your app.

## 2 Process Description

## *Main Activity*
*This is the main view that will be seen from all users. We will call this as the menu activity which will allow users to create multiple lists. Users can also perform operaions such as check the list, delete list, create list, rename list. The users can also view the items to add to the list.

- *Entrance criteria - This is the main activity, opening the app will direct users to this view.*

## Create List Activity
*This is the activity where users are allowed to create new lists based on their requirements.

There are three types of data required in order to make a successful item on the list. The **ItemType**, **ItemName**, and the **Quantity** of the items. The user needs at least one item to create a successful new list. Furthermore, in this activity, the user can also view a list of items and the user can pick and add items to a list by picking them from a hierarchical list, where the first level is the item type (e.g., fruit), and the second level is the name of the actual item.*

## Check your List Activity
*This activity is a view that displays the user the lists that have been created previously. All the names will be shown in a list view activity and each of the lists can be viewed separately. Once a list have been clicked, a user can view the list and the items. *

## Choosen List Activity
*This view is accessed through every list that have been created by the user. The user can view all of the items of the selected list.
Once the user is in the choosen List, Item Activity, the user can  finalize their items. The user can either go back and modify the items, or select the items in the list and delete them permenently if necessary. In this case, the user can also hide checkOff items and the visibility will be set to hidden. This activity will also allow the user to checkout the items in the list. This will save the items in the list directly to the database, and will alert the user after a succesful save with a confirmation message.*

## View Selected Activity
*This view is another list view of selected lists as the user may want to view concurrently. Saved lists in the database can be selected beforehand and items in the particular list can be viewed in this view selected activity *

## Delete List Activity
*This activity allows users to click on a particular list and delete straight away if necessary. *


## Update Item Activity
*A list view that shows users the changes that have been made to the previously created list.
 The user in this activity can see the items in a list. And the users can then update list products like they were in new List Activity. This activyty will allow users to add the product to an existing list, remove a product in the existing list, or modify the quantity of the items in the list at any time. *


## 3 Team
<!--

- *Team members' names*
- *Roles, with a short description of each role*
- *Table showing which team member(s) has which role(s)*
-->
Team 5 Structure
- Project Manager: Keeps processes of the overall project moving along; keeps team informed of deadlines and requirements.
- Coder: Responsible more for the code side of this project; ensures that the apps functionality works correctly.
- Documenter: Responsible for keeping track of progress by documenting information at every stage of the project to stay organized.

|Team Member | Project Manager | Coder | Documenter |
|---|---|---|---|
| Joseph Almonte | x | x | x |
| Joey Cheung |   | x | x |
| Anguel Metodiev |   | x | x |
| Joseph Salomon |   | x | x |
| Christopher Shepherd |   | x | x |
