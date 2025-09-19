## Software Necesario

Requeridos1 [vscode](https://code.visualstudio.com/) 
Requeridos2 [GitHub](https://git-scm.com/) 

## git
Software de control de versiones diseñado por Linus Torvals

## Beneficios de Git
Trabajo en Equipo 
Manejos de Calidad Trabajando a través de Ramas

## Repositorios
El proyecto con todos los archivos "originales"
Disponible online = GitHUb, Bitbucket, Gitlab
Trabajamos con una copia

## Git 
Nuevo Repositorio
Clonar Repositorio

Crear Cuenta [Github](https://github.com/)

## Nuevo Repositorio

```sh
Botón de new 
kenkairon/nuevoRepositorio
Descripción = Clase de Git 
create repository
Abrimos terminal en code .
```

## Verificamos si esta instalado

```sh
git -v 
touch ejemplo.html
```
```sh
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejemplo de HTML para Git</title>
</head>
<body>
    <h1>Estoy aprendiendo Git</h1>
</body>
</html>
```

```sh
git config --global user.name "kenkairon"
git config --global user.email "ingeinfo2006@gmail.com”
git init 
git add ejemplo.html
git commit -m "Agregar ejemplo"
git branch -M main
git remote add origin https://github.com/kenkairon/CursoDeGithub"
git push -u origin main
```
## Comprobar que estamos en el archivo remoto que asignamos

```sh
git remote -v
```

## Caso Específico

### Deshacer el último commit pero conservar los cambios en los archivos
```sh
git reset --soft HEAD~1
```
### Deshacer el último commit y también quitarlo del área de staging
```sh
git reset --mixed HEAD~1
```
### Deshacer el último commit y borrar también los cambios en los archivos
```sh
git reset --hard HEAD~1
```

## Plugins

Dillinger is currently extended with the following plugins.
Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |    
| GitHub | [plugins/github/README.md][PlGh] |
