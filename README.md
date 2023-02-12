# **Git**

## **¿Qué es Git**

Git es un sistema de control de versiones de código. Es una herramienta que permite a los desarrolladores mantener un registro de los cambios realizados en su código y colaborar de manera efectiva en proyectos de software.

Por ejemplo, con Git, puedes crear un repositorio que contenga todo el historial de cambios en tu proyecto. Cada vez que realizas un cambio en el código, puedes "comitear" ese cambio al repositorio, lo que permite llevar un registro de ese cambio y revertir fácilmente a versiones previas si es necesario.

Además, Git permite trabajar de manera colaborativa en proyectos de software. Puedes clonar repositorios de otros desarrolladores, hacer tus propios cambios y enviarlos de vuelta al repositorio original como "pull request". Esto permite un flujo de trabajo colaborativo y eficiente para el desarrollo de software.

> "Git is a free and open source distributed version
> control system designed to handle everything
> from small to very large projects with speed and
> efficiency”. [Source](https://git-scm.com)

Entre sus características podremos destacar:

- Control de cambios
- Fácil de usar
- Más útil con archivos de texto
- Gestión de funciones
- Trabajo en equipo
- No hay un servidor real
- Equipos remotos
- Implementación en diferentes entornos
- ¡Moderno y en constante evolución!

## **Instalación**

- Enlaces:
  - [Window](https://git-scm.com/download/win)
  - [Mac](https://git-scm.com/download/mac)
  - [Linux](https://git-scm.com/download/linux)
- Configuración:
  - Define Visaul Studio Code como editor por defecto.
  - Define la rama principal como "main".

## **Comandos básicos**

### Configurar git

- **`git config --global user.name "[name]`**: establecer el nombre que quieres adjuntar en tus commit.
- **`git config --global user.email "[email address]"`**: establecer el email que quieres adjuntar en tus commit.

### Iniciar:

- **`git init [project-name]`**: iniciar un repositorio.
- **`git clone [url]`**: clonar un repositorio.

### Stage & Snapshot:

- **`git init`**: iniciar un repositorio.
- **`git status`**: verificar el repositorio, muestra archivos modificados en el directorio de trabajo y listos para hacer commit.
- **`git add [file]`** or **`git add .`** : agregar un archivo o todos los cambios.
- **`git diff`**: diferencias de lo que ha cambiado pero no está en stage.
- **`git commit -m [menssage]`**: hacer commit de los cambios y agregar un mensaje descriptivo.

### Branch & Merge:

- **`git branch`**: listar las ramas, una \* aparece junto a la rama activa actual..
- **`git branch [branch-name]`**: crear una nueva rama.
- **`git checkout [branch-name]`**: seleccionar una rama.
- **`git checkout -b [branch-2] [branch-1]`**: crear una rama llamada branch-2 a partir de la rama branch-1.
- **`git merge [branch]`**: fusionar la rama especificada en la rama actual.
- **`git log`**: mostrar todos los commits en la rama actual.
- **`git log --oneline`**: mostrar todos los commits en una sola línea.

### Share & update:

- **`git remote add [url]`**: añadir url git.
- **`git push [branch]`**: enviar los commits de la rama local a la rama en el repositorio remoto.
- **`git pull [branch]`**: obtener el último commit de la rama remota.

### Tracking path changes:

- **`git rm [file]`**: borrar el archivo del proyecto.
- **`git mv [existing-path] [new-path]`**: cambiar la ruta del archivo existente y preparar el movimiento

### Rewrite history:

- **`git rebase [branch]`**: aplicar cualquier confirmación del branch actual antes de la especificada.
- **`git reset --hard [commit]`**: limpiar el área de preparación y reescribir el árbol de trabajo a partir del commit especificado.

**Más recursos**:

- [Original documentation](https://git-scm.com/docs)
- [Pro Git book](https://git-scm.com/book/en/v2)
- [Git Cheat Sheets](https://training.github.com/) in different lenguages.

## **Graphical Interfaces**

- [SourceTree](https://www.sourcetreeapp.com)
- [GitKraken](https://www.gitkraken.com)

## **How to do good comments**

There 7 basic rules:

1. Separate subject from body with a blank line.
2. Limit the subject line to 50 characters.
3. Capitalize the subject line.
4. Do not end the subject line with a period.
5. Use the imperative mood in the subject line.
6. Wrap the body at 72 characters.
7. Use the body to explain what and why vs. how.

![How to write a correct commit](https://cbea.ms/content/images/size/w2000/2021/01/git_commit_2x.png)

[Source](https://chris.beams.io/posts/git-commit/)

## **Git-flow Workflow**:

Git flow is a popular Git branching strategy aimed at simplifying release management, and was introduced by software developer Vincent Driessen in 2010. Fundamentally, Git flow involves isolating your work into different types of Git branches.
In the Git flow workflow, there are five different branch types:

- Main: contains production-ready code that can be released.
- Develop: contains pre-production code with newly developed features that are in the process of being tested.
- Feature: it is used when adding new features to your code.
- Release: used when preparing new production releases
- Hotfix: used to quickly address necessary changes in your main branch.
  ![Git flow](https://www.gitkraken.com/wp-content/uploads/2021/03/git-flow-4.svg)
  [Source](https://www.gitkraken.com/learn/git/git-flow)

### **Steps for basic Git-flow**:

1.  **Main** branch is only for client not for develop.
2.  Create a **"develop"** branch.
3.  New feature branch -> branch [feature-name].
4.  When the feature is finished, **merge with develop**.
5.  All features are ready, **merge with main**, add a tag/release.

En resumen, podríamos decir que Git es una herramienta esencial para cualquier desarrollador de software que desee llevar un control de versiones y colaborar de manera efectiva en proyectos de software.
