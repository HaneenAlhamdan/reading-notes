## LINQ & Delegates

In C#, LINQ is present in System.Linq namespace. It provides different type of classes and methods which supports LINQ queries. In this namespace:

* Enumerable class holds standard query operators that operate on object which executes IEnumerable<T>.
* Queryable class holds standard query operators that operate on object which executes IQueryable<T>.


![Untitled-Diagram24](https://user-images.githubusercontent.com/98957434/161871747-58e70092-60f1-4e98-a838-872fe210ee7f.jpg)


## Advantages of LINQ
- User does not need to learn new query languages for a different type of data source or data format.
- It increase the readability of the code.
- Query can be reused.
- It gives type checking of the object at compile time.
- It provides IntelliSense for generic collections.


## Three Parts of a Query Operation
1. Obtain the data source.
2. Create the query.
3. Execute the query.

![th (6)](https://user-images.githubusercontent.com/98957434/161872437-871b745b-774b-4234-9ac4-63bd36d8786b.jpg)


## Connecting C# with Database:
 To work with a database, the first of all you required a connection. The connection to a database normally consists of the below-mentioned parameters.

var queryAllCustomers = from cust in customers
                        select cust;



## To execute the query

1. Now write the foreach loop that will cause the query to execute. Note the following about the code:

    * Each element in the returned sequence is accessed through the iteration variable in the foreach loop.

    * The type of this variable is Student, and the type of the query variable is compatible, IEnumerable<Student>.

2. After you have added this code, build and run the application to see the results in the Console window.

foreach (Student student in studentQuery)
{
    Console.WriteLine("{0}, {1}", student.Last, student.First);
}