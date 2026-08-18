# PEP-T+ Labs — sitio web

Landing page de una sola página, sin dependencias externas: todo el CSS, el JavaScript
y los gráficos (SVG + canvas) están dentro de `index.html`.

## Contenido

```
index.html    la web completa (único archivo necesario)
logo.png      opcional — ver abajo
```

## Publicar

Cualquier hosting estático sirve. No hace falta compilar nada.

- **GitHub Pages** — Settings → Pages → Source: `Deploy from a branch` → rama `main`, carpeta `/ (root)`.
- **Netlify / Vercel** — arrastrar la carpeta, o conectar el repositorio.
- **Hosting propio** — subir `index.html` por FTP a la raíz del dominio.

## Usar el logo real

El emblema dorado del hero está dibujado en vector. Para reemplazarlo por el archivo real:

1. Guardar la imagen como **`logo.png`** junto a `index.html`.
2. Listo — la página la detecta sola y oculta el dibujo vectorial.

## Qué editar

Todo está en `index.html`, buscar y reemplazar:

| Dato | Valor actual (placeholder) |
|---|---|
| Email | `orders@pept-labs.com` |
| WhatsApp | `https://wa.me/10000000000` |
| Telegram | `https://t.me/peptlabs` |
| Precios | `$54`, `$58`, `$46`, `$49`, `$42`, `$44` |
| Lote de ejemplo | `PT-2408-A` |

## Idiomas

El sitio es bilingüe inglés/español. El botón **EN ▾** del menú cambia el idioma.
Cada texto lleva sus dos versiones en los atributos `data-en` y `data-es`.

## Aviso legal

Los productos se ofrecen únicamente para investigación de laboratorio. El aviso aparece
en la barra superior, en la sección "The PEP-T+ standard" y en el pie de página.

## Usar el arte del hero como imagen

El ADN del hero está dibujado con código (canvas). Si preferís usar una imagen ya
renderizada — por ejemplo el mockup original — el sitio la toma sola:

1. Guardá la imagen como **`hero-dna.png`** junto a `index.html`.
2. Recargá. El dibujo por código se apaga y queda la imagen ocupando todo el hero.

Recomendado: 1600 × 900 px o más. La imagen se recorta con `object-fit: cover`
anclada a la derecha, así el ADN queda del lado de la placa.

Para volver al ADN animado, basta con borrar o renombrar `hero-dna.png`.
