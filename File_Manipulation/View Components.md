## View Components

View components are one of the potentially less well known features of ASP.NET Core Razor views. Unlike tag-helpers which have the pretty much direct equivalent of Html Helpers in the previous ASP.NET, view components are a bit different.
In spirit, they fit somewhere between a partial view and a full controller - approximately like a ChildAction. However whereas actions and controllers have full model binding semantics and the filter pipeline etc, view components are invoked directly with explicit data. They are more powerful than a partial view however, as they can contain business logic, and separate the UI generation from the underlying behaviour.

View components seem to fit best in situations where you would want to use a partial, but that the rendering logic is complicated and may need to be tested.

### Creating a view component
View components can be defined in a multitude of ways. You can give your component a name ending in ViewComponent, you can decorate it with the [ViewComponent] attribute, or you can derive from the ViewComponent base class. The latter of these is probably the most obvious, and provides a number of helper properties you can use, but the choice is yours.

To implement a view component you must expose a public method called InvokeAsync which is called when the component is invoked:

public Task<IViewComponentResult> InvokeAsync();



### Our InvokeAsync method
 is pretty self explanatory. We are checking if the current user is signed in using the SignInManager<>, and if they are we fetch the associated ApplicationUser from the UserManager<>. Finally we call the helper View method, passing in a template to render and the model user. If the user is not signed in, we call the helper View without a template argument.

The calls at the end of the InvokeAsync method are reminiscent of action methods. They are doing a very similar thing, in that they are creating a result which will execute a view template, passing in the provided model.


### What is the View Component in Asp.Net Core?
The view component is a new feature in Asp.net Core, it looks like the partial view in asp.net framework MVC but it is stronger and more powerful. View component separate view and business code to different other files to management. ViewComponents are completely self-contained objects that consistently render Html from a razor view. View components don't use model binding and only depend on the data provided when calling into it.

### A View Component has some features below:

1. Separate Html and logic code.
2. Support invoke async help load page faster.
3. Separate code helps make unit tests easy.
4. Renders a chunk rather than a whole response.
5. Fully supports constructor dependency injection.

![The-Poco-view-component](https://user-images.githubusercontent.com/98957434/173241557-55d70abf-1abf-4fcc-87cd-3f23fc1aba28.jpg)
