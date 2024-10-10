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

# Trabajando con Poetry

Para Visualizar todos los entornos virtuales que Poetry administra en tu proyecto
$ poetry env list

Para checar el entorno virtual actual en el que Poetry esta trabajando
$ cd  src/ensafi2023 
$ poetry env info --path

Podemos utilizar la herramienta de entornos virtuales de Poetry para crear differentes entornos virtuales con differentes configuraciones y versiones de Python para probar nuestra applicacion bajo diferentes circunstancias.
Para crear un entorno vitual que será administrado automaticamente por Poetry, ejecutamos el siguiente comando
$ poetry env use python3

El entorno virtual será almacenado en el folder Caches/pypoetry de la instalacion global de Poetry en el sistema

Para cambiar de entorno virtual manejado por Poetry
poetry env use python

Para eliminar todos los entornos virtuales asociados a tu proyecto, ejecuta el siguiente comando
$ poetry env remove --all