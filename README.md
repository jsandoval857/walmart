# Prueba Full Stack Developer

Esta aplicación esta compuesta por 3 (tres) componentes:

1. la base de datos *mongodb*
2. la api en *node.js* con *expres*
3. la web en *angular 9*

## Ejecutar aplicación

para ejecutar la aplicacón se debe seguir los siguientes pasos:

- clonar repositorio:  `git clone https://github.com/jsandoval857/walmart`
- entrar en la carpeta *walmart*: `cd walmart`
- levantar el stack de la aplicación: `docker-compose up`
- presionar ***ctrl + c*** para detener el stack
- elimine los componentes creados con el siguiente comando: `docker-compose down`

Para ingresar a la *api*, la url es `http://localhost:3000`

Para ingresar a la *web*, la url es `http://localhost:8000`

## Ejecutar las Pruebas del componente web

- entrar en la carpeta *walmart/web*: `cd walmart/web`
- para ejecutar las pruebas ejecutar el siguiente comando: `docker-compose up`
- presionar ***ctrl + c*** para detener las pruebas
- elimine los componentes creados con el siguiente comando: `docker-compose down`
