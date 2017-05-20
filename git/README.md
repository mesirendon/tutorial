# Tutorial de Git

En este tutorial vamos a ver los conceptos básicos de Git.

Las herramientas para desarrollar este contenido son:

* [Git](https://git-scm.com)
* [GitKraken](http://www.gitkraken.com)

## Instalación en Windows

* Descargar Git para su arquitectura (32 o 64 bits).
* Instalar Git Bash
  * Ejecutar
  * Sí
  * Next >
  * Next >
  * Seleccionar todo, Next >
  * Next >
  * Next >
  * Next >
  * Next >
  * Next >
  * Enable symbolic links, Next >
  * Finish
* Crear llaves ssh
  * `ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`
  * Enter
  * Password 1
  * Password 2
  * `eval $(ssh-agent -s)`
  * `ssh-add ~/.ssh/id_rsa`
* Agregar llaves a GitHub
  * `clip < ~/.ssh/id_rsa.pub`
  * Pegar llave pública en GitHub
* Probar integración de llave
  * `ssh -T git@github.com`
  * Escribir `yes` y Enter
* Clonar este repositorio
  * `git clone git@github.com:mesirendon/tutorial.git`

## Instalación en Linux

```bash
$ sudo apt-get install git-core
```
