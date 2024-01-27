
# Memoria de la Práctica 1
## Introducción

En esta primera práctica nos sumergimos en el mundo de **Git** y **Github**, dos herramientas esenciales en el desarrollo de software colaborativo. A través de una serie de pasos cuidadosamente diseñados, exploramos los comandos fundamentales de Git, como `clone`, `status`, `add`, `commit`, `push`, y `checkout`. Estos comandos son pilares fundamentales para el control de versiones y la colaboración eficiente en proyectos de  desarrollo de software. Además, pusimos en práctica el concepto de *"forking"* en GitHub, permitiéndonos trabajar en nuestro propio espacio de trabajo antes de contribuir a proyectos compartidos. A medida que avanzamos, también nos adentramos en el entorno de desarrollo Java, instalando herramientas clave como **Java 17** y **Maven** que serán necesarias en prácticas posteriores. 

 ## Desarrollo de la Práctica
Dado que las indicaciones para la realización de la práctica se encontraban en el repositorio [gitt-3-pat/p1](https://github.com/gitt-3-pat/p1) y considerando que no se pretende reflejar los cambios en este repositorio, la primera acción consistió en crear una duplicación del repositorio bajo mi propio Github ID, que es [lauragonzalezmoran](https://github.com/lauragonzalezmoran/). Esta duplicación facilitará la ejecución de la práctica desde mi propio entorno de trabajo personal.  Para llevar a cabo esta duplicación, utilicé la opción "fork" disponible en la plataforma GitHub (Imagen 1) , y al nuevo repositorio resultante le asigné el nombre *"p1-fork"*. 
>Imagen 1: Opción de Fork 
<img width="923" alt="image" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/c9b9e644-ba80-4ea0-89c6-bd5ef723a4a6">
> [!NOTE]
> Esta misma acción podría haberse realizado desde el terminal, mediante el comando git clone
Una vez realizado el fork, ya tenemos un nuevo repositorio en nuestra cuenta de github en la nube. Sin embargo, para poder trabajar sobre este repositorio, será necesario hacer una copia del proyecto completo en mi máquina local. Para ello, utilizaremos el comando git `clone`



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
