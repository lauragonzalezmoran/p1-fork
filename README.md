
# Memoria de la Práctica 1
## Introducción

En esta primera práctica nos sumergimos en el mundo de **Git** y **Github**, dos herramientas esenciales en el desarrollo de software colaborativo. A través de una serie de pasos cuidadosamente diseñados, exploramos los comandos fundamentales de Git, como `clone`, `status`, `add`, `commit`, `push`, y `checkout`. Estos comandos son pilares fundamentales para el control de versiones y la colaboración eficiente en proyectos de  desarrollo de software. Además, pusimos en práctica el concepto de *"forking"* en GitHub, permitiéndonos trabajar en nuestro propio espacio de trabajo antes de contribuir a proyectos compartidos. A medida que avanzamos, también nos adentramos en el entorno de desarrollo Java, instalando herramientas clave como **Java 17** y **Maven** que serán necesarias en prácticas posteriores. 

 ## Desarrollo de la Práctica
En el contexto del desarrollo de la práctica, las instrucciones pertinentes se encontraban alojadas en el repositorio [gitt-3-pat/p1](https://github.com/gitt-3-pat/p1). Considerando que el objetivo no es reflejar los cambios en este repositorio original, se llevó a cabo la creación de una duplicación del repositorio bajo el Github ID correspondiente. En este caso, la duplicación se realizó bajo mi identificador [lauragonzalezmoran](https://github.com/lauragonzalezmoran/).Esta duplicación proporciona la ventaja de realizar la práctica en un entorno de trabajo personal. Para llevar a cabo este proceso, se utilizó la función "fork" disponible en la plataforma GitHub, como se muestra en la Imagen 1. Al nuevo repositorio resultante se le asignó el nombre "p1-fork".
>Imagen 1: Opción de Fork 
><img width="923" alt="image" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/c9b9e644-ba80-4ea0-89c6-bd5ef723a4a6">

Una vez completado el fork, se obtiene un nuevo repositorio en la cuenta de GitHub en la nube. No obstante, para realizar el trabajo en este repositorio, es esencial crear una copia del proyecto en la máquina local. Para ello, se generará un CodeSpace y, tras abrir el terminal, se ejecutará el comando `git clone` https://github.com/lauragonzalezmoran/p1-fork. Esta acción permite trabajar en modo *offline*, realizar pruebas sin afectar al repositorio en la cuenta personal de GitHub.

El siguiente paso implica realizar modificaciones en el repositorio local. Esto llevará a que la versión del repositorio en https://github.com/lauragonzalezmoran/p1-fork y la máquina local ya no estén sincronizadas. Por lo tanto, se recurrirá a los comandos de Git para actualizar el repositorio en la nube cuando sea necesario. En este escenario, la modificación conllevará la creación de un archivo llamado *git.txt*. Para lograr esto, se empleará el comando `nano git.txt`. Se introducirá cualquier texto en este archivo y, para visualizar su contenido, se utilizará el comando `cat git.txt`, tal como se ilustra en la Imagen 2 a continuación:
>Imagen 2: Creación y Lectura de Fichero
> <img width="650" alt="Captura de pantalla 2024-01-23 100007" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/feba6704-23d5-421a-906b-86e6d2139837">





## Explicación de los comandos de Git empleados 


## ¿Como probar en la nube?

[Github-Codespaces](https://github.com/features/codespaces)

## Comandos git básicos

```
git clone https://github.com/gitt-3-pat/p1
git status
git add .
git commit -m "TU MENSAJE"
git push

git checkout -b feature/1
git checkout main
```

## ¿Cómo escribir un README.md con formato?

[Github Markdown](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
