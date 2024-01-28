
# Memoria de la Práctica 1
## Introducción

En esta primera práctica nos sumergimos en el mundo de **Git** y **Github**, dos herramientas esenciales en el desarrollo de software colaborativo. A través de una serie de pasos cuidadosamente diseñados, exploramos los comandos fundamentales de Git, como `clone`, `status`, `add`, `commit`, `push`, y `checkout`. Estos comandos son pilares fundamentales para el control de versiones y la colaboración eficiente en proyectos de  desarrollo de software. Además, pusimos en práctica el concepto de *"forking"* en GitHub, permitiéndonos trabajar en nuestro propio espacio de trabajo antes de contribuir a proyectos compartidos. A medida que avanzamos, también nos adentramos en el entorno de desarrollo Java, instalando herramientas clave como **Java 17** y **Maven** que serán necesarias en prácticas posteriores. 

 ## Desarrollo de la Práctica
En el contexto del desarrollo de la práctica, las instrucciones pertinentes se encontraban alojadas en el repositorio [gitt-3-pat/p1](https://github.com/gitt-3-pat/p1). Considerando que el objetivo no es reflejar los cambios en este repositorio original, se llevó a cabo la creación de una duplicación del repositorio bajo el Github ID correspondiente. En este caso, la duplicación se realizó bajo mi identificador [lauragonzalezmoran](https://github.com/lauragonzalezmoran/). Esta duplicación proporciona la ventaja de realizar la práctica en un entorno de trabajo personal. Para llevar a cabo este proceso, se utilizó la función "fork" disponible en la plataforma GitHub, como se muestra en la Imagen 1. Al nuevo repositorio resultante se le asignó el nombre "p1-fork".
>Imagen 1: Opción de Fork 
><img width="923" alt="image" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/c9b9e644-ba80-4ea0-89c6-bd5ef723a4a6">

Una vez completado el fork, se obtiene un nuevo repositorio en la cuenta de GitHub en la nube. No obstante, para realizar el trabajo en este repositorio, es esencial crear una copia del proyecto en la máquina local. Para ello, se generará un CodeSpace y, tras abrir el terminal, se ejecutará el comando `git clone` https://github.com/lauragonzalezmoran/p1-fork. Esta acción permite trabajar en modo *offline*, realizar pruebas sin afectar al repositorio en la cuenta personal de GitHub.

El siguiente paso implica realizar modificaciones en el repositorio local. Esto llevará a que la versión del repositorio en lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork) y la máquina local ya no estén sincronizadas. Por lo tanto, se recurrirá a los comandos de Git para actualizar el repositorio en la nube cuando sea necesario. En este escenario, la modificación conllevará la creación de un archivo llamado *git.txt*. Para lograr esto, se empleará el comando `nano git.txt`. Se introducirá cualquier texto en este archivo y, para visualizar su contenido, se utilizará el comando `cat git.txt`, tal como se ilustra en la Imagen 2 a continuación:
>Imagen 2: Creación y Visualización del Fichero *git.txt*
> <img width="650" alt="Captura de pantalla 2024-01-23 100007" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/feba6704-23d5-421a-906b-86e6d2139837">

Es importante notar como estos cambios realizados en la máquina local todavía no se han extendido al repositorio personal en la nube. Es decir, en este caso, el fichero * git.txt* todavía no aparece en [lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork), tal como se muestra en la Imagen 3: 
>Imagen 3: Pantallazo del estado actual del repositorio [lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork)
><img width="940" alt="Captura de pantalla 2024-01-23 100035" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/06699859-8ccc-488a-8f2b-d21f7600e88e">


Es por esto que, una vez que estemos satisfechos con los cambios llevados a cabo en nuestra máquina local, deberemos conseguir que estos se propaguen a nuestro repositorio en la nube. Para ello, se hará uso de los comandos `git add .`, `git  commit -m "MENSAJE"` y `git push origin main`, entre otros. 

Actualmente los cambios no están registrados en el *staging area* ,lo cual también se puede comprobar con el comando 'git status`: 
>Imagen 4: Current Staging Area
><img width="681" alt="Captura de pantalla 2024-01-23 100116" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/533e9cec-1ada-4e24-99df-decf5e4fad93">

El *staging area* es el lugar donde se registran los cambios listos para ser commiteados. Para añadirlos en este area, utilizaremos el comando `git add git.txt`: 
>Imagen 5: New Staging Area
><img width="688" alt="Captura de pantalla 2024-01-23 100200" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/b61689da-0a65-4d12-960c-7f9759728c85">
Como se puede observar en la Imagen 5, tras ejecutar el comando anterior, hemos incluido el fichero git.txt en el *staging area*. Una vez realizado esto, ya podemos emplear el comando `git commit -m "MENSAJE"` para confirmar los cambios y registrarlos en el historial del repositorio. 
<img width="676" alt="Captura de pantalla 2024-01-23 100251" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/cd3c1d81-b7b6-40d2-b5a3-e9d311adf992">
<img width="667" alt="Captura de pantalla 2024-01-23 100424" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/2853be52-50bf-410d-a5da-349e7585c475">

Por último, se debe enviar los cambios de nuestra rama main al respositorio remoto personal  [lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork) , para poder así visualizar los cambios desde GitHub

<img width="674" alt="Captura de pantalla 2024-01-23 100452" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/cc169b13-5ac7-449d-a036-61ae964317de">

<img width="949" alt="Captura de pantalla 2024-01-23 100508" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/d4ff7774-18cd-4b94-899f-0bb7230affca">

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
