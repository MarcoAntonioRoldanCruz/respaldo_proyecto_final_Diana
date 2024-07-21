# Guía de Trabajo en Colaboración en Proyecto de GitHub

## Introducción

Este documento proporciona las instrucciones y mejores prácticas para colaborar en proyectos de desarrollo de software utilizando GitHub. Sigue estos pasos para asegurar un flujo de trabajo eficiente y minimizar conflictos.

## Configuración Inicial

1. **Clonar el Repositorio:**

   - Clona el repositorio desde GitHub a tu máquina local:
     ```bash
     git clone https://github.com/tu_usuario/tu_repositorio.git
     cd tu_repositorio
     ```

2. **Configurar Git:**

   - Configura tu nombre y correo electrónico:
     ```bash
     git config --global user.name "Tu Nombre"
     git config --global user.email "tuemail@example.com"
     ```

3. **Configurar el Repositorio Remoto:**
   - Asegúrate de que el repositorio remoto esté configurado correctamente:
     ```bash
     git remote -v
     ```

## Flujo de Trabajo

1. **Actualizar la Rama Principal:**

   - Antes de comenzar a trabajar, asegúrate de que tu rama `main` esté actualizada:
     ```bash
     git checkout main
     git pull origin main
     ```

2. **Crear una Nueva Rama para tus Cambios:**

   - Crea una nueva rama para trabajar en una funcionalidad o corrección específica:
     ```bash
     git checkout -b nombre-de-la-rama
     ```

3. **Realizar Cambios y Commits:**

   - Realiza tus cambios en el código y haz commits frecuentemente:
     ```bash
     git add .
     git commit -m "Descripción de los cambios"
     ```

4. **Subir Cambios a GitHub:**

   - Sube tus cambios a la rama remota:
     ```bash
     git push origin nombre-de-la-rama
     ```

5. **Crear una Pull Request (PR):**

   - Ve a GitHub y abre una Pull Request desde tu rama hacia `main`. Asegúrate de describir claramente los cambios y cualquier contexto necesario.

6. **Revisión de Código:**

   - Revisa el código de tus compañeros y realiza comentarios constructivos. Resuelve cualquier comentario antes de fusionar la Pull Request.

7. **Fusión de Pull Request:**
   - Una vez aprobada la PR, fusiónala a `main` en GitHub. Luego, actualiza tu rama local:
     ```bash
     git checkout main
     git pull origin main
     ```

## Resolución de Conflictos

1. **Obtener Últimos Cambios:**

   - Antes de empezar a trabajar en una nueva funcionalidad, asegúrate de que tu rama local esté actualizada:
     ```bash
     git pull origin main
     ```

2. **Resolver Conflictos en Visual Studio Code:**

   - Si encuentras conflictos, abre el archivo con conflictos en Visual Studio Code. Utiliza la herramienta de combinación para resolver los conflictos.
   - Puedes cambiar la vista a texto tradicional si prefieres trabajar de esa manera:
     1. Abre la configuración (`Ctrl + ,` o `Cmd + ,` en macOS).
     2. Busca "Merge Editor" y desmarca la opción "Use Merge Editor".

3. **Realizar el Commit de Resolución:**

   - Una vez que hayas resuelto los conflictos, guarda los cambios y realiza un commit:
     ```bash
     git add archivo.txt
     git commit -m "Resuelto conflicto en archivo.txt"
     ```

4. **Subir Cambios Resueltos:**
   - Sube los cambios resueltos a GitHub:
     ```bash
     git push origin nombre-de-la-rama
     ```

## Mejores Prácticas

- **Comunicación:**

  - Mantén una comunicación abierta con tu equipo sobre el estado de tus cambios y cualquier problema que encuentres.

- **Commits Pequeños:**

  - Realiza commits pequeños y frecuentes para facilitar la revisión y resolución de conflictos.

- **Documentación:**

  - Asegúrate de que tus commits y Pull Requests estén bien documentados para que otros miembros del equipo entiendan los cambios.

- **Sincronización Regular:**
  - Mantén tu rama sincronizada con `main` para minimizar conflictos.

## Contacto

Para cualquier duda o problema, contacta al equipo de desarrollo o al administrador del repositorio.

---

¡Gracias por colaborar y mantener un flujo de trabajo eficiente en nuestro proyecto!
