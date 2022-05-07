## Roles_Claims_Tokens

When an identity is created for authenticated user, it may be assigned one or more claims which are issued by trusted party. The claim is a name-value pair that represents what the subject is or is not, instead of what the subject can and cannot do. The claim based authorization checks the value of the claim and allows access to the resource, based on that value.


## Adding claims checks
Claim based authorization checks:

1. Are declarative.
2. Are applied to Razor Pages, controllers, or actions within a controller.
3. Can not be applied at the Razor Page handler level, they must be applied to the Page.

Claims in code specify claims which the current user must possess, and optionally the value the claim must hold to access the requested resource. Claims requirements are policy based, the developer must build and register a policy expressing the claims requirements.

The simplest type of claim policy looks for the presence of a claim and doesn't check the value.

## Difference between Authentication and Authorization
 
![Untitled-4](https://user-images.githubusercontent.com/98957434/167267274-ca9ed13c-4084-46ba-a150-6be2f7827877.jpg)

In authentication process, the identity of users are checked for providing the access to the system. While in authorization process, person’s or user’s authorities are checked for accessing the resources. Authentication is done before the authorization process, whereas authorization process is done after the authentication process.

## JWT to authenticate Servers API’s

### What is JWT?

A JWT is a mechanism to verify the owner of some JSON data. It’s an encoded, URL-safe string that can contain an unlimited amount of data (unlike a cookie) and is cryptographically signed.
When a server receives a JWT, it can guarantee the data it contains can be trusted because it’s signed by the source. No middleman can modify a JWT once it’s sent.


### When to use JWT authentication

JWT is a particularly useful technology for API authentication and server-to-server authorization.

![th (17)](https://user-images.githubusercontent.com/98957434/167267560-e5908743-87e6-40cf-97ae-22d98e74fd2b.jpg)


### Following are some standard claims: Wikipedia

* Issuer (iss) - identifies principal that issued the JWT;

* Subject (sub) - identifies the subject of the JWT;

* Audience (aud) - The "aud" (audience) claim identifies the recipients that the JWT is intended for. Each principal intended to process the JWT must identify itself with a value in the audience claim. If the principal processing the claim does not identify itself with a value in the aud claim when this claim is present, then the JWT must be rejected.

* Expiration time (exp) - The "exp" (expiration time) claim identifies the expiration time on or after which the JWT must not be accepted for processing. The value should be in NumericDate[10][11] format.

* Not before (nbf) - Similarly, the not-before time claim identifies the time on which the JWT will start to be accepted for processing.

* Issued at (iat) - The "iat" (issued at) claim identifies the time at which the JWT was issued.

* JWT ID (jti) - case sensitive unique identifier of the token even among different issuers.