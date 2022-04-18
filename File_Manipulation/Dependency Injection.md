## Dependency Injection

ASP.NET Core is designed from scratch to support Dependency Injection. ASP.NET Core injects objects of dependency classes through constructor or method by using built-in IoC container.

Built-in IoC Container
ASP.NET Core framework contains simple out-of-the-box IoC container which does not have as many features as other third party IoC containers. If you want more features such as auto-registration, scanning, interceptors, or decorators then you may replace built-in IoC container with a third party container.

The built-in container is represented by IServiceProvider implementation that supports constructor injection by default. The types (classes) managed by built-in IoC container are called services.

There are basically two types of services in ASP.NET Core:

1. Framework Services: Services which are a part of ASP.NET Core framework such as IApplicationBuilder IHostingEnvironment, ILoggerFactory etc.
2. Application Services: The services (custom types or classes) which you as a programmer create for your application.


## Repository Pattern

The Domain layer contains enterprise logic and types and the Application layer contains business logic and types. The difference is that enterprise logic could be shared across many systems, whereas the business logic will typically only be used within a system.

![1_GiykAevGwTtP_6LQ1CB1Ug](https://user-images.githubusercontent.com/98957434/163886656-1ce962fe-7b04-47cb-b060-0f598f68362e.png)


### Domain layer contains:
* Entities
* Aggregates
* Value Objects
* Domain Events
* Enums
* Constants

## SOLID design principles
in C# are basic design principles. SOLID stands for Single Responsibility Principle (SRP), Open closed Principle (OSP), Liskov substitution Principle (LSP), Interface Segregation Principle (ISP), and Dependency Inversion Principle (DIP).  
 
### The reasons behind most unsuccessful applications Solutions
1. Intro to SOLID principles
2. SRP
3. OCP
4. LSP
5. ISP
6. DIP

### Intro to SOLID principles
 
SOLID principles are the design principles that enable us to manage most of the software design problems. Robert C. Martin compiled these principles in the 1990s. These principles provide us with ways to move from tightly coupled code and little encapsulation to the desired results of loosely coupled and encapsulated real needs of a business properly. SOLID is an acronym of the following.
S: Single Responsibility Principle (SRP)
O: Open closed Principle (OCP)
L: Liskov substitution Principle (LSP)
I: Interface Segregation Principle (ISP)
D: Dependency Inversion Principle (DIP)


### Example

public class SecurityHandler
{
    public bool LoginUser(string userName, string password)
    {
        LoginService service = new LoginService();
 
        return service.ValidateUser(userName, password);
    }
}

![th (13)](https://user-images.githubusercontent.com/98957434/163888287-206128a5-cfc2-45b2-adba-e050ebe65b00.jpg)
