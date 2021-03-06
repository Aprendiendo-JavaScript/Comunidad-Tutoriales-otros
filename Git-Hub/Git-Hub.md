# Cómo colaborar en un proyecto en GitHub

*   Fork del repositorio original a nuestra cuenta
*   Clonar el repositorio del fork a nuestra PC
*   Actualizar la rama maestra usada en el repositorio original.
*   Crear una rama nueva en nuestro repositorio local.
*   Hacer los cambios
*   Hacer un Pull Request

## Fork del repositorio original a nuestra cuenta

El primer paso es hacer "Fork" del repositorio.

## Clonar el repositorio del fork a nuestra PC

Después de tener el repositorio en nuestra cuenta, seleccionar la dirección del repositorio "SSH o HTTP" y clonar:

`$ git clone https://github.com/User/NombreRepo.git`

Dentro de la carpeta que genera, comprobar la URL del repositorio:

`$ git remote -v`

Antes de realizar modificaciones agregar la URL del repositorio original del proyecto:

`$ git remote add upstream https://github.com/User/RepoOriginal(Forkeado)`

Comprobar

`$ git remote -v`

## Actualizar la rama maestra usada en el repositorio original.

Antes de empezar a trabajar, obtener los últimos cambios del Repo Original de la rama de desarrollo ("develop"):

`$ git fetch upstream rama-develop` o `$ git pull upstream rama-develop`

## Crear una Rama nueva en nuestro repositorio local.

Para crear una rama usar la opción "checkout" de git:

`$ git checkout -b feature-nombre-rama`

## Hacer cambios

Realizar todos los cambios que se desea hacer al proyecto.

Agregar los archivos y hacer un commit

`$ git add .`

`$ git commit -m "Mensaje descriptivo"`

Después de realizar el commit hacer el push hacia nuestro repositorio indicando la rama que hemos creado.

`$ git push origin feature-nombre-rama`

## Hacer un Pull Request

Hacer click en "New Pull Request"

Seleccionar las Ramas a comprar, que son la rama creada local y la rama develop del repositorio forkeado (upstream).

Si todo está bien, enviar con el botón "Create Pull Request".

Esperar a que los encargados del repositorio lo revisen, acepten y mezclen en la rama correspondiente.

>*Nota: No olvidar que la nomenclatura de varios pasos expuestos aquí se encuentran en el documento [CONTRIBUTING.md](CONTRIBUTING.md)*

<br/><br/><br/><br/>

Este documento esta basada de la guía que se encuentra en: [BCasal/Colaborar Proyecto GitHub.markdown](https://gist.github.com/BCasal/026e4c7f5c71418485c1). __*Muchas Gracias*__!