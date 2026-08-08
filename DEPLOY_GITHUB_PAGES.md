# Publicación en GitHub Pages

Este proyecto es una aplicación React/Vite. GitHub Pages **no debe** publicar la
raíz de la rama `main`, porque `index.html` contiene JSX que primero debe ser
compilado.

## Configuración necesaria (una sola vez)

1. Abre `Settings` → `Pages` en el repositorio de GitHub.
2. En `Build and deployment`, cambia `Source` a **GitHub Actions**.
3. No selecciones `Deploy from a branch`, `/root` ni `/docs`.
4. Abre `Actions` y ejecuta `Deploy portfolio to GitHub Pages`, o envía un nuevo
   commit a `main`.

El workflow instala las dependencias, ejecuta `npm run build`, verifica el
resultado y publica exclusivamente la carpeta `dist`.

URL esperada:

`https://plinaresalan-ppusi.github.io/portfolio_Alan/`
