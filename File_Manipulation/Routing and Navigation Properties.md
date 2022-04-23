## Routing and Navigation Properties


## Routing within MVC

In the ASP.NET Web Forms application, every URL must match with a specific .aspx file. For example, a URL http://domain/studentsinfo.aspx must match with the file studentsinfo.aspx that contains code and markup for rendering a response to the browser.
Routing is not specific to the MVC framework. It can be used with ASP.NET Webform application or MVC application.
ASP.NET introduced Routing to eliminate the needs of mapping each URL with a physical file. Routing enables us to define a URL pattern that maps to the request handler. This request handler can be a file or class. In ASP.NET Webform application, request handler is .aspx file, and in MVC, it is the Controller class and Action method. For example, http://domain/students can be mapped to http://domain/studentsinfo.aspx in ASP.NET Webforms, and the same URL can be mapped to Student Controller and Index action method in MVC.


![routing-process](https://user-images.githubusercontent.com/98957434/164866135-4a25edb5-c151-4c65-8c2c-531815991a5b.png)

### Configure a Route
Every MVC application must configure (register) at least one route configured by the MVC framework by default. You can register a route in RouteConfig class, which is in RouteConfig.cs under App_Start folder. The following figure illustrates how to configure a route in the RouteConfig class .

As you can see in the above figure, the route is configured using the MapRoute() extension method of RouteCollection, where name is "Default", url pattern is "{controller}/{action}/{id}" and defaults parameter for controller, action method and id parameter. Defaults specify which controller, action method, or value of id parameter should be used if they do not exist in the incoming request URL.

In the same way, you can configure other routes using the MapRoute() method of the RouteCollection class. This RouteCollection is actually a property of the RouteTable class.


## Routing within Core

There are two types of routing:
* Conventional Routing
* Attribute Routing

### How Routing Works in ASP.NET Core?

![Screenshot (237)](https://user-images.githubusercontent.com/98957434/164868000-30d431d1-3c97-4f52-9942-f7a945563f5c.png)


### Conventional Routing in ASP.NET Core
The conventional routing is determined based on the conventions defined in the route templates which will map the incoming Requests path to controllers and their action methods. This convention based to routes are defined within the Configure method of the Startup.cs class file.

The conventional Routing establishes a convention for the URL path, such that given a template:

First token maps to a controller
Second token maps to an action
Third token maps to the optional id action parameter



### Attribute Routing in ASP.NET Core
This route is determined based on the attributes which are configured either at the controller level or at the action method level and we can use both Conventional Routing and Attribute Routing in a single application.

Attribute routing maps the URLs by applying routing template directly on the controller and action. There is an existence of controller and action in the template is not mandatory for the attribute routing, as they don’t play any part in the routing process.

We can use the [Route] or [HttpGet] (and other verbs) attributes to specify templates. This template can also have literals and tokens (except for controller and action tokens).

Attribute apply to the controller are merged with those on an action for E.g.In the HomeController, PageOne action can be access via /home/one URL.

