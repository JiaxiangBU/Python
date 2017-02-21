# How to install requests?

At 1st, Go to the Mac Terminal, type `pip install requests` and `return`.

Terminal replies:
`Collecting requests

Using cached requests-2.13.0-py2.py3-none-any.whl

Installing collected packages: requests

Successfully installed requests-2.13.0`

* Do not type `pip install requests` and `return` in IDLE. The good reason:

> pip is run from the command line, not the Python interpreter. It is a program that installs modules, so you can use them from Python. Once you have installed the module, then you can open the Python shell and do import selenium.

> The Python shell is not a command line, it is an interactive interpreter. You type Python code into it, not commands.

From: http://stackoverflow.com/questions/8548030/why-does-pip-install-inside-python-raise-a-syntaxerror

And next, type `import requests` in IDLE.
