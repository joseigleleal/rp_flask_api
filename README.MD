
# Create a Virtual Environment

In this section, you’ll build your project structure. You can name the root folder of your project any way you like. For example, you could name it `rp_flask_api/`. Create the folder and navigate into it:

```bash
mkdir rp_flask_api
cd rp_flask_api
```

In this case, you name the root folder of your project `rp_flask_api/`. The files and folders that you create over the course of this series will be located in either this folder or its subfolders.

After you navigate to the project folder, it’s a good idea to create and activate a virtual environment. That way, you’re installing any project dependencies not system-wide but only in your project’s virtual environment.

Select your operating system below and use your platform-specific command to set up a virtual environment:

### Linux + macOS

```bash
python -m venv venv
source venv/bin/activate
```

With the commands shown above, you create and activate a virtual environment named `venv` by using Python’s built-in `venv` module. The parenthesized `(venv)` in front of the prompt indicates that you’ve successfully activated the virtual environment.

## Add Dependencies

After you’ve created and activated your virtual environment, it’s time to install Flask with pip:

```bash
python -m pip install Flask==2.2.2
```

The Flask micro web framework is the main dependency that your project requires. On top of Flask, install Connexion to handle the HTTP requests:

```bash
python -m pip install "connexion[swagger-ui]==2.14.1"
```

To also make use of auto-generated API documentation, you install Connexion with the added support for Swagger UI. Later in this tutorial, you’ll learn more about the Python packages that you just installed.
