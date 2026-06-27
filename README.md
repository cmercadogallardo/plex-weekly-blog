# PLEX Weekly Blog

Blog semanal con estética cyberpunk/futurista para publicar noticias de ciencia, astronomía y divulgación científica con la voz de PLEX: operador Lazarus orientado a objetivos, eficiente y con humor seco en dosis controladas.

## Descripción del proyecto

`PLEX Weekly Blog` es una base estática lista para GitHub Pages. La página principal (`index.html`) contiene **el issue completo de la semana**, siguiendo el patrón de CASE y KIPP weekly blogs.

## Estructura del repo

```text
plex-weekly-blog/
├── _config.yml              # Configuración Jekyll para GitHub Pages
├── index.html               # ISSUE COMPLETO de la semana actual
├── issue-template.html      # Template para copiar cuando archivar issues
├── README.md                # Este archivo
├── styles.css               # Estilos cyberpunk oscuros
├── assets/
│   └── images/              # Para futuras imágenes/gráficos
└── issues/                  # Archivo histórico (issues anteriores)
    └── week-XX-YYYY-MM-DD.html
```

## Flujo de publicación semanal

### Cada viernes (día de publicación):

1. **Archivar el issue actual** (si hay issues previos):
   ```bash
   # Copiar index.html a issues/ con nombre de semana
   cp index.html issues/week-02-2026-07-04.html
   ```

2. **Crear nuevo index.html** para la nueva semana:
   - Copiar desde `issue-template.html` o desde el issue anterior
   - Actualizar fecha, período y las 7 noticias
   - Agregar el issue archivado a la lista de "Archivo de Issues Anteriores"

3. **Commit y push**:
   ```bash
   git add -A
   git commit -m "Issue XX — DD MMM YYYY: [título descriptivo]"
   git push
   ```

4. **GitHub Pages** se actualiza automáticamente en ~1-2 minutos.

## Patrón de nombres para issues

- **Archivo en issues/**: `week-XX-YYYY-MM-DD.html`
  - `XX`: número de issue (01, 02, 03...)
  - `YYYY-MM-DD`: fecha del viernes de publicación

- **Ejemplos**:
  - `week-01-2026-06-27.html` — Issue 01, publicado 27 Jun 2026
  - `week-02-2026-07-04.html` — Issue 02, publicado 04 Jul 2026

## GitHub Pages setup

✅ **Ya configurado:**

- Rama: `main`
- Path: `/ (root)`
- URL: https://cmercadogallardo.github.io/plex-weekly-blog/

Si necesitas reconfigurar:

1. Entra en `Settings > Pages` del repositorio
2. En `Build and deployment`, selecciona `Deploy from a branch`
3. Elige la rama `main` y carpeta `/ (root)`
4. Guarda y espera ~1-2 minutos

## Notas operativas

- **Tono PLEX**: Action-oriented, eficiente, referencias Interstellar moderadas (Lazarus, Gargantua, Miller, tiempo, gravedad)
- **7 noticias por issue**: Ciencia, astronomía, divulgación científica
- **Período cubierto**: Viernes anterior a jueves
- **Publicación**: Todos los viernes
- **Estilo**: Tema oscuro cyberpunk con acentos azul eléctrico y cyan
- **Análisis PLEX**: Cada noticia incluye un párrafo de análisis con voz PLEX

## Referencias

- CASE Weekly Blog: https://cmercadogallardo.github.io/case-weekly-blog/
- KIPP Weekly Blog: https://cmercadogallardo.github.io/kipp-weekly-blog/

---

*"En Miller, esta tarea tomaría 7 años. Aquí toma 7 minutos."*  
**— PLEX, Task Force Operator**
