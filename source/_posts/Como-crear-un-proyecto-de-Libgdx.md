---
title: Como crear un proyecto de Libgdx.
date: 2023-03-16 18:00:46
tags: Java, Libgdx, Español
categories: Tutorial
cover: ../images/crearProyectoLibgdx/cover.png
---

# Como crear un proyecto con Java y Libgdx.

Para aprender como crear un proyecto de Libgdx, no usaremos el generador oficial de Libgdx, mas bien, usaremos Gdx-Liftoff que nos permitirá usar mas lenguajes y extensiones de terceros. 

Para este ejemplo, crearemos el proyecto de "Pong" que será el juego del siguiente tutorial.

### Descargar OpenJDK

Para descargar e instalar openjdk simplemente lo descargamos de [Temurin](https://adoptium.net/es/temurin/).

![Descarga de Temurin](../images/crearProyectoLibgdx/TemurinPagina.png)

Es importante activar las opciones de: añadir al PATH, asociar .jar y establecer la variable JAVA_HOME.

![Opciones de instalación](../images/crearProyectoLibgdx/OpcionesInstalacionTemurin.png)

### Descargar Gdx-Liftoff

Vamos al repositorio de [Gdx-liftoff](https://github.com/tommyettinger/gdx-liftoff/releases), descargamos el archivo .zip y lo descomprimimos.

![Descargar gdx-liftoff](../images/crearProyectoLibgdx/DescargarGdxLiftoff.png)

### Configurar proyecto

Abrimos Gdx-Liftoff y rellenamos las opciones:

![Primeras opciones de Gdx-liftoff](../images/crearProyectoLibgdx/OpcionesDelGenerado1.png)

1. Título del juego.
2. Dominio y nombre del juego (com.domino.nombredeljuego).
3. Nombre de la clase principal.
4. Carpeta vacía donde se generará el proyecto.
5. Dirección del SDK de Android (No es necesario si no se creara para android).
6. Plataformas para las que se creará el juego.

![Segundas opciones de Gdx-liftoff](../images/crearProyectoLibgdx/OpcionesDelGenerado2.png)
7. Usar otros lenguajes (no usar si se trabaja con HTML y GWT).

![Terceras opciones de Gdx-liftoff](../images/crearProyectoLibgdx/OpcionesDelGenerado3.png)
8. Extensiones oficiales de Libgdx.

![Cuartas opciones de Gdx-liftoff](../images/crearProyectoLibgdx/OpcionesDelGenerado4.png)
9. Extensiones de terceros (en este caso usaremos ShapeDrawer para dibujar formas geometricas). 

### Generar proyecto

Damos clic en "Generate project!", esperamos a que termine y diga "SETUP COMPLETE" y listo.

![Generar proyecto](../images/crearProyectoLibgdx/GenerarProyecto.png)

### Probar proyecto
Vamos a los Tasks de Gradle > lwjgl3 > application > run.

![Probar proyecto Task](../images/crearProyectoLibgdx/ProbarProyectoEscritorio.png)
![Probar proyecto ventana](../images/crearProyectoLibgdx/ProbarProyectoEscritorio2.png)


### Compilar proyecto

Para generar un .jar para escritorio vamos a:

Tasks de Gradle > lwjgl3 > Tasks > build > jar.

![Compilar escritorio](../images/crearProyectoLibgdx/CompilarJar.png)

Para compilar para HTML vamos a:

Tasks de Gradle > html > Tasks > other > dist.

![Compilar HTML](../images/crearProyectoLibgdx/CompilarHTML.png)

### Despedida

Espero que te haya ayudado a crear tu proyecto de Ligdx de una manera fácil y entendible, si tienes alguna duda o sugerencia no dudes en comentar 😁

Bueno, me piro vampiro, ten un buen dia.