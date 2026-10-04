# Portafolio — Japheth Canales

Sitio estático de portafolio. Sin dependencias ni build: es un `index.html` con CSS y JS embebidos.

## Estructura

```
index.html                         página completa (ES / EN)
assets/japheth.jpg                 foto
assets/dashboard-hospital.mp4      grabación del reporte Power BI
assets/dashboard-hospital-poster.png
assets/CV_Japheth_Canales_Asencio.pdf
```

## Publicar en GitHub Pages

1. Sube estos archivos a la raíz del repositorio.
2. Settings → Pages → Source: `Deploy from a branch`, rama `main`, carpeta `/ (root)`.
3. En un par de minutos queda en `https://jmcanales.github.io/<nombre-del-repo>/`.

Si el repositorio se llama `jmcanales.github.io`, la URL es directamente `https://jmcanales.github.io`.

## Editar contenido

Todo el texto vive en el objeto `COPY` (español e inglés) y los datos en `PROJECTS`, `STACK`, `JOBS`, `EDU` y `NOTES`, al inicio del `<script>` en `index.html`.

- **Idioma**: se detecta por el navegador y se cambia con el botón ES / EN.
- **Proyectos**: cada entrada lleva `cat` (`auto`, `ml`, `bi`, `scrape`), `year`, `tags` y `link` opcional.
- **Repositorios**: se leen en vivo de la API pública de GitHub; si falla, se muestra una lista fija.
- **Tableau**: agrega objetos a `VIZZES` con la URL pública del dashboard (`.../viz/<Libro>/<Hoja>`); se muestran como miniatura que abre el dashboard en Tableau Public.
- **Video**: la constante `SEGMENTS` define los tramos que se reproducen en bucle, en segundos. El recorte de la interfaz de Power BI se hace por CSS en `.video-frame video`.

## Pendiente

- Certificaciones: sección reservada, falta el contenido.
- Notas: títulos propuestos, falta escribirlas.
