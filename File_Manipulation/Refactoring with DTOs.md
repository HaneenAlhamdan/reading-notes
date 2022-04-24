## Refactoring with DTOs

Now here our goal is to show cart subtotal without including taxes. To achieve this goal we do not make any changes in OOB(out of the box) files but we use them from our created custom files to achieve this goal. We need to follow the following steps to achieve this goal.

* Create data transfer object(DTO)
* Create converter and populator
* Create facade and populate the data
* Call the facade from CartPageController/ Modify CartPageController
* Modify the cartTotal.tag file


## Create Data Transfer Objects (DTOs)
Now we will create one DTO(data transfer object) class named as SubTotalWithOutTax and it contains one property called as a sub of PriceData type. This sub property will hold the value of order subtotal without taxes.

Steps to create SubTotalWithOutTax DTO class
Navigate to yacceleratorfacades->resources and open yacceleratorfacades-beans.xml.
Add the following lines of code to yacceleratorfacades-beans.xml file.
SubTotalWithOutTax DTO class
Note: This entry must be between <beans> </beans> tag.
Build the hybris system by running ant clean all.
After successful build we can check our SubTotalWithOutTax DTO(data transfer object) class at the specified package and the file will look like this.

![Screenshot (239)](https://user-images.githubusercontent.com/98957434/164952599-fd2eb730-021a-4012-b26c-2728b7f8cb3e.png)

## Create an ASP.NET Core 3.1 API project
First off, let’s create an ASP.NET Core project in Visual Studio. Assuming Visual Studio 2019 is installed in your system, follow the steps outlined below to create a new ASP.NET Core API project in Visual Studio.

1. Launch the Visual Studio IDE.
2. Click on “Create new project.”
3. In the “Create new project” window, select “ASP.NET Core Web Application” from the list of the templates displayed.
4. Click Next. 
5. In the “Configure your new project” window, specify the name and location for the new project.
6. Click Create. 
7. In the “Create New ASP.NET Core Web Application” window shown next, select .NET Core as the runtime and ASP.NET Core 3.1 (or later) from the drop-down list at the top.
8. Select “API” as the project template to create a new ASP.NET Core API application. 
9. Ensure that the check boxes “Enable Docker Support” and “Configure for HTTPS” are unchecked as we won’t be using those features here.
10. Ensure that Authentication is set as “No Authentication” as we won’t be using authentication either.
11. Click Create. 


## How to use DTOs

### Use DTOs for abstraction
You can take advantage of DTOs to abstract the domain objects of your application from the user interface or the presentation layer. In doing so, the presentation layer of your application is decoupled from the service layer. So if you would like to change the presentation layer, you can do that easily while the application will continue to work with the existing domain layer. Similarly, you can change the domain layer of your application without having to change the presentation layer of the application.

### Use DTOs for data hiding
Another reason you would want to use DTOs is data hiding. That is, by using DTOs you can return only the data requested. As an example, assume you have a method named GetAllEmployees() that returns all the data pertaining to all employees. Let’s illustrate this by writing some code.
In the project we created earlier, create a new file called Employee.cs. Write the following code inside this file to define a model class named Employee.