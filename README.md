<!--
https://pypi.org/project/readme-generator/
https://pypi.org/project/python-readme-generator/
https://pypi.org/project/django-readme-generator/
-->

[![](https://img.shields.io/pypi/pyversions/django-embed-gist.svg?longCache=True)](https://pypi.org/project/django-embed-gist/)
[![](https://img.shields.io/pypi/v/django-embed-gist.svg?maxAge=3600)](https://pypi.org/project/django-embed-gist/)
[![Travis](https://api.travis-ci.org/looking-for-a-job/django-embed-gist.py.svg?branch=master)](https://travis-ci.org/looking-for-a-job/django-embed-gist.py/)

#### Installation
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

#### `settings.py`
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
    <a href="https://pypi.org/project/django-readme-generator/">django-readme-generator</a>
</p>