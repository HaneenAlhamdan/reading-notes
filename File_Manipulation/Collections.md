## Collections
Collections standardize the way of which the objects are handled by your program. In other words, it contains a set of classes to contain elements in a generalized manner. With the help of collections, the user can perform several operations on objects like the store, update, delete, retrieve, search, sort etc.


![Collections](https://user-images.githubusercontent.com/98957434/161398476-65acd5e7-7156-46a6-b76c-6d7572e83e5e.jpg)


* Dictionary<TKey,TValue>:-It stores key/value pairs and provides functionality similar to that found in the non-generic Hashtable class.

* List<T>	It is a dynamic array that provides functionality similar to that found in the non-generic ArrayList class.

* Queue<T>	A first-in, first-out list and provides functionality similar to that found in the non-generic Queue class.

* SortedList<TKey,TValue>	It is a sorted list of key/value pairs and provides functionality similar to that found in the non-generic SortedList class.

* Stack<T>	It is a first-in, last-out list and provides functionality similar to that found in the non-generic Stack class.

* LinkedList<T>	It allows fast inserting and removing of elements. It implements a classic linked list.

## Enumeration (or enum)
Enumeration (or enum) is a value data type in C#. It is mainly used to assign the names or string values to integral constants, that make a program easy to read and maintain. For example, the 4 suits in a deck of playing cards may be 4 enumerators named Club, Diamond, Heart, and Spade, belonging to an enumerated type named Suit. Other examples include natural enumerated types (like the planets, days of the week, colors, directions, etc.). The main objective of enum is to define our own data types(Enumerated Data Types). Enumeration is declared using enum keyword directly inside a namespace, class, or structure.

### Example:-
enum days
{

    Sat,
    Sun,
    Mon,
    Tus,
    Wed,
    Thu,
    Fri,
 
}