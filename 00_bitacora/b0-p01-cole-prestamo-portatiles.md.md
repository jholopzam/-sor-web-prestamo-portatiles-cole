
- **Alumno:** Jhoseen lopez zambrano
- **Bloque:** SOR — Sistemas Operativos en Red · 2.º SMR
- **Fase / ejercicio:** Fase 0.8 · Práctica 01 · Cole: préstamo de portátiles
- **Fecha de inicio:** 19/10/2026
- **Fecha de entrega:** 17/10/2026

---

## 🎯 Qué se pedía

Crear desde cero una bóveda llamada Boveda_HTML_Centro, un proyecto web de préstamo de portátiles con su propio repositorio Git conectado a GitHub mediante SSH, guardar versiones evolutivas (inicio, mantenimiento y ampliación con normas, contacto e imagen), ignorar clips de vídeo locales, consultar versiones anteriores en el historial y documentarlo todo en un vídeo de pantalla y en esta bitácora.

## ⌨️ Comandos y pasos importantes

- `git init` — inicializa un repositorio local de Git en la carpeta de trabajo.
- `git branch -M main` — establece el nombre de la rama principal como main.
- `git remote add origin ...` — vincula el repositorio local con el repositorio remoto en GitHub mediante SSH.
- `git status` — muestra el estado actual del árbol de trabajo y los archivos modificados o sin seguimiento.
- `git add <ruta>` — prepara archivos específicos para el siguiente commit (área de preparación / índice).
- `git diff` — compara los cambios realizados en el disco con respecto al último commit o al índice.
- `git commit -m "mensaje"` — guarda una versión local con los cambios preparados y un mensaje descriptivo.
- `git push` — sube los commits locales a la rama principal del repositorio remoto en GitHub.
- `git check-ignore -v ...` — comprueba qué regla del fichero `.gitignore` excluye un archivo determinado.
- `git switch --detach <codigo>` — permite situarse temporalmente en un commit anterior para consultar su estado sin alterar ramas.
- `git switch main` — regresa a la rama principal de trabajo.

## 🛠️ Qué he hecho

1. He iniciado OBS Studio para grabar la sesión completa desde el principio y he comprobado previamente Git, mi identidad de usuario y la autenticación SSH con GitHub.
2. He creado la bóveda `Boveda_HTML_Centro` fuera de OneDrive y he estructurado las carpetas `00_Grabaciones`, `01_Proyecto`, `00_Bitacora` y `web`.
3. He redactado esta bitácora, creado el fichero `.gitignore` para excluir vídeos locales y escrito la primera versión de `index.html` con la disponibilidad inicial del equipo 01.
4. He inicializado Git dentro de `01_Proyecto`, he creado el repositorio vacío `sor-web-prestamo-portatiles-cole` en GitHub y he configurado el remoto `origin` mediante SSH.
5. He guardado el primer commit con la página inicial y he realizado el primer `push` a GitHub.
6. He modificado el estado del portátil a mantenimiento, he comprobado los cambios con `git diff` y he guardado la segunda versión subiéndola al remoto.
7. He construido la ampliación añadiendo la imagen `portatil.png`, los clips de vídeo locales (que han quedado excluidos correctamente gracias a `.gitignore`), y las páginas `normas.html` y `contacto.html` enlazadas desde la portada.
8. He preparado individualmente cada archivo de la ampliación, he comprobado el estado y he registrado la tercera versión en un nuevo commit y su respectivo `push`.
9. He comprobado el historial, he visitado temporalmente el primer commit mediante `git switch --detach` para verificar el estado inicial y he regresado a la rama `main`.
10. He completado esta bitácora con los enlaces definitivos, he realizado el último commit documental y he detenido la grabación para subir el vídeo a YouTube con sus marcas de tiempo.

## 🚩 Qué me ha fallado y cómo lo he resuelto

nada

## 🤔 Respuestas a las preguntas

1. Porque la bóveda de Obsidian contiene la organización general de apuntes y grabaciones, mientras que el control de versiones con Git debe aplicarse únicamente sobre la carpeta específica del código del proyecto (`01_Proyecto`) para no mezclar configuraciones de la aplicación ni archivos multimedia externos.
2. Antes de `add`, `git status` mostraba los ficheros en rojo como no rastreados (`??`) o modificados sin preparar (`M`). Después de `add`, aparecían en verde en el área de preparación (índice) listos para el commit. Después de `commit`, el árbol de trabajo quedaba limpio indicando que no había cambios pendientes.
3. Para mantener una copia de respaldo segura en la nube, posibilitar la entrega de la tarea y permitir la colaboración o sincronización remota utilizando claves SSH para una autenticación segura sin contraseñas.
4. Porque las páginas nuevas son ficheros sin seguimiento que Git todavía no conoce en el historial, por lo que `git diff` compara únicamente ficheros que ya están bajo seguimiento, mientras que `git status` sí informa de la existencia de dichos archivos nuevos.
5. Mediante el comando `git check-ignore -v`, el cual indica explícitamente qué regla y número de línea del fichero `.gitignore` están aplicando la exclusión sobre los archivos de vídeo.
6. Muestra un resumen estadístico de los ficheros que han sido añadidos al área de preparación (índice), indicando las rutas modificadas y el número de inserciones o eliminaciones de líneas preparadas para el próximo commit.
7. Al visitar el primer commit mediante `--detach`, los archivos del proyecto retroceden temporalmente al estado inicial de esa versión. Al volver a `main`, se recupera la versión más avanzada con toda la ampliación y el historial completo intactos.
8. Permite auditar la evolución del proyecto, identificar el autor y el motivo de cada cambio, recuperar versiones funcionales anteriores si una modificación falla, y coordinar de manera ordenada el trabajo entre varios técnicos evitando sobreescrituras accidentales.
9. No es necesario repetir `git init` ni configurar de nuevo el remoto `origin`. Solo debo modificar el archivo, comprobar los cambios con `git status` y `git diff`, preparar el archivo con `git add`, guardarlo localmente con `git commit -m` y subirlo con `git push`.

## 🔗 Enlaces

- **Vídeo de esta fase:** https://youtu.be/cHhLWILFHLQ[cite: 
- **Playlist:** https://www.youtube.com/playlist?list=PLO5ffLKNKdF8[cite: 
- **Repositorio GitHub:** https://github.com/jholopzam/-sor-web-prestamo-portatiles-cole.git[cite: 

## 💭 Dudas / a repasar

- Ninguna duda pendiente; el flujo completo de control de versiones y exclusión mediante `.gitignore` ha quedado comprendido.