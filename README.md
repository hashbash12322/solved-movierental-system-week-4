Download Link: https://assignmentchef.com/product/solved-movierental-system-week-4
<br>
Some of your methods need parameters. For example, to open a file you need to pass either the filename or account id (assumes that filename has the account id) so that the method knows which file to open.

You moved the attributes for media types into Media class now and that is still not correct. When the system runs, the UI would create an object of type media genre such as SciFi to represent the rental of that type/genre and then it would be stored in the list of objects in MediaRentalAccount.

You still have some classes show both aggregation and inheritance. The same two classes cannot have both inheritance relationship and composition/aggregation relationship All media class types/genre have inheritance relationships between each other.

Your inheritance notation is incorrect. Check the UML Basics document in week 1 under You Try for the correct notation.You are missing constructors in some classes. All classes need to show a constructor.

The mediaID attribute should be in Media and inherited. You do not need different attributes for an id across classes.

There should only be a single calculate method per class as you can only calculate rental fee based on the specifications.

To delete account and save to file you should not have parameters as they should so their actions on the currently opened file.

You do not need methods for rental type and genre in MediaRentalAccount.

To add media to the list in MediaRentalAccount you need to pass the media object that should be added.

To renew or return media, you need to pass the id of the media to do the action on since the account class will have a list of them stored.

You are missing cardinality for Person in the composition between MediaRentalAccount and Person.

You should not have method for rental type or to rent or renew media in Media class. Those actions are not done in Media but rather your account class.

You would not pass cost to the Media constructor as that value is calculated by the calculate method.

Some genre media classes need their own calculate methods. When the child class has different calculation than the parent, it needs its own calculation.

Your constructor for AudioBookCD should have all the attribute parameters to create the object or none and not just some of them. Same for MovieDVD and MusicCD.

Added/changed correctly the diagram to show polymorphism such as overriding an inherited method and overloading constructors

All the class attributes are private or protected appropriately to protect the integrity of the class’s data

The attributes have constructors or corresponding get/set methods as appropriate to access attributes. You must have a way to provide values to the attributes.

All methods have correct access modifiers (private, protected, or public)