# BARBER OS — Cascarón de entrada (GitHub Pages)

Esta carpeta es la **puerta de entrada** que oculta la URL de Apps Script.
El barbero abre un link limpio de GitHub (`lumennexo.github.io/...`), escribe su
llave, y el panel se abre **embebido** — nunca ve la dirección de `script.google.com`.

## Archivos
- `index.html` — la pantalla de acceso + el panel embebido (esto va a GitHub).
- `BARBER_OS_API.gs.txt` — el código de Apps Script (el motor). Este NO va a GitHub;
  va pegado en tu Google Sheet.

## Pasos (una vez por barbería)

1. **Apps Script**: pega `BARBER_OS_API.gs.txt` en tu Sheet, guarda, y
   **reimplementa** (Administrar implementaciones → editar → Nueva versión).
   *(Este código ya trae el permiso para poder embeberse.)*
   Copia la URL de la Web App (termina en `/exec`).

2. **index.html**: abre el archivo y edita SOLO estas dos líneas de arriba del script:
   - `EXEC_URL` = la URL `/exec` que copiaste.
   - `NOMBRE`   = el nombre que se muestra en la entrada (ej. "Estación 12").

3. **GitHub Pages**: sube `index.html` a tu repo de GitHub Pages
   (por ejemplo, una carpeta `barberos/` dentro de `lumennexo.github.io`).
   Tu link quedaría algo como: `https://lumennexo.github.io/barberos/`

4. Comparte ese link con el barbero, y dale su **PIN** aparte (como contraseña).
   La primera vez lo escribe; después se recuerda y entra directo.

> Para otra barbería: copia esta carpeta, cambia `EXEC_URL` y `NOMBRE`, y súbela
> a otra ruta (ej. `lumennexo.github.io/barberia-x/`).
