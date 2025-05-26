# Proyecto Final de Ingeniería

Template para el Proyecto Final de Ingeniería en la Universidad Argentina De la Empresa.

## Instalación de entorno en Windows

1. Instalar Miktex.
2. En la consola de Miktex, actualizar.
3. Luego, seleccionar todos los paquetes (ordenar por no instalados) no instalados, e instalarlos.

**Opcional**

1. Instalar LaTeX Workshop en VS Code.
2. Automatizar la compilación de VS Code mediante una carpeta de configuración de VS Code.

## Compilar el PDF

Para generar el documento PDF se debe abrir el cmd, bash o PowerShell en la carpeta donde se encuentra el proyecto. Acto seguido, ejecutar los siguientes comandos:

```shell
$ pdflatex main.tex
$ bibtex main
$ pdflatex main.tex
$ pdflatex main.tex
```

En las diferentes pasadas se van realizando diferentes cambios en el documento, hasta que al ejecutar la última pasada se genera una versión final de dicho documento.

En casos de error se pueden obtener más detalles con `pdflatex -file-line-error -interaction=errorstopmode main`.