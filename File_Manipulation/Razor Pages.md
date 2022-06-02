## Razor Pages

Razor Pages is a new feature of ASP.NET Core that makes coding page-focused scenarios easier and more productive. Initial impression of the public was that Razor Pages is easier and faster alternative to MVC for smaller apps that are solely page focused. However, it turns out that it just might be bigger than that.

## Code Snippets
All snippets are included in their final form. They exclude namespaces, as those may differ depending on the project name.

Index.cshtml


![th8](https://tse3.mm.bing.net/th?id=OIP.Xq3Kfi6jMqyGMGWYtD4pkQHaDM&pid=Api&P=0&w=387&h=166)

## Examine the project files

* Pages folder
Contains Razor pages and supporting files. Each Razor page is a pair of files:

A .cshtml file that has HTML markup with C# code using Razor syntax.
A .cshtml.cs file that has C# code that handles page events.

* wwwroot folder
Contains static assets, like HTML files, JavaScript files, and CSS files. For more information, see Static files in ASP.NET Core.

* appsettings.json
Contains configuration data, like connection strings. For more information, see Configuration in ASP.NET Core.

* Program.cs
var builder = WebApplication.CreateBuilder(args);

// Add services to the container.
builder.Services.AddRazorPages();

var app = builder.Build();

// Configure the HTTP request pipeline.
if (!app.Environment.IsDevelopment())
{
    app.UseExceptionHandler("/Error");
    // The default HSTS value is 30 days. You may want to change this for production scenarios, see https://aka.ms/aspnetcore-hsts.
    app.UseHsts();
}

app.UseHttpsRedirection();
app.UseStaticFiles();

app.UseRouting();

app.UseAuthorization();

app.MapRazorPages();

app.Run();