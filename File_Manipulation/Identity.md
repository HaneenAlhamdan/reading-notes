# Identity

## Intro to Identity

ASP.NET Identity allows you to add customized login/logout functionality and customized profile features that make it easy to customize the data about the logged-in user. Today there is a much broader array of data storage (which is increasing very quickly) options for web application and most of the developers want to enable their websites to use the social identity providers for Authentication and Authorization. Now what do the two terms Authentication and Authorization mean?

### There are four modes of authentication:-

1. No Authentication: This authentication mode doesn't require any user authentication for applications.

2. Individual User Accounts: This type of application is configured to use ASP.NET Identity for user authentication that was already known as ASP.NET Membership in early days. ASP.NET Identify enables a user to register for an account either by creating an account on the website itself by creating a username and word or by signing in through social providers such as Twitter, Facebook, Microsoft Account or Google.

3. Organizational Accounts: This type of authentication mode will be configured to use Windows Identity Foundation (WIF) based on user accounts in Active Directory, Microsoft Azure Active Directory, or Office 365.

4. Windows Authentication: This mode of authentication will support Windows Identity IIS module for authentication. IIS stands for Internet Information Services that acts as a web server for .NET application specially designed for Windows Operating Systems. This authentication is intended for Intranet Applications.


### There are the following six important pieces of the ASP.NET Identity system:
 User
* Role
* User Manager
* Role Manager
* Authentication Manager
* Entity Framework DBContext


## Identity Demystified

### API Resources
 Identity Server Models (or the underlying tables),  a few tables that start with Api***. 
Here are the tables:

![1_HO7wMyGSNom1QAX-rLYZjg](https://user-images.githubusercontent.com/98957434/165363628-2232abb3-8738-4abc-9e3d-533ae6177a82.jpeg)


### What is an API Claim?

A Claim represents a single fact about the user. It could be the user's first name, last name, age, employer, birth date, or anything else that is true about the user. A single claim will contain only a single piece of information. A claim representing something about a user John Smith could be his first name: John. A second claim would be his last name: Smith.
Claims are represented by the Claim class in ASP.Net Core. It's most common constructor accepts two strings: type and value. The 'type' parameter is the name of the claim, while the value is the information the claim is representing about the user.