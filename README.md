# 🧠 Fundamentos de Git y GitHub

Este repositorio contiene ejemplo y pasos básicos para aprender a trabajar con **Git** y **GitHub**

![GitHub Repo stars](https://img.shields.io/github/stars/kenkairon/CursoDeGithub)

---

# 🎯 Objetivo de Clase 
Introducir los conceptos fundamentales de Git y GitHub, explicar la utilidad en el desarrollo 
colaborativo, y practicar el flujo básico de trabajo  con repositorios locales y remoto

## 📌 Herramientas Necesarias

- Editor de Codigo [Visual Studio Code](https://code.visualstudio.com/) 
- Terminal: PowerShell, Terminal(Windows), iTerm(Mac), terminal estandar(Linux)
- Git: Sistema de Control de Versiones Descargar desde [Git](https://git-scm.com/) 

---

## 🐙 ¿Qué es Git

***Git** Es Software de control de versiones diseñado por ***Linus Torvals***.
Permite gestionar el historial de un proyecto, trabjar en equipo y mantener la calidad del código

***Resuelve problemas como:***
- Manejo de versiones (“final_final_v2”)
- Historial de cambios
- Autoría de líneas de código
- Reversión de errores

### ✅ Beneficios de Git
- Trabajo en Equipo más organizado
- Manejos de Calidad  y Control de Cambios
- Creación de ramas para desarrollar sin afectar el código principal

---

## 🌐 ¿Qué es GitHub?
Plataforma para alojar repositorios Git
Funciona como red social profesional para desarrolladores
Permite compartir, revisar y colaborar en proyectos
Repositorios pueden ser públicos o privados

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

## Crea archivo html
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
---
## 📥 Traer cambios del repositorio remoto
### 1. Verificar si hay cambios disponibles
Para consultar si existen actualizaciones en el repositorio remoto sin descargarlas aún, utiliza el siguiente comando:
```sh
git fetch
```
### 2. Descargar cambios
Para traer los cambios del repositorio remoto y fusionarlos con tu rama local actual, utiliza el siguiente comando:
```sh
git pull
```
### 3. Ver estado actual
Para revisar el estado del repositorio y ver qué archivos han sido modificados, agregados o están listos para confirmar, utiliza el siguiente comando:
```sh
git status
```
## 🧪 Revertir cambios y ver historial
### 1. Ver historial de commits
Para consultar el historial de cambios realizados en el repositorio, utiliza el siguiente comando:
```sh
git log
```
### 2. Revertir un commit específico
Si necesitas deshacer un cambio que ya fue confirmado, puedes revertir un commit específico utilizando su identificador SHA:
```sh
git revert SHA
```
Reemplaza SHA por el código único del commit que deseas revertir (puedes obtenerlo con git log).
Este comando no elimina el commit original, sino que crea uno nuevo que revierte sus efectos.

---

🔄 Clonar un repositorio existente

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
---
## 📚 Glosario técnico

| Término        | Definición                                                   |
|----------------|--------------------------------------------------------------|
| Repositorio    | Carpeta que contiene todos los archivos y el historial de cambios |
| Commit         | Registro de cambios con mensaje y autoría                     |
| Push           | Envío de cambios al repositorio remoto                        |
| Pull           | Descarga de cambios desde el repositorio remoto               |
| Fetch          | Consulta de cambios disponibles sin descargarlos              |
| Stage          | Área de preparación antes de confirmar cambios                |
| Fork           | Copia de un repositorio para modificarlo sin afectar el original |
| GitHub Actions | Automatizaciones que se ejecutan sobre el código              |
