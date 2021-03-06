Global Humanitarians Unite
==========================

This is the Global Humanitarians Unite website prototype.

See `LICENSE` to read the license (Apache 2.0), and `CHANGELOG.md` for the
release log.

Environment Setup
-----------------

    $ bower install
    $ virtualenv -p python3 venv
    $ . venv/bin/activate
    $ pip install -r requirements.txt

Initializing the Application
----------------------------

With the environment set up, now you can configure the application:

    $ cd ghu_web
    $ python generate_key.py
    $ python manage.py migrate
    $ python manage.py loaddata pages.json

Running a Debug Server
----------------------

After activating the virtualenv and `cd`ing to `ghu_web/`:

    $ python manage.py runserver

Deployment
----------

See the `/deploy/` directory in this repository for instructions on
deploying the site.
