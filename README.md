# PLEX Weekly Blog

Blog semanal con estetica cyberpunk/futurista para publicar noticias de ciencia, astronomia y divulgacion cientifica con la voz de PLEX: operador Lazarus orientado a objetivos, eficiente y con humor seco en dosis controladas.

## Descripcion del proyecto

`PLEX Weekly Blog` es una base estatica lista para GitHub Pages. Incluye una landing page, un template para issues individuales, un primer issue de ejemplo y configuracion minima de Jekyll para publicar sin friccion.

## Estructura del repo

```text
plex-weekly-blog/
├── _config.yml
├── index.html
├── issue-template.html
├── README.md
├── styles.css
├── assets/
│   └── images/
└── issues/
    └── week-01-2026-06-20.html
```

## Instrucciones de publicacion

1. Crea un nuevo issue semanal copiando `issue-template.html` dentro de `issues/`.
2. Renombra el archivo con el patron `week-XX-YYYY-MM-DD.html`.
3. Actualiza el contenido del issue con la fecha del viernes de publicacion y el periodo cubierto de viernes anterior a jueves.
4. Añade el nuevo enlace en `index.html` dentro de la seccion de issues.
5. Confirma los cambios y subelos al repositorio.

## GitHub Pages setup

1. Sube este repositorio a GitHub.
2. Entra en `Settings > Pages`.
3. En `Build and deployment`, selecciona `Deploy from a branch`.
4. Elige la rama principal y la carpeta `/ (root)`.
5. Guarda la configuracion y espera a que GitHub publique el sitio.

Si quieres probarlo en local con Jekyll:

```bash
bundle exec jekyll serve
```

Tambien puedes abrir `index.html` directamente en el navegador para una validacion rapida del layout, ya que el sitio es estatico.

## Notas operativas

- El estilo visual usa tema oscuro con acentos azul electrico y cyan.
- La carpeta `assets/images/` queda preparada para portadas, graficos o imagenes de futuros issues.
- El contenido esta redactado en espanol con referencias ligeras al universo de *Interstellar*.
