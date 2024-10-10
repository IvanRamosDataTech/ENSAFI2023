# ENSAFI2023
La Encuesta Nacional sobre Salud Financiera (ENSAFI) 2023 tiene la finalidad de generar información estadística sobre los aspectos que definen la salud financiera de la población de 18 años y más en el México.

# Instalacion
Este projecto utiliza [Poetry](https://python-poetry.org/docs/basic-usage/) como gestionador de dependencias y paquetes de Python.

El primer paso es instalar pipx, una herramienta que nos permite ejecutar herramientas CLI de python en sus propios entornos virtuales, aislados de los entornos virtuales de otras aplicaciones propias. En este caso; poetry tiene sus propias dependencias y ensefi las suyas. Para evitar una colision de versiones de librerias, siempre es recomendable instalar Poetry a traves de pipx.

in MacOS

$ brew install pipx
$ pipx ensurepath

in Windows
> scoop install pipx
> pipx ensurepath

Luego, instalamos Poetry

$ pipx install poetry
$ poetry --version

Este proyecto ya tiene poetry, pero en caso de querer saber como se genera un proyecto con poetry, puedes ejecutar el siguiente comando
$ poetry new ENSEFI2023 --src

Este es un buen post para seguir las instrucciones de como utilizar poetry
https://realpython.com/dependency-management-python-poetry/

