<!--
https://readme42.com
-->


[![](https://img.shields.io/pypi/v/django-embed-gist.svg?maxAge=3600)](https://pypi.org/project/django-embed-gist/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/django-embed-gist.py/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/django-embed-gist.py/actions)

### Installation
```bash
$ [sudo] pip install django-embed-gist
```

#### Pros
+   native (html links)

#### How it works
input:
```html
<a href="https://gist.github.com/user/id" target="_blank">title</a>
```

output:
```html
<script src="https://gist.github.com/user/id.js"></script>
```

##### `settings.py`
```python
INSTALLED_APPS+= [
    'django_embed_gist'
]
```

#### Examples
```html
{% load embed_gist %}

{{ post.body|embed_gist|safe }}
```

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>