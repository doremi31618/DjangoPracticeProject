# Python on Replit

This is a template to get you started with Python on Replit. It's ready to go so you can just hit run and start coding!

## Running the repl

1. Setup a new secret environment variable (the lock icon) where the key is `SECRET_KEY` and the value is
   a randomly generated token of 32 bits of randomnese. To generate such a token type this into the shell and hit Enter:
```
python
import secrets
secrets.token_urlsafe(32)
```
2. Hit run!

See this 1 minute video for a walkthrough: [https://www.loom.com/share/ecc4e738149f4d1db3bcff01758b3e71](https://www.loom.com/share/341b5574d12040fb9fcbbff150777f1c)

## Installing packages

To add packages to your repl, you can just import directly in the file you want to use the package in, and it will automatically be installed when you press the run button. Like below:
```python
import math
import pandas as pd
```

You could also install packages by using the Replit packager interface in the left sidebar.

## Installed Django from scratch
to setup django on "repl.it" you would need following steps

### installed django
```
pip3 install django
```

### start a new project
```
django-admin startproject <replace_with_your_project_name> .
```

### start a new app
```
python manage.py startapp <replace_with_your_app_name> 
```

### add ALLOWED_HOSTS path to settings.py
```python
ALLOWED_HOSTS = [   
  '*'
]

```

### start server 
you need to specified the host and port to let replit show the webview
``` 
python manage.py runserver 0.0.0.0:3000
```

## Issue 

### Failed to install psycopg2 package 

due to the reason why failed to install psycopg2 is because lack with some required package to build the entire pkg

solution is just install psycopg2-binary
```python
pip install psycopg2-binary
```

