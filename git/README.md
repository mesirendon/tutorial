# Tutorial de Git

En este tutorial vamos a ver los conceptos básicos de Git.

Las herramientas para desarrollar este contenido son:

* [Git](https://git-scm.com)
* [GitKraken](http://www.gitkraken.com)
* Explicación de [`git-flow`](http://danielkummer.github.io/git-flow-cheatsheet/).

## Concepto
Git es un sistema de control de versiones distribuido libre y de código abierto, diseñado para gestionar versiones de software en equipos de diversos tamaños.

![Zones](https://git-scm.com/book/en/v2/images/areas.png)

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

## Configuración
```bash
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
# En Linux
git config --global core.editor vim
# En windows
git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -nosession"
```
