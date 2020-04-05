# Design Document

**Author**: \<Team 5>

## 1 Design Considerations


### 1.1 Assumptions


Assumption: We will make use of a database to store the list of categorized items

Background: We are developing an Android app that manages grocery lists for a user. You should be able to search for different items grouped by Item Type, and add them to your personal list. You can also have more than one grocery list in your app.

Dependecies: Will rely on the database of items

Use: Allows users to store a grocery list and check off items, thus making it easier and more convenient for them to go grocery store shopping

Operational Environment: Phone application

Other Issues: We are not sure yet

### 1.2 Constraints

The app will not be compatible on some older phones that are running a dated android software

### 1.3 System Environment

Any smartphone running android sofware with an API of 24 or above

## 2 Architectural Design

### 2.1 Component Diagram

![ComponentDiagram img](/GroupProject/Design-Team/Images/370componentDiagram.jpeg)

Our project should consist of three main components:
- The initial "Search" page, which can direct the user to the ItemDatabase component, or the ListManagement component.
- The ItemDatabase component will consist of the entire list of available items that the user can add to their grocery list. In this component, items can also be added when necessary, and chosen to add to the third component of this project.
- The ListManagement component allows the user to manage the items that they've added to their list. They can also manage their lists, since they are allowed to have more than one particular grocery list (they will be able to remove, add, and rename lists).

### 2.2 Deployment Diagram

## 3 Low-Level Design

### 3.1 Class Diagram

![Team-design img](/GroupProject/Design-Team/Images/design.JPG)

### 3.2 Other Diagrams

## 4 User Interface Design
![UIDiagram img](/GroupProject/Design-Team/Images/UIDiagram.jpg)
