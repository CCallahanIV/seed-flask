Flask App Seed
======

A seed project based off of Flask's Flaskr tutorial
https://flask.palletsprojects.com/en/1.1.x/tutorial/


Install
-------

Create a virtualenv and activate it::

    $ python3 -m venv venv
    $ . venv/bin/activate

Install app::

    $ pip install -e .


Run
---

::

    $ export FLASK_APP=app
    $ export FLASK_ENV=development
    $ flask init-db
    $ flask run

Or on Windows cmd::

    > set FLASK_APP=app
    > set FLASK_ENV=development
    > flask init-db
    > flask run

Open http://127.0.0.1:5000 in a browser.


Test
----

::

    $ pip install '.[test]'
    $ pytest

Run with coverage report::

    $ coverage run -m pytest
    $ coverage report
    $ coverage html  # open htmlcov/index.html in a browser
