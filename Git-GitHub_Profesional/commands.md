# Commands for Git

- **git init** - Inicializa en la carpeta un repositorio, la base de datos de cambios de cualquier archivo.
- **git add < nombre del archivo >** - Agrega el archivo a la base de datos de cambios, Git ahora sabe que existe. El o los archivo(s) pasan a *staging*.
- **git add .** - Agrega todos los archivos que hayan cambiado de la carpeta de la que estés.
- **git commit -m "< mensaje >"** - Envía los últimos cambios del archivo a la base de datos del sistema de control de versiones.
- **git status** - Muestra el estado de tu base de datos.
- **git show** - Muestra todos los cambios históricos hechos, incluyendo las líneas de código o texto o las lineas de otros archivos y quién las hizo.
- **git log < nombre archivo >** - Ver la historia de un archivo.
- **git log --stat** - Muestra el log con los cambios específicos hechos en cada archivo.
- **git checkout < hash commit / rama > < nombre de archivo >** - Regresa un archivo a la versión indicada.
- **git reset < hash commit > --soft** - Borra todo el historial y los registros de Git pero se mantienen los cambios que están en Staging Area.
- **git reset < hash commit > --hard** - Borra toda la información de los commits, incluso lo que haya en Staging Area.
- **git reset HEAD** - Saca lo que se encuentra en el Staging Area.
- **git rm < nombre archivo > --cached** -
