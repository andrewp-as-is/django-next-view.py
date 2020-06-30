<!--
https://readme42.com
-->


[![](https://img.shields.io/pypi/v/django-next-view.svg?maxAge=3600)](https://pypi.org/project/django-next-view/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/django-next-view.py/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/django-next-view.py/actions)

### Installation
```bash
$ [sudo] pip install django-next-view
```

#### Examples
```python
from django_next_view.views import NextViewMixin

class MyView(NextViewMixin,...):
    def post(self,request,*args,**kwargs):
        ...
        return self.next()
```

add `next` arg to forms/links
```html
<form action="..." method="POST">
<input type="hidden" name="next" value="url" />
</form>

<a href="{% url 'view_name' %}?next=url">GET</a>
```

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>