# Ajax Service

Wraper que automatiza el proceso de configurar los llamados a una base de datos que funciona como un API rest. 

Funciona originalmente con Django Rest Reramewok pudiendo adaptarse a Laravel

El Wraper configura un servicio recibiendo un url y devolviendo el resultado en diferentes modos

Silent- Devuelve los resultados, Sin ninguna información

Console-Devuelve los resultados, e imprime en la consola el status

Loud-Lanza un alert con el status de la respues

Custom- permite proveer un callback para procesar los resultados de forma personalizada



Django Config

Con Django Rest Framework uinstalado preparar el entorno para crear un esquema y tener acceso a el

```shell
$ pip install coreapi pyyaml
```

```python
from rest_framework.schemas import get_schema_view

schema_view = get_schema_view(title='Pastebin API')

urlpatterns = [
    path('schema/', schema_view),
    ...
]
```







#TODO

- [ ] Leer el Schema del servicio ajax en la creación para poder generar un servicio generico que agrupe todas la rutas