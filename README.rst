Django AJAX SEARCH ENGINE
===================

A customizable AJAX-powered search engine for Django.

FEATURES
-----------------------------------

- Works with the latest jQuery library version
- Displays instant search results as you type


INSTALLATION REQUIREMENTS
-----------------------------------

- Python 2.6 or Python 2.7
- `Django <http://www.djangoproject.com/>`_ >= 1.3
- `jQuery <http://jquery.com/>`_ >= 1.4.4

To Install::
    
    easy_install django-ajax-search

Next Add `ajax search` To Your `INSTALLED_APPS` To Include The Related css/js::

    INSTALLED_APPS = (
        'django.contrib.staticfiles',
        # Other apps here
        'ajax-search',
    )

The jQuery and jQuery UI libraries are not included in the distribution but must be included
in your templates. See the example project for an example using these libraries from the
Google CDN.

Once Installed You Should Add The Urls To Your Root Url Patterns::

    urlpatterns = patterns('',
        # Other patterns go here
        url(r'^ajax-search/',include('ajax-search.urls')),
    )

Full Documentation At http://django-ajax-search.readthedocs.org/
	
ADDITIONAL HELP AND SUPPORT
-----------------------------------

You Can Find Additional Help Or Support On The Mailing List: http://groups.google.com/group/django-ajax-search
