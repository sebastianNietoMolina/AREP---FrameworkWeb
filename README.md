# Promedio y desviación estándar con Lista Enlazada

Este proyecto contiene la implementación del cálculo de promedio y desviación estándar de una muestra poblacional.
El cálculo es presentado en una página web apoyada sobre el framework spark.

## Estado

[![Codacy Badge](https://app.codacy.com/project/badge/Grade/c16d3bb3c8784784ae0c3f10ff88bf78)](https://www.codacy.com/manual/alejovasquero/AREP---FrameworkWeb?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=alejovasquero/AREP---FrameworkWeb&amp;utm_campaign=Badge_Grade)
[![CircleCI](https://circleci.com/gh/alejovasquero/AREP---FrameworkWeb.svg?style=svg)](https://circleci.com/gh/alejovasquero/AREP---FrameworkWeb)

[Despliegue en heroku](https://frameworkweb.herokuapp.com/)

## Empezando

Estas instrucciones te utilizar la página web, compilar el proyecto y las pruebas.
Las instrucciones se limitan a compilación, ejecución y uso. 

### Prerrequisitos

Para instalar y correr exitosamente este proyecto necesitamos:
*  **Java**
*  **Maven**
*  **Git**

### Instalación

Primeramente vamos a descargar el repositorio en nuestra máquina local, y en la carpeta de 
nuestra preferencia. En consola vamos a digitar el siguiente comando para clonar el repositorio.

```console
git clone https://github.com/alejovasquero/SparkWebApp---AREP
```

Entremos a el directorio del proyecto

```console
cd SparkWebApp
```

Debemos compilar el proyecto, que contiene las clases necesarias para poder correr nuestro
proyecto. Por medio de maven vamos a crear todos los compilables **.class**. Desde consola, y ubicados en la carpeta donde se encuentra
nuestra configuración de maven.

```console
mvn package
```

Ahora que nuestras clases etan compiladas vamos a ejecutar la clase principal para
ver el código en acción : )

## Spark local

Una vez compiladas las clases vamos a correr el proyecto

```console
mvn exec:java -Dexec.mainClass="edu.escuelaing.arep.SparkWebApp"
```

Ahora vamos a entrar a nuestro browser en [localhost:4567/hello](localhost:4567/hello)

## Spark HEROKU

Si queremos hacer uso de la aplicación desde heroku entramos al siguiente [link](https://ancient-dusk-94293.herokuapp.com/hello)

## USO de la aplicación

Vamos a insertar una lista de datos válidos y recibir el resultado:
Una vez en la página /hello, vamos a insertar la lista de datos para cálcular.

![](resources/data.PNG)

Una vez los datos están completos damos en el botón de envío.
Ahora vamos a ser dirigidos a la página de resultados pata validarlos.

![](resources/results.PNG)

## Corriendo las pruebas

Correr las pruebas dentro del proyecto es muy sencillo, 
y lo haremos por medio de una fase de maven, la fase **test**, del ciclo de vida **default**. 

```console
mvn test
```

![](resources/AllTest.PNG)

## Construido con

*  [Maven](https://maven.apache.org/) - Manejo de dependencias
*  [Git](https://git-scm.com/) - Control de versiones
*  [Java](https://www.java.com/es/) - Lenguaje de programación
*  [Spark](http://sparkjava.com/) - Framework de desarrollo web

## Autores

*  **David Alejandro Vasquez Carreño** - *Trabajo inicial* - [alejovasquero](https://github.com/alejovasquero)

## Licencia

Este proyecto está licenciado bajo la licencia del MIT - Vea el [LICENSE.md](LICENSE.md) para más detalles
