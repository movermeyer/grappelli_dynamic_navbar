# grappelli-dynamic-navbar

[![Latest PyPI version](https://img.shields.io/pypi/v/grappelli-dynamic-navbar.svg)](https://crate.io/packages/grappelli-dynamic-navbar/)

[![Number of PyPI downloads](https://img.shields.io/pypi/dm/grappelli-dynamic-navbar.svg)](https://crate.io/packages/grappelli-dynamic-navbar/)


Available features:
* [Header navbar](#navbar)
  
Add a dynamic navbar that change according to user permissions

Add Traslation and addlink.

# Requirements

* Python > 2.6
* django-grappelli >= 2.4.5
* Django >= 1.4

# Installation

* ```pip install grappelli-dynamic-navbar```
* Put ```grappelli_dynamic_navbar``` **before** ```grappelli``` on INSTALLED_APPS.


## settings.py

 * Put 'grappelli_dynamic_navbar' **before** 'grappelli' on INSTALLED_APPS
 * Put 'apptemplates.Loader' on your TEMPLATE_LOADERS setting:

```python
# Your setting will look like:
TEMPLATE_LOADERS = (
    'django.template.loaders.filesystem.Loader',
    'django.template.loaders.app_directories.Loader',
    'apptemplates.Loader',
)
```

 * Be sure 'django.core.context_processors.request' on your TEMPLATE_CONTEXT_PROCESSORS setting:

![Navigation bar](https://github.com/xangmuve/grappelli_dynamic_navbar/blob/master/screenshot.png)


## To run tests

```
pip install -r requirements/tests.txt Django
export DJANGO_SETTINGS_MODULE=grappelli_dynamic_navbar.test_settings
`which django-admin.py` test grappelli_dynamic_navbar"
```

## Contributing

1. Fork it.
2. Create your feature branch. (`git checkout -b my-new-feature`)
3. Commit your changes. (`git commit -am 'Add some feature'`)
4. Push to the branch. (`git push origin my-new-feature`)
5. Create new Pull Request.
