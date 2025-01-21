# In this chapter, i started with learning git basics and then proceeded to setting up development environment by installing the essential tools needed. The chapter showed a guide to installating Python, a prerequisite for FastAPI. i learned how to check if Python is already installed on the system and how to install it if it wasn’t. Once Python was installed, i proceeded to setting up a virtual environment to manage my project's dependencies effectively. i also learnt what Docker is,how to install and create a file. After setting up Python and the virtual environment, i moved on to installing FastAPI and Uvicorn. FastAPI is a modern, fast web framework for building APIs with Python . The installation process involved using pip, Python's package installer. The command pip install fastapi uvicorn was used to install FastAPI along with all its optional dependencies, which include Uvicorn. This setup ensured i had all the tools necessary to build and run the FastAPI application.With the environment set up and the tools installed, i transitioned to building a simple API as an introduction to FastAPI. The chapter provided a step-by-step guide to creating the first FastAPI application. i started by creating a new Python file, typically named `api.py'.The next step was to instantiate the FastAPI class to create an app instance:

from fastapi import FastAPI

app = FastAPI()
With the app instance ready, i moved on to defining the first route. A route in FastAPI is an endpoint that responds to client requests. i defined a route using the @app.get("/") decorator, indicating that this route would respond to GET requests sent to the root URL ("/"). Inside the route function, i simply returned a welcome message.

@app.get("/")
 async def welcome() -> dict:
    return { "message": "Hello World"}
After defining the route, the next step was to run the application. i used Uvicorn for this purpose, with the command uvicorn main:app --reload. Running this command started a development server, and the API was now accessible at http://127.0.0.1:8080.

i then tested the API by navigating to the URL in a web browser or using tools like curl. Seeing the welcome message response confirmed that the API was set up correctly and functioning as expected.

This chapter laid a solid foundation for working with FastAPI. i covered the essential steps of setting up the development environment, installing necessary tools, and building a simple API. By the end of the chapter, i had a basic understanding of FastAPI and how to create routes.

In summary, i:

Installed Python and created a virtual environment.
Installed FastAPI and Uvicorn.
Built a simple FastAPI application.
Defined a route to handle GET requests.
Ran and tested the API using Uvicorn.