# Create Page In Django

In Django if you want to create a new page, you should create new views and then assign the views into the urls. 

## Create Views in Django

open `urls.py` in `web/urls.py`

``` python
# urls.py 

from django.urls import path

...

def home_page(request):
    return 'This is New Views'

urlpatterns = [
    ...
    path('', home_page), # at root path assign home_page views
]

```

and try open browser at `localhost:8000`. You will see the new page that you have created.