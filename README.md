# django_jqgrid

Responsável por gerar o crud usando no front end o plugin jquery-Jqgrid

&nbsp;
### Pré requisito

- Python 3.5+
- Django 1.9+

&nbsp;
### Instalação

1- Adicionar na instalção do django o app django_jqgrid
```
INSTALLED_APPS = [
    'django_jqgrid',
]
```

2 - inserir no urls.py o path sentando para view do django_jqgrid.
```
from django_jqgrid.views import TableView

urlpatterns = [
    path('django-jqgrid/', TableView.as_view(), name="django_jqgrid")
]
```

3 - Gerar o html o usando o jqGrid da maneira desejada, mas você deve utilizar o arquivo
django_jqgrid/templates/example.html como exemplo para configurar o plugin jquery.
