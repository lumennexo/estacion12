# BARBER OS Lite v5 — GitHub Pages

Estructura separada:

- `/index.html` → acceso EXCLUSIVO del barbero mediante PIN.
- `/reservar/index.html` → acceso público EXCLUSIVO para clientes.

El motor y la base de datos permanecen en Google Apps Script + Google Sheets.
No subas el Script Maestro a este repositorio.

## Actualización del repositorio existente
Reemplaza el `index.html` de la raíz por el nuevo.
Elimina `BARBER_OS_API.gs.txt`.
Crea la carpeta `reservar` y coloca dentro su `index.html`.
Puedes reemplazar `LEEME.md` por este archivo.
