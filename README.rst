CMSPlugin Frequently
============

django-cms plugin and apphook for the django-frequently app.

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    pip install cmsplugin-frequently

To get the latest commit from GitHub

.. code-block:: bash

    pip install -e git+git://github.com/bitmazk/cmsplugin-frequently.git#egg=cmsplugin_frequently

TODO: Describe further installation steps (edit / remove the examples below):

Add ``cmsplugin_frequently`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'cmsplugin_frequently',
    )

Add the ``cmsplugin_frequently`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^/', include('cmsplugin_frequently.urls')),
    )

Before your tags/filters are available in your templates, load them by using

.. code-block:: html

	{% load cmsplugin_frequently_tags %}


Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate cmsplugin_frequently


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    mkvirtualenv -p python2.7 cmsplugin-frequently
    make develop

    git co -b feature_branch master
    # Implement your feature and tests
    git add . && git commit
    git push -u origin feature_branch
    # Send us a pull request for your feature branch
