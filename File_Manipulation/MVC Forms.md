## MVC Forms


### What is FormMethod?
 
FormMethod is a command which executes form as POST or GET. FormMethod made HTTP request either in GET or POST form.

![MVC_Architecture](https://user-images.githubusercontent.com/98957434/170842649-a5ec0b91-a7db-4cb5-8833-3f925f53c4d7.png)


Advantage:
1. It is easy to create a form using Weakly Typed mechanism
2. Mostly used when you need to create a form with one or two input items.

Disadvantage:
1. Because, it is not strongly typed so IntelliSense doesn't help you.
2. Have higher chance of getting exception and runtime error messages.

Step 1: Create a new MVC Application, By Selecting Empty Template and adding MVC Core Reference.