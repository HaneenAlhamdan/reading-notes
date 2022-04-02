## interface 

An interface is defined as a syntactical contract that all the classes inheriting the interface should follow. The interface defines the 'what' part of the syntactical contract and the deriving classes define the 'how' part of the syntactical contract.
Interfaces define properties, methods, and events, which are the members of the interface. Interfaces contain only the declaration of the members. It is the responsibility of the deriving class to define the members. It often helps in providing a standard structure that the deriving classes would follow.
Abstract classes to some extent serve the same purpose, however, they are mostly used when only few methods are to be declared by the base class and the deriving class implements the functionalities.
Eample 1:-  

public interface ITransactions {
   // interface members
   void showTransaction();
   double getAmount();
}


Eample 2:-  

public void OpenBoot(); //and many other badly designed methods/properties, etc.
}

public interface IDrivable
{
void Drive();
}

....all we're doing here is using the language conttructs available to us in C# to declare to a consumer "look, the only thing I can guarantee about that IDrivable Car I gave you is that it has a Drive() method." - i.e the "Contract" aspect of an interface.
Now if there were some way to take your concrete implementation of Car and specify the contract inline on the actual class members , then that'd be just fine - but pointless unless you absolutely only ever needed a single concrete implementation of that behaviour, because otherwise you would need some way to share this definition of contract in a central place...bringing you right back to the interface keyword!

 interfaces for Unit testing is in some way an artificial and unnatural thing - in fact it's more natural to me if I have a class "GroceryShopper" and I want to test that it goes to the store and buys milk given a means of transport:
Surely a properly isolated unit test says "Drive that IDrivable thing I gave you to the store and get some milk" because we really only care about the milk, not the vehicle, as opposed to "Drive this Car to the store..." where we are now relying on having a working and callable Drive method that won't throw, etc...and even if you use a stub Car object, how do you guarantee that the stub's Drive method won't drift in signature from the concrete's method without some kind of...contract...to enforce it, thus rendering your tests meaningless unless you test objects by contract only.

## Interface References

In C#, you are allowed to create a reference variable of an interface type or in other words, you are allowed to create an interface reference variable. Such kind of variable can refer to any object that implements its interface. An interface reference variable only knows that methods which are declared by its interface declaration. It does not allow accessing any other variables or methods that might be supported by the objects. This concept is similar when you use a parent class reference to access a child class object.