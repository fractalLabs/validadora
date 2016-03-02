# Validadora

La validadora es un proyecto que permite el análisis de recursos de datos y la identificaciones de posibles problemas de estructura, formato o estandarización.
Todo esto a través de un API que permiten crear validaciones asíncronas y consultar su estado ya sea por medio del identificador de la validación o definiendo URL a donde será notificado cuando termine la validaciones.

[![Stories in Ready](https://badge.waffle.io/mxabierto/validadora.png?label=ready&title=Ready)](https://waffle.io/mxabierto/validadora)

## Instalación

La validadora tiene dos formas de instalación, una es como un paquete normal de Python y la otra como contenedor.

En cualquier opción que desees seguir, necesitaras clonar el repositorio:

```console
git clone  http://github.com/mxabierto/validadora
```

### Paquete de Python

Se recomienda el uso de `virtualenvs` para la instalación y en especial si se desea contribuir al proyecto.

```console
python setup.py install
```

### Adicional

 También proveemos `playbooks` y un `Vagrantafile` para crear un ambiente de pruebas.
 Consultalo en la wiki.

### Contenedor

Necesitaras instalar Docker, en el caso de Mac o Windows hacer uso de `boot2docker` para poder construir el contenedor.

```console
docker build -t mxabierto/validadora .
```

## Uso

Si has elegido la opción del paquete de Python puedes levantar una instancia de la aplicación con:

```console
python bin/run.py
```

Pero si tu opción fue Docker, necesitas enlazar tu carpeta temporal a manera que podemos compartir los datasets entre los validadores.

```console
docker run -v /tmp:/datasets -p 5000:5000 mxabierto/validadora
```

## Demo

Puedes visualizar un demo del proyecto [aqui](http://10.15.9.12:5000/).

## ¿Preguntas o problemas?

Encuentra mas información en [el wiki](https://github.com/mxabierto/validadora/wiki)

Mantenemos la conversación del proyecto en [la página de issues (problemas)](https://github.com/mxabierto/validadora/issues). Si tienes otra pregunta, nos puedes contactar a escuadron@datos.gob.mx

## Contribuye

Queremos que este proyecto sea el resultado de un esfuerzo de [la comunidad](https://github.com/mxabierto/validadora/graphs/contributors). [Ayúdanos con código, ideas y bugs](https://github.com/mxabierto/validadora/issues).

## Licencia

[Libre Uso MX (compatible con Creative Commons)](http://datos.gob.mx/libreusomx/)
