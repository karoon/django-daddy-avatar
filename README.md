django-daddy-avatar
===================

simple django avatar from gravatar

Installation
------------

To install:

    pip install django-daddy-avatar

Usage:

    INSTALLED_APPS = (
        ...
        'daddy-avatar',
        ...
    )

    {% load daddy_avatar %}
    <!-- from string -->
    <img src="{{'vchakoshy@gmail.com'|daddy_avatar:50}}" />

    <!-- from queryset -->
    <img src="{{post.user.email|daddy_avatar:200}}" />
