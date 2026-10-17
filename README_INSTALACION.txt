GUITARSTUDIO PREMIUM - PWA PARA ANDROID

1. Publicación: sube el CONTENIDO de esta carpeta a un repositorio GitHub nuevo.
2. En Vercel: Add New > Project > Importa el repositorio, Framework Preset: Other,
   Root Directory: ./ (raíz), Build Command: vacío, Output Directory: ./.
3. Una vez que Vercel muestre la dirección https://..., abre la URL en Chrome Android.
4. Espera a que cargue; toca «Instalar GuitarStudio» cuando aparezca, o en el menú
   de Chrome (⋮) elige «Instalar aplicación» / «Añadir a pantalla principal».
5. Si en algún momento cambias el contenido: vuelve a publicar los archivos y actualiza
   la versión del caché en sw.js (v1 -> v2) para evitar contenido antiguo.

PRUEBAS LOCALES: no abras index.html con doble clic para probar instalación PWA:
  Desde esta carpeta: python -m http.server 8000
  Luego en tu PC: http://localhost:8000
  La instalación en Android requiere HTTPS (Vercel lo proporciona).

NOTAS:
- La interfaz y recursos principales se guardan offline después de una primera carga exitosa.
- YouTube, Chordify, fuentes externas y otros servicios web necesitan internet.
- El progreso, las tareas, notas y favoritos permanecen en el navegador/dispositivo.
- Utiliza Exportar para generar una copia de seguridad antes de cambiar de teléfono.
- Chrome puede decidir no mostrar el diálogo de instalación; usa el menú del navegador.
