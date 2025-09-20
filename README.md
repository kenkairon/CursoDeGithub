# Curso de Git y GitHub

Este repositorio contiene ejemplo y pasos básicos para aprender a trabajar con **Git** y **GitHub**

![GitHub Repo stars](https://img.shields.io/github/stars/kenkairon/CursoDeGithub)

---

## 📌 Software Necesario

[Visual Studio Code](https://code.visualstudio.com/) 
[Git](https://git-scm.com/) 

---

## 🐙 ¿Qué es Git

***Git** Es Software de control de versiones diseñado por ***Linus Torvals***.
Permite gestionar el historial de un proyecto, trabjar en equipo y mantener la calidad del código

### ✅ Beneficios de Git
- Trabajo en Equipo más organizado
- Manejos de Calidad  y Control de Cambios
- Creación de ramas para desarrollar sin afectar el código principal

---

##  📂 Repositorios
Un repositorio es el proyecto con todos los archivos y su historial
Puede estar disponible en servicio online **GitHUb, Bitbucket, Gitlab**.
Normalmente trabajamos con una **copia local** en nuestro equipo.

---

## 🚀 Primeros pasos Git 

### Crear cuenta en GitHub 
👉 [Registrarme en GitHub](https://github.com/)


### Crear un nuevo repositorio
1. En GitHub, haz clic en **New**`
2. Nombre: `nuevoRepositorio`
3. Descripción: *Clase de Git*
4. Clic en ***Create repository***
5. Abrir la terminal en VSCode con :
  ```sh
    code .
  ```


##  🔧Verificar instalación

```sh
git -v 
```
## Crear un archivo de prueba:

```sh
touch ejemplo.html
```

```html
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

## ⚙️ Configuración inicial de Git
```sh
git config --global user.name "kenkairon"
git config --global user.email "ingeinfo2006@gmail.com”
```

## 📥 Flujo básico de Git
```sh
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

## 📊 Comandos informativos

```sh
git fech 
git status
```

## 🔄 Clonar un repositorio existente

```sh
git clone https://github.com/nolimits4web/swiper
```

## Caso Específico

#### Deshacer el último commit pero conservar los cambios en los archivos
```sh
git reset --soft HEAD~1
```
#### Deshacer el último commit y también quitarlo del área de staging
```sh
git reset --mixed HEAD~1
```
#### Deshacer el último commit y borrar también los cambios en los archivos
```sh
git reset --hard HEAD~1
```

## Plugins

| Plugin | README |
| ------ | ------ |    
| GitHub | [plugins/github/README.md][PlGh] |



