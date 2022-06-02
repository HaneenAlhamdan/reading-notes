## MVC / Cookies

### What are HTTP cookies?

Cookies are small pieces of data used as a storage medium in the browser and sent to the server with each request. They are helpful for session management, user personalization, and tracking.

1. Session management:
2. User personalization:
3. Tracking:

![th (20)](https://tse3.mm.bing.net/th?id=OIP.z6V8OMLRQyejV7h6PnOKswAAAA&pid=Api&P=0&w=296&h=153)


### How to create HTTP cookies

1. Client-side

After opening the console, you can set a cookie with JavaScript by typing out the code:
document.cookie="example=1"

2. Web server-side

In the case where you wish to build your own website, you can create a HTML script where a button creates a cookie.
<<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-compatible" content ="ie=edge">
    <title>Document</title>

</head>
<body>
    <button id = 'btnCreateCookie'>Create Cookie </button>
    <script>
      const btnCreateCookie = document.getElementbyID("btnCreateCookie")
      btnCreateCookie.addEventLister("click", e=> document.cookie = "example-3")
    </script>
</body>
</html>

### CookieOptions

As an optional third parameter to the Append() method we just used, you can pass an instance of the CookieOptions class

using Microsoft.AspNetCore.Http;