# Guía de Colaboración del Repositorio

Bienvenido al repositorio del equipo. Para asegurar que todos trabajamos de forma ordenada y sin sobrescribir el código de nuestros compañeros, seguiremos un flujo de trabajo basado en ramas (**GitHub Flow**).

Por favor, lee y sigue estos pasos cada vez que vayas a contribuir al proyecto.

## 1. Configuración Inicial (Solo la primera vez)

1.1 **Clonar el repositorio**: Descarga el código del proyecto a tu máquina local ejecutando el siguiente comando en tu terminal.
`git clone <URL-del-repositorio>`

1.2 **Navegar al directorio**: Entra en la carpeta del proyecto recién clonado.
`cd <nombre-del-repositorio>`

## 2. Flujo de Trabajo Diario (Para cada nueva tarea)

2.1 **Sincronizar la rama principal**: Antes de empezar a programar, asegúrate siempre de tener la **última versión del código** para evitar conflictos.
`git checkout main`
`git pull origin main`

2.2 **Crear una rama de trabajo**: **Nunca trabajes directamente sobre la rama main**. Crea siempre un espacio aislado para tu nueva funcionalidad o corrección. Utiliza nombres descriptivos (por ejemplo: `feature/menu-navegacion` o `bugfix/error-login`).
`git checkout -b <nombre-de-tu-rama>`

2.3 **Guardar los cambios (Commit)**: Una vez que hayas terminado de escribir y probar tu código, empaquétalo en tu ordenador con un mensaje claro que explique las modificaciones.
`git add .`
`git commit -m "Añade una descripción breve pero clara de lo que hace este código"`

2.4 **Subir la rama a GitHub (Push)**: Envía tu rama de trabajo al repositorio remoto para que el resto del equipo tenga acceso a ella.
`git push origin <nombre-de-tu-rama>`

## 3. Revisión e Integración

3.1 **Crear un Pull Request (PR)**: Ve a la página del repositorio en GitHub y haz clic en el botón verde para abrir un **Pull Request**. Describe qué cambios has realizado para que el equipo lo entienda fácilmente.

3.2 **Solicitar revisión**: Espera a que al menos **un miembro del equipo revise tu código**. Si hay sugerencias, realiza los cambios en tu ordenador, haz un nuevo `commit` y un nuevo `push` a tu rama.

3.3 **Fusionar el código (Merge)**: Una vez que el PR esté aprobado, haz clic en **"Merge pull request"** en GitHub para integrar oficialmente tu código en la rama `main`.

## 4. Limpieza del Entorno

4.1 **Eliminar ramas antiguas**: Para mantener el repositorio limpio, borra la rama que acabas de fusionar tanto en GitHub (con el botón que aparece tras el merge) como en tu ordenador local.
`git checkout main`
`git pull origin main`
`git branch -d <nombre-de-tu-rama>`
