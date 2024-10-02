# Clase 05 - git

 ## Para crear un repositorio de git 

 ```sh
 git init
 ```

 ## Ver en qué estados están los archivos y en qué área

 ```sh
 git status
 ```

## Áreas del repositorio de git 

3 áreas

* Working directory (WD): directorio de trabajo donde se van agregando o quitando los archivos durante el desarrollo.
* Staging area (SA): Área de control de cambios. Area temporal/intermedia.
* Local repo (LR): Una caja donde voy a ir teniendo todas las fotos que vaya sacando.

## Estado de los archivos

* untracked: Archivos que estan en el WD pero que GIT no les está dando seguimiento.
* unmodified: Archivos que GIT ya está siguiendo y con respecto al WD, no fueron modificados.
* modified: Archivos que se encuentran en el respositorio (están siendo seguidos por GIT) pero difieren con lo que se encuentra actualmente en el WD.
* staged: Archivos que están en el área temporal/intermedia.

## Agrego al área de confirmación el archivo/archivos

```sh
git add <nombre-archivo>
git add <nombre-archivo> <nombre-archivo> <nombre-archivo>
git add . # agrega todos los archivos 
```

# Persistimos los cambios agregados al área de confirmación en un commit

```sh
git commit -m "mensaje descriptivo de lo que tiene el commit"
```

# Corregir el mensaje del commit

```sh
git commit --amend -m "el mensaje corregido"
```

# Como el timeline de commits

```sh
git log # Versión larga
git log --oneline # Versión corta
```