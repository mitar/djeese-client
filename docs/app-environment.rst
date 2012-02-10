################
Application APIs
################

In addition to the standard Django and django CMS APIs, djeese apps may use
additional APIs only available on the djeese platform.


******************************
Inject snippets into templates
******************************

Your app may want to inject HTML into all templates rendered. One of the use
cases for this is an app that adds analytics supports, such as Google
Analytics, to the website. For this, there are two APIs, one to add content
into the head of the document, and one to add content to the bottom of the
page:


``template_api.registry``
=========================

This object has two public methods:

.. py:method:: template_api.registry.add_to_tail(content) 

    Adds content to the end of the document.

.. py:method:: template_api.registry.add_to_head(content)

    Adds content to the end of the document.
