# Precio de Circuito — PWA offline

## Archivos
- `index.html`: aplicación y calculadora.
- `manifest.webmanifest`: configuración de instalación e icono.
- `sw.js`: caché para abrir la aplicación sin Internet.
- `icons/`: iconos de la aplicación.

## Publicar en GitHub Pages
1. Descomprime este paquete.
2. Sube **todo el contenido** de la carpeta (no solamente el ZIP) a la raíz de tu repositorio GitHub.
3. En GitHub abre **Settings → Pages**.
4. En **Build and deployment**, selecciona `Deploy from a branch`, la rama `main` y la carpeta `/ (root)`. Guarda.
5. Espera a que GitHub Pages publique la web y abre la dirección HTTPS desde Chrome en Android.
6. Abre la página una vez con Internet. Espera unos segundos para que el service worker guarde los archivos.
7. En Chrome, menú ⋮ → **Instalar aplicación** o **Añadir a pantalla de inicio**.

## Acceso ADMIN
- Usuario: `Inventa`
- Clave: `inventa123`

Los cambios de componentes, precios y multiplicadores se guardan en el almacenamiento local del navegador de ese dispositivo. No se sincronizan automáticamente entre celulares.

## Importante sobre la clave
Esta clave sirve como bloqueo básico de la interfaz, no como seguridad real: al ser una aplicación estática, el código puede inspeccionarse. No uses esta contraseña para proteger información sensible.

## Uso sin conexión
La primera visita debe hacerse con Internet para descargar y almacenar la aplicación. Después de esa primera carga, podrá abrirse desde el icono instalado sin conexión. Si publicas una nueva versión, abre la página con Internet para actualizar la caché.
