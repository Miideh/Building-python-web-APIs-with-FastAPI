#

Chapter 7 focused on improving the security of a FastAPI application using OAuth and JSON Web Tokens (JWT).

OAuth and JWT:
OAuth is an open-standard authorization protocol or framework that allows third-party services to exchange user information without exposing their credentials. JWT, on the other hand, is a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

In the FastAPI application, OAuth was implemented to manage user authentication and authorization.JWT was used to create secure tokens that represent the user's authentication state. These tokens are sent to clients upon successful authentication and must be included in subsequent requests to access protected routes.

Dependency Injection:
Another critical topic covered in this chapter is dependency injection, a design pattern used to implement IoC (Inversion of Control). It allows developers to inject dependencies into a class, rather than having the class manage its dependencies. This leads to more modular, testable, and maintainable code.

In FastAPI, dependency injection is seamlessly integrated. i learned how to define dependencies that route handlers can use.

Protecting Routes:
In this chapter, I learnt how to protect routes from unauthorized access. By using dependencies for JWT token verification, i ensured that only authenticated users could access certain endpoints. This is achieved by declaring dependencies in the route definitions. If the token is missing or invalid, the user receives an appropriate error message and is denied access to the protected resource.

CORS Middleware:
Cross-Origin Resource Sharing (CORS) is a security feature that restricts how resources on a web server can be accessed by pages from a different domain. To allow our API to be accessed by clients from any domain, i added a CORS middleware to the FastAPI application. This middleware allows us to specify which origins, methods, and headers are permitted.

CORS settings was configured to permit access from any client, enabling broader accessibility to the API. This is particularly useful when building APIs that will be consumed by web applications hosted on different domains.
