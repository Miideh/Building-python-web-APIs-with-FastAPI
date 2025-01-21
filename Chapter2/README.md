In this chapter, i learnt about the APIRouter class in FastAPI, which allows us to create modular and organized routes, connecting them seamlessly to the primary FastAPI instance. This approach helps maintain a clean and structured codebase, promoting better organization and readability.

Utilizing APIRouter
i began by understanding the purpose and usage of the APIRouter class. By defining routes using this class, i can group related endpoints together, making the code more maintainable. 


Creating Models for Request Bodies
Next is creating models for request bodies using Pydantic. Pydantic models provide built-in validation, ensuring that the data received in the request body adheres to the expected structure and data types. 

Path and Query Parameters
Adding path and query parameters to the operations was another crucial aspect covered in this chapter. Path parameters allow us to capture dynamic values from the URL, while query parameters enable us to handle optional inputs. 

Building a CRUD Todo Application
To put all these concepts into practice, i built a simple CRUD (Create, Read, Update, Delete) todo application. This application demonstrated how to combine routers, models, and parameters to create a fully functional API. Here’s a quick recap of the key operations:

Create: Adding a new todo item.

Read: Retrieving all todo items or a specific one by ID.

Update: Modifying an existing todo item.

Delete: Removing a todo item.

