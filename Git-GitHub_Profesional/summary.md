# Curso Profesional de Git y GitHub

## Sistema de control de versiones

Un sistema de control de versiones permite que en lugar de guardar diferentes versiones de un mismo archivo, guarda solo los cambios que se hicieron sobre el archivo y no solo los cambios si no que también dónde, quién y cuándo.

Git es un sistema de control de versiones (es el más popular) que fue creado por la fundación Linux, particularmente por Linus Torvalds. Es el sistema que maneja el Kernel de Linux.

---

## Flujo de trabajo

### Entorno de desarrollo Personal

- **Directorio de trabajo**: Es la carpeta en donde están tus archivos.
- **Preparación / Staging**: Es el lugar donde enviamos los archivos antes de mandarlos al repositorio local.
- **Repositorio local**: Base de datos de cambios históricos del proyecto.
- **Servidor remoto**: Repositorio remoto donde se encuentra la version unificada del trabajo de diferentes desarrolladores.

## Ramas

Cuando se crea una rama, lo que se hace es crear una copia del último commit en otro lado por lo que los cambios que hagamos no se verán en la rama de dónde partimos.

## README.md

Es un archivo **markdown** y es el que veremos por defecto al entrar a un repositorio. Es una muy buena practica configurarlo para describir el proyecto, los requerimientos y las instrucciones que debemos seguir para contribuir correctamente.

## Cifrado asimétrico

Requiere de una clave pública y una clave privada. La clave pública si utiliza para cifrar los datos y la clave privada si utiliza para descifrar los datos. Esto funciona para mandar mensajes privados entre varios nodos con la lógica de que firmas tu mensaje con una llave pública vinculada con una llave privada que puede leer el mensaje.

### ¿Cómo funciona?

- Ambas partes crean sus llaves públicas y privadas.
- Ambos pueden compartir sus llaves públicas.
- El emisor usa la llave pública de la otra parte para cifrar el mensaje.
- El receptor usa su llave privada para descifrar el mensaje.

---

## ¿Cómo traer una rama a tu repositorio local?

Para traer una rama que no es la rama **main** o **master** a tu repositorio local ejecuta las siguientes comandos...

~~~bash
git fetch origin < nombre de la rama >
~~~

Esto va a traer los datos que haya en dicha rama y para colocar datos en una rama con el mismo nombre ejecutas...

~~~bash
git checkout < nombre de la rama >
~~~

---
