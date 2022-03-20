## File and Stream I/O
The stream is basically the sequence of bytes passing through the communication path. There are two main streams: the input stream and the output stream. 
* The input stream is used for reading data from file (read operation) 
* The output stream is used for writing into the file (write operation).
 
 ![Example](https://user-images.githubusercontent.com/98957434/158898050-9136de36-b0ba-4921-87ab-67fcea0f9bb6.jpg)

## Write to a file
 StreamWriter class is one of the common ways to create and write to a file. The StreamWriter constructor takes a full file name and creates the file if it does not exist. 
 Example:-
  Console.WriteLine("Welcome in my world");

## Read to a file
The File.ReadAllText() method opens a text file, reads all the text in the file into a string, and then closes the file.
Example:-
 text = File.ReadLine();