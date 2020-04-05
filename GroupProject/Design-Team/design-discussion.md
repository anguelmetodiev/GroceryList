
# Section A (INDIVIDUAL DESIGNS):

# Design 1 (Joseph Soloman)

![JosephSaloman-design img](/GroupProject/Design-Individual/JosephSalomon/design.JPG)

## Pros:
	Simple enough to redesign
	Simple (J.A)
	Easy to implement and make changes/additions where necessary (CHRIS)
	Adding and editing can be done easily if needed (A.M)



## Cons:
    Did not finish relationship types (aka one to many...)
    Does not show access to database
    Does not have user class
    Relations aren't represented properly. No accessible classes (J.A)
    Users needed - users need to be able to have a one-to-many relationship with their grocery lists (CHRIS)
	Lack of user class and 1-to-MANY relations (A.M)

# Design 2 (Christopher Shepherd)

![ChristopherLShepherd-design img](/GroupProject/Design-Individual/ChristopherLShepherd/design.JPG)

## Pros:
    Very thorough in search, Everything has a functionality and purpose
    Thorough, covered all requirements (J.A)
	Easy search, user class and relations implemented well (A.M)

## Cons:
    Must go through Item Type to access items (cant directly look for items), Too many functions
    Some of the functions should be moved into accesible classes (J.A)
	More than needed functions. (A.M)

# Design 3 (Joseph Almonte)

![JAlmonte95-design img](/GroupProject/Design-Individual/jalmonte95/design.JPG)

## Pros:
    Proper way to represent connections.
    Everything is represented correctly - this is probably how an actual
    developer would design this project. (CHRIS)
	Excellent design representation. (A.M)

## Cons:
    Looks like user searches for items when not in a specified list. (user should be in specified list when searching for items to add)
    Possibly difficult to execute
    Not sure how the search would work out - search for itemName and then
    itemType? I think this could be represented with a SEARCH connection that splits
    (either itemName search or itemType search) and then joins back together for a
    single Item. (CHRIS)
	Search can be implemented in a better way by ItemName and ItemType. (A.M)

# Design 3 (Joey Cheung)

![JoeyCheung-design img](/GroupProject/Design-Individual/Joey%20Cheung/design.JPG)

## Pros:
    Simple
    Easy to traverse through
    Simple(J.A)
    Easy to implement and make changes/additions where necessary (CHRIS)
	Well organized and simple, easy to modify (A.M)

## Cons:
    No ability to create a new item.
    Quantity can just be an instance variable, doesnt need to be individual class
    Relations are not shown, there are no accesible classes or heirarchal display for items(J.A)
    I would keep the actual list of ALL items to choose from as a separate
    object instead of an ArrayList inside the personal List class. (CHRIS)
	Relationships one to many are not displayed. (A.M)


# Design 3 (Anguel Metodiev)

![AnguelMetodiev-design img](/GroupProject/Design-Individual/anguelmetodiev/design.JPG)

## Pros:
    Everything has a manager so easy to add, delete, etc.
    Everything is neat
    Well done, everything looks properly represented (J.A.)
    Easy to understand conceptually. (CHRIS)
	Mapped well and easy to follow. (A.M)

## Cons:
    Not able to search item without going through itemType
    Also no user class
    A relationship between itemManager and itemType/item should exist (J.A.)
    ^^Agreed. Right now the relationship is between the List and ItemType,
    and so the ItemType and Item classes have no connection to the GLDatabase
    to choose items. Also, should add a user class since they can have more
    than one lists. (CHRIS)I absolutely agree with you. Lacking the connection to the GLDatabase (A.M)

# Section B (TEAM DESIGN):

![Team-design img](/GroupProject/Design-Team/Images/design.JPG)

## Joseph Almonte's comparison:

The similarities between my design and the team's are the User, item, and groceryList classes.

The main difference is that there are no accesible classes, the team decided to add functions to several classes in order to condense the UML design as opposed to my design which has several accesible classes that act as functions. We decided to do this because we thought it would make more sense for the functions to be placed within the classes that would be using it. Also, in the team's design the relations are better represented.

I feel as though the team decided to use the submitted design as opposed to mine because it covered all the necessary requirements for the UML/app design and was better condensed, making it simpler for everyone to read and understand what is happening within the app.


## Joseph Salomon comparison:

The similarities with my design and the groups design is the way that everything interacts.

However it is very different becuase in my design it  was not specific enough with how everything interacts with eachother and the relationship with other classes. (one to many or many to many etc...)

The groups design is better to use becuase it is more clear than my design. The groups model defines each relationship as opposed to mine which are just lines. This allows the design to be more understandable and be easily readable for everyone.


## Christopher Shepherd's comparison:

My design's basic structure was chosen to be represented as the Team's UML design for this project, and so there aren't too many differences.
The main issues that came up during the discussion regarding my original design was the inability for classes to access functions in other classes because I made them private. The other issue was the fact that I included way more functions than I needed to.
Upon discussion with the rest of the team, I found that I ended up including "Nice-to-have" functionality for this app, that aren't necessary at all. Including these "Nice-to-have" functions at this preliminary design stage of our project can create more unnecessary work down the road for the whole team. We decided to restrict the functionality to only what is absolutely crucial according to the requirements stated by Brad and Janet.
As for inaccessible functions between classes, we decided to just make most of the operations public to allow variability of operations between classes.


## Anguel Metodiev comparison:

Comparing the team design to my design, I have noticed the following:
My design has a class List allows user to create and manage all items,
implemented by a database, GLDataBase, ItemManager allows user to search,
create, delete items, items can be updated by the update methods conveniently matches item types with item.
However, the group design is better than mine because my design has some cons such as GroceryListManager and ItemManager can be merged to reduce repetition and smoother application
before user enters their inputs, GLDataBase could already have all possible data (items, types) stored. The group model compensates for the issues listed in my design.


## Joey Cheung comparison:

The similiarities between my design and the team's designs
We mostly had the same functionalities and were both able to traverse it fairly easily and wasn't too convoluted. Many functions and classes were similar as well so we had the same line of thinking when it came to this.
The differences between my design and the team's designs
My design was a lot more simple compared to everyone else's designs even though many of the other team members also had simple designs, my design was for sure the most simple. My design lacked in some functionality though as the team pointed out such as the inability to create a new item and the fact that I didn't need to make an a class for quantity and could have just made it into and instance variable instead.
My design overall lacked relationships but was simple and editable for the team's desired design however we chose to not use my design.


# Section C (SUMMARY):

As a group we learned how to communicate effectively and give constructive criticism without attacking and offending each other.
We also realized that it is best to work within teams when creating something like a UML design, a project that most of us are not too familiar with, because we can all realize eachother's mistakes in order to provide input and to build the best design possible. Many members missed certain aspects in their own individual UML design that others had which overall made it easier to decide that we would build off Chris' design because we felt as if his design was the most complete and there were only a few aspects to edit from it.
We also learned that everyone may not operate on the same schedule and timing but as long as we communicate in some form the work will be done and all members are willing to contribute.
