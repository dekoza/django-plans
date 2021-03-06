Installation
============

Setup for django project
------------------------

You can install app using package manager directly from github::

    $ pip install -e git://github.com/cypreess/django-plans.git#egg=django-plans

Now you need to configure your project. Add this app to your ``INSTALED_APPS`` setting::

    INSTALLED_APPS += ('plans', )

Define all **required** settings options described in :doc:`settings`.

Don't forget to run ``manage.py syncdb`` in your project or run south migration if you use south.

Running example project
-----------------------

Clone git repository to your current directory::

    $ git clone git://github.com/cypreess/django-plans.git


Optionally create virtual env and get required packages to run example project::

    $ cd django-plans/example
    $ pip install -r pip_example.req


Initialize example project database::

    $ cd ..
    $ python manage.py syncdb

Load an initial data (used also for testing)::

    $ python manage.py loaddata test_django-plans_auth test_django-plans_plans


Start dev webserver:

    $ python manage.py runserver