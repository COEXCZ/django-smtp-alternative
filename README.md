django_smtp_alternative
=======================

Django email backend providing sending with alternative SMTP server if primary server fails

Installation
------------

```bash
$ pip install django-smtt-alternative
```

Usage
-----

settings.py

::
  EMAIL_BACKEND = "django_smtp_alternative.EmailBackend"
  
  ALTERNATIVE_EMAIL_HOST = 'alternative.host'
  ALTERNATIVE_EMAIL_PORT = '25'

Following settings are not required, if some is not defined or set to None, is used default settings acoording to primary SMTP configuration.

::  
  ALTERNATIVE_EMAIL_HOST_USER = 'username'
  ALTERNATIVE_EMAIL_HOST_PASSWORD = 'password'
  ALTERNATIVE_EMAIL_USE_TLS = False

License
-------

LGPLv3
