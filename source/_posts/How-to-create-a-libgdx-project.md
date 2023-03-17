---
title: How to create a libgdx project.
date: 2023-03-17 16:20:09
tags: Java, Libgdx, English
categories: Tutorial
cover: ../images/crearProyectoLibgdx/cover.png
---

# How to create a project with Java and Libgdx.

To learn how to create a Libgdx project, we won't use the official Libgdx generator, rather, we'll use Gdx-Liftoff which will allow us to use more third-party languages and extensions. 

For this example, we will create the "Pong" project that will be the game for the next tutorial.

### Download OpenJDK

To download and install openjdk we simply download it from [Temurin](https://adoptium.net/es/temurin/).

![Temurin's Download](../images/crearProyectoLibgdx/TemurinPagina.png)

It is important to activate the options: add to the PATH, associate .jar and set the JAVA_HOME variable.

![Installation Options](../images/crearProyectoLibgdx/OpcionesInstalacionTemurin.png)

### Download Gdx-Liftoff

Let's go to the repository [Gdx-liftoff](https://github.com/tommyettinger/gdx-liftoff/releases), we download the .zip file and unzip it.

![Download gdx-liftoff](../images/crearProyectoLibgdx/DescargarGdxLiftoff.png)

### Configure Project

We open Gdx-Liftoff and fill in the options:

![Gdx-liftoff First Options](../images/crearProyectoLibgdx/OpcionesDelGenerado1.png)

1. Game title.
2. Domain and game name (com.domino.gamename).
3. Name of the main class.
4. Empty folder where the project will be generated.
5. Android SDK address (Not required if not built for android.)
6. Platforms for which the game will be created.

![Gdx-liftoff Second Options](../images/crearProyectoLibgdx/OpcionesDelGenerado2.png)
7. Use other languages (do not use if you work with HTML and GWT).

![Gdx-liftoff Third Options](../images/crearProyectoLibgdx/OpcionesDelGenerado3.png)
8. Official Libgdx extensions.

![Gdx-liftoff Fourth Options](../images/crearProyectoLibgdx/OpcionesDelGenerado4.png)
9. Third party extensions (in this case we will use ShapeDrawer to draw geometric shapes). 

### Generate Project

We click on "Generate project!", We wait for it to finish and say "SETUP COMPLETE" and that's it.

![Generate Project](../images/crearProyectoLibgdx/GenerarProyecto.png)

### Test Project
Go to Gradle Tasks > lwjgl3 > application > run.

![Test Project Task](../images/crearProyectoLibgdx/ProbarProyectoEscritorio.png)
![Test Project Window](../images/crearProyectoLibgdx/ProbarProyectoEscritorio2.png)


### Compile Project

To generate a .jar for desktop we are going to:

Gradle Tasks > lwjgl3 > Tasks > build > jar.

![Compile Desktop](../images/crearProyectoLibgdx/CompilarJar.png)

To compile for HTML we are going to:

Gradle Tasks > html > Tasks > other > dist.

![Compile HTML](../images/crearProyectoLibgdx/CompilarHTML.png)

### Farewell

I hope it has helped you to create your Ligdx project in an easy and understandable way, if you have any questions or suggestions do not hesitate to comment 😁

Well, see you later, have a good day.