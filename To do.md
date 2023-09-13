# Intro to fastapi : 

- FastAPI is a modern, fast (high-performance), web framework for building APIs with Python 3.6+ based on standard Python type hints.

- https://fastapi.tiangolo.com/
# Why fastapi :

- Fast : Very high performance, on par with NodeJS and Go (thanks to Starlette and Pydantic).
- Fast to code : Increase the speed to develop features by about 200% to 300%.
- Fewer bugs : Reduce about 40% of human (developer) induced errors.
- Intuitive : Great editor support. Completion everywhere. Less time debugging.
- Easy : Designed to be easy to use and learn. Less time reading docs.
- Short : Minimize code duplication. Multiple features from each parameter declaration. Fewer bugs.
- Robust : Get production-ready code. With automatic interactive documentation.
- Standards-based : Based on (and fully compatible with) the open standards for APIs: OpenAPI (previously known as Swagger) and JSON Schema.

Let's get started:
- Activate virtual environment(ubuntu or mac):
    - `python3 -m venv env`
    - `source env/bin/activate`

- Activate virtual environment(windows):
    - `py -m venv env`
    - `.\env\Scripts\activate`

- Install fastapi and uvicorn:
    - `pip install fastapi`
    - `pip install uvicorn[standard]`


- Create a file main.py and add the following code:
    ```
    from fastapi import FastAPI

    app = FastAPI()


    @app.get("/")
    async def root():
        return {"message": "Hello World"}

    ```
- create a  
    - `uvicorn main:app --reload`