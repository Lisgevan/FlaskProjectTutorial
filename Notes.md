# 1. Create and activate a virtual environment

## **A. Create an environment**

**Create a project folder and a .venv folder within:**

    (Windows)

    ```python
    > mkdir myproject
    > cd myproject
    > py -3 -m venv .venv
    ```

## **B. Activate the environment**

**Before you work on your project, activate the corresponding environment:**

    (Windows)

    ```python
    > .venv\Scripts\activate
    ```

_Your shell prompt will change to show the name of the activated environment._

# Install Flask

    ```python
    pip install Flask
    ```

# Flask project typical stracture:

- flaskr/, a Python package containing your application code and files.
- tests/, a directory containing test modules.
- .venv/, a Python virtual environment where Flask and other dependencies are installed.
- Installation files telling Python how to install your project.
- Version control config, such as git. You should make a habit of using some type of version control for all your projects, no matter the size.
- Any other project files you might add in the future.

_By the end, your project layout will look like this:_

```
/home/user/Projects/flask-tutorial
├── flaskr/
│   ├── __init__.py
│   ├── db.py
│   ├── schema.sql
│   ├── auth.py
│   ├── blog.py
│   ├── templates/
│   │   ├── base.html
│   │   ├── auth/
│   │   │   ├── login.html
│   │   │   └── register.html
│   │   └── blog/
│   │       ├── create.html
│   │       ├── index.html
│   │       └── update.html
│   └── static/
│       └── style.css
├── tests/
│   ├── conftest.py
│   ├── data.sql
│   ├── test_factory.py
│   ├── test_db.py
│   ├── test_auth.py
│   └── test_blog.py
├── .venv/
├── pyproject.toml
└── MANIFEST.in
```

# Run the application

    ```
    flask --app flaskr run --debug
    ```
