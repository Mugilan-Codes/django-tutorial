# Django Tutorial

## Learning Django by following Official Docs. Also learing pyenv, pyenv-virtualenv, & poetry

- [Django](https://www.djangoproject.com/) (Official Website) - The web framework for perfectionists with deadlines.
- [Writing your first Django app](https://docs.djangoproject.com/en/3.2/intro/tutorial01/) - this is part 1, visit the link for more

### PRE-REQUISITE

- Python is required. You can install it anyway you want, i prefer pyenv
- [pyenv](https://github.com/pyenv/pyenv) - Simple Python version management
- [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv) - a pyenv plugin to manage virtualenv (a.k.a. python-virtualenv)
- [poetry](https://github.com/python-poetry/poetry) - Python dependency management and packaging made easy

### STEPS

1. Make a project folder

   ```sh
   mkdir <project_folder> && $_
   ```

1. Create a Virutalenv using pyenv-virtualenv or poetry (or any other). Make sure to select the correct interpreter in vscode

   ```sh
   # create
   pyenv virtualenv <python_version> <virtualenv_name>

   # set the environment to auto-activate (.python-version) 
   pyenv local <virtualenv_name>

   # dependency manager
   poetry init
   ```

1. Install Package

   ```sh
   poetry add django
   ```

1. Start project

   ```sh
   poetry run django-admin.py startproject <project_name> .
   ```

1. Export dependencies to a requirements.txt

   ```sh
   poetry export -f requirements.txt --output requirements.txt
   ```

#### RESOURCES

- [Time zones](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/) - time zone handling
- [Related objects reference](https://docs.djangoproject.com/en/3.2/ref/models/relations/) - model relations
- [Field lookups](https://docs.djangoproject.com/en/3.2/topics/db/queries/#field-lookups-intro) - how to use double underscores
- [Making queries](https://docs.djangoproject.com/en/3.2/topics/db/queries/) - database API
- [URL dispatcher](https://docs.djangoproject.com/en/3.2/topics/http/urls/) - use of URLconfs. A URLconf maps URL patterns to views
- PyLint (Optional) - DevDependency
  - [PyLint for Django in VSCode](https://dkolodzey.medium.com/pylint-for-django-in-vscode-f3fadb8462d) - Medium Article
  - [Missing Docstring](https://stackoverflow.com/a/54881400/12381908) - Stackoverflow
- [Templates](https://docs.djangoproject.com/en/3.2/topics/templates/)
- [Avoiding race conditions using F()](https://docs.djangoproject.com/en/3.2/ref/models/expressions/#avoiding-race-conditions-using-f)
- [Class-based views](https://docs.djangoproject.com/en/3.2/topics/class-based-views/)
- [Testing in Django](https://docs.djangoproject.com/en/3.2/topics/testing/)
- Static Files
  - [Managing static files (e.g. images, JavaScript, CSS)](https://docs.djangoproject.com/en/3.2/howto/static-files/)
  - [The staticfiles app](https://docs.djangoproject.com/en/3.2/ref/contrib/staticfiles/)
  - [Deploying static files](https://docs.djangoproject.com/en/3.2/howto/static-files/deployment/) discusses how to use static files on a real server.

#### REFERENCES

- [SETTING UP A DJANGO 3 PROJECT WITH POETRY](https://davebaker.me/2020/07/19/setting-up-django-project-with-poetry/)
- [Managing a Django Project with Poetry](https://rasulkireev.com/managing-django-with-poetry/)
- [Get started with pyenv & poetry. Saviours in the python chaos!](https://blog.jayway.com/2019/12/28/pyenv-poetry-saviours-in-the-python-chaos/)
- [Poetry virtual environment in project root](https://github.com/python-poetry/poetry/issues/108#issuecomment-628681234) - Github Discussions
- [Python: Setting Up Project Environment](https://dev.to/jaeheonjee/python-setting-up-project-environment-1ei8) - Example
