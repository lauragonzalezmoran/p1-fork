
# Memoria de la Práctica 1
## Introducción

En esta primera práctica nos sumergimos en el mundo de **Git** y **Github**, dos herramientas esenciales en el desarrollo de software colaborativo. A través de una serie de pasos cuidadosamente diseñados, exploramos los comandos fundamentales de Git, como `clone`, `status`, `add`, `commit`, `push`, y `checkout`. Estos comandos son pilares fundamentales para el control de versiones y la colaboración eficiente en proyectos de  desarrollo de software. Además, pusimos en práctica el concepto de *"forking"* en GitHub, permitiéndonos trabajar en nuestro propio espacio de trabajo antes de contribuir a proyectos compartidos. A medida que avanzamos, también nos adentramos en el entorno de desarrollo Java, instalando herramientas clave como **Java 17** y **Maven** que serán necesarias en prácticas posteriores. 

 ## Desarrollo de la Práctica
 ### Git y Github
En el contexto del desarrollo de la práctica, las instrucciones pertinentes se encontraban alojadas en el repositorio [gitt-3-pat/p1](https://github.com/gitt-3-pat/p1). Considerando que el objetivo no es reflejar los cambios en este repositorio original, se llevó a cabo la creación de una duplicación del repositorio bajo el Github ID correspondiente. En este caso, la duplicación se realizó bajo mi identificador [lauragonzalezmoran](https://github.com/lauragonzalezmoran/). Esta duplicación proporciona la ventaja de realizar la práctica en un entorno de trabajo personal. Para llevar a cabo este proceso, se utilizó la función "fork" disponible en la plataforma GitHub, como se muestra en la Imagen 1. Al nuevo repositorio resultante se le asignó el nombre "p1-fork".
>Imagen 1: Opción de Fork 
><img width="923" alt="image" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/c9b9e644-ba80-4ea0-89c6-bd5ef723a4a6">

Una vez completado el fork, se obtiene un nuevo repositorio en la cuenta de GitHub en la nube. No obstante, para realizar el trabajo en este repositorio, es esencial crear una copia del proyecto en la máquina local. Para ello, se generará un CodeSpace y, tras abrir el terminal, se ejecutará el comando `git clone` https://github.com/lauragonzalezmoran/p1-fork. Esta acción permite trabajar en modo *offline*, realizar pruebas sin afectar al repositorio en la cuenta personal de GitHub.

El siguiente paso implica realizar modificaciones en el repositorio local. Esto llevará a que la versión del repositorio en [lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork) y la máquina local ya no estén sincronizadas. Por lo tanto, se recurrirá a los comandos de Git para actualizar el repositorio en la nube cuando sea necesario. En este escenario, la modificación conllevará la creación de un archivo llamado *[git.txt](./git.txt)*. Para lograr esto, se empleará el comando `nano git.txt`. Se introducirá cualquier texto en este archivo y, para visualizar su contenido, se utilizará el comando `cat git.txt`, tal como se ilustra en la Imagen 2 a continuación:
>Imagen 2: Creación y Visualización del Fichero *[git.txt](./git.txt)*
> <img width="650" alt="Captura de pantalla 2024-01-23 100007" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/feba6704-23d5-421a-906b-86e6d2139837">

Es crucial destacar que los cambios realizados en la máquina local aún no han sido reflejados en el repositorio personal en la nube, es decir, el archivo *[git.txt](./git.txt)* no figura aún en [lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork), como se muestra en la Imagen 3:

> Imagen 3: Estado actual del repositorio [lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork)
> <img width="940" alt="Captura de pantalla 2024-01-23 100035" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/06699859-8ccc-488a-8f2b-d21f7600e88e">

Por ende, una vez satisfechos con los cambios en la máquina local, es esencial propagarlos al repositorio en la nube mediante los comandos `git add .`, `git commit -m "MENSAJE"` y `git push origin main`, entre otros.

En el estado actual, los cambios no están registrados en el *staging area*, lo cual puede verificarse con el comando `git status`:

> Imagen 4: Estado actual del área de preparación (*staging area*)
> <img width="681" alt="Captura de pantalla 2024-01-23 100116" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/533e9cec-1ada-4e24-99df-decf5e4fad93">

El *staging area* es el espacio donde se registran los cambios listos para ser commiteados. Para añadirlos, se utiliza el comando `git add git.txt`:

> Imagen 5: Nuevo estado del área de preparación (*staging area*)
> <img width="688" alt="Captura de pantalla 2024-01-23 100200" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/b61689da-0a65-4d12-960c-7f9759728c85">

Después de ejecutar este comando, el archivo *[git.txt](./git.txt)* se incluye en el *staging area*. Posteriormente, se utiliza el comando `git commit -m "MENSAJE"` para confirmar los cambios y registrarlos en el historial del repositorio:

> Imagen 6: Confirmación de cambios
> <img width="676" alt="Captura de pantalla 2024-01-23 100251" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/cd3c1d81-b7b6-40d2-b5a3-e9d311adf992">
> <img width="667" alt="Captura de pantalla 2024-01-23 100424" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/2853be52-50bf-410d-a5da-349e7585c475">

Finalmente, se envían los cambios de la rama main al repositorio remoto personal [lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork) mediante el comando `push origin main` para poder visualizar los cambios desde GitHub. 
>Imagen 7 : Push Changes
><img width="674" alt="Captura de pantalla 2024-01-23 100452" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/cc169b13-5ac7-449d-a036-61ae964317de">
><img width="949" alt="Captura de pantalla 2024-01-23 100508" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/25845179-48fb-431e-8ea2-efb1e56bf227">

En esta última imagen se puede comprobar cómo el fichero *[git.txt](./git.txt)* se ha añadido correctamente al repositorio personal [lauragonzalezmoran/p1-fork](https://github.com/lauragonzalezmoran/p1-fork), por lo que, ahora sí, no existe ninguna diferencia entre nuestra máquina local y este. Esto también podríamos confirmarlo mediante `git status` como se ha hecho anteriormente.


### Explicación de los comandos de Git empleados

- `git clone`: Este comando se utiliza para clonar un repositorio existente. Al realizar un `git clone`, se crea una copia local del repositorio en la máquina del usuario, permitiendo así contribuir al proyecto.

- `git status`: Proporciona información sobre el estado actual del repositorio. Al ejecutar este comando, se obtiene una visión general de los cambios pendientes, los archivos modificados y otros detalles relevantes.

- `git add .`: Agrega todos los cambios realizados en el directorio de trabajo al área de preparación (*staging area*), preparándolos para ser confirmados en el próximo commit.

- `git commit -m "MESSAGE"`: Este comando registra los cambios realizados en el área de preparación en el historial del repositorio. El mensaje proporciona información sobre la naturaleza de los cambios realizados.

- `git push origin main`: Envía los cambios confirmados en la rama local "main" al repositorio remoto en GitHub. Esto actualiza la versión remota con los últimos cambios locales.

- `git checkout`: Permite cambiar entre ramas o versiones anteriores del código. Es útil para explorar diferentes ramas de desarrollo o revertir a versiones anteriores del proyecto.

  ### Entorno de Desarrollo Java

  El último paso de la práctica consiste en instalar herramientas que serán necesarias para futuras prácticas. A continuación, se deja evidencia de todas:
  
<img width="839" alt="Captura de pantalla 2024-01-28 173811" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/1a74dbaf-d52c-45c1-8886-716162bf0cd9">
<img width="854" alt="Captura de pantalla 2024-01-28 180143" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/35bd900b-cd56-47ea-b35e-909857466ea2">
<img width="493" alt="Captura de pantalla 2024-01-28 180252" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/38ec7d61-9909-4c39-a6aa-a66f48b5e178">
<img width="955" alt="Captura de pantalla 2024-01-28 180523" src="https://github.com/lauragonzalezmoran/p1-fork/assets/122973125/2b654c10-10c0-4399-aead-a73254c63914">






