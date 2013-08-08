nikola-event-kit
================

Just enough stuff to help you setup a small event, like a PyDay

How to get started (In Linux)
-----------------------------

Create a virtualenv and activate it::

    virtualenv venv
    . venv/bin/activate

Install Nikola in it::

    pip install nikola

If you run into trouble getting that in place, feel free to ask for help, this will only be
difficult once, I swear.

From now on, whenever you need to use Nikola, always remember to activate the virtualenv first::

    . venv/bin/activate

How to get your site built
--------------------------

::

    cd site
    nikola build

How to see the results
----------------------

::

    nikola serve
    xdg-open http://localhost:8000

How to make it be your own site
-------------------------------

Edit ``site/conf.py`` and change the obvious things::

    BLOG_AUTHOR
    BLOG_TITLE
    SITE_URL
    BLOG_EMAIL
    BLOG_DESCRIPTION
    DEFAULT_LANG
    TRANSLATIONS
    SIDEBAR_LINKS (maybe)

And now, edit the files inside ``stories`` to change the site's contents. Those files are written in `reStructuredText <http://nikola.ralsina.com.ar/quickstart.html>`_

How to make it not look like a generic bootstrap site
-----------------------------------------------------

Get a theme from http://themes.nikola.ralsina.com.ar or `create your own <http://nikola.ralsina.com.ar/creating-a-theme.html>`_

How to <other thing>
--------------------

Ask at the `Nikola discuss google group <http://groups.google.com/group/nikola-discuss>`_
Rebuild and check as needed.
