## Hash Tables

Are used to store data in key and value form, is synchronized. It is thread-safe and can be shared with many threads.
IT doesn't allow any null key or value, is a legacy class and  is slow.
Hashtable is internally synchronized and can't be unsynchronized.

![th4](https://tse3.mm.bing.net/th?id=OIP.m7hiSx2tSoVdfmHx3lF8MQFNC7&pid=Api&P=0&w=295&h=166)


### Hashing is implemented in two steps:

An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
The element is stored in the hash table where it can be quickly retrieved using hashed key.

hash = hashfunc(key)
index = hash % array_size

### What is a hash function?

The meaning of the verb “to hash” – to chop or scramble something – provides a clue as to what hash functions do to data. That’s right, they “scramble” data and convert it into a numerical value. And no matter how long the input is, the output value is always of the same length. Hash functions are also referred to as hashing algorithms or message digest functions. They are used across many areas of computer science, for example:

* To encrypt communication between web servers and browsers, and generate session IDs for internet applications and data caching
* To protect sensitive data such as passwords, web analytics, and payment details
* To add digital signatures to emails
* To locate identical or similar data sets via lookup functions