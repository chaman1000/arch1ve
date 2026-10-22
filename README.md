# Mi red

Esfera 3D de imágenes, videos y audio. HTML + CSS + JavaScript, sin dependencias ni instalación.

## Usar
Abre `index.html` en el navegador (los estilos están en `style.css`).

## Agregar archivos
1. Copia tus archivos a la carpeta `media/`.
2. En `index.html`, busca la lista `MEDIA` y agrega una línea por archivo:

```js
{type:'image', src:'media/foto1.jpg', title:'Mi foto'},
{type:'video', src:'media/clip.mp4',  title:'Un clip'},
{type:'audio', src:'media/tema.mp3',  title:'Una canción'},
```

## Ajustes rápidos (en `index.html`)
- Tamaño de las fotos: busca `const w=Math.round(64+((i*37)%40))` (base 64 px + variación hasta 40 px).
- Velocidad de giro automático: `0.0015` dentro de `frame()`.
- Fondo: variable `--bg` al inicio de `style.css`.

## Subir a Git y publicar gratis
```bash
git init
git add .
git commit -m "Primera versión"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/mi-red.git
git push -u origin main
```
Luego, en GitHub: Settings → Pages → Branch `main` → Save.

Nota: GitHub rechaza archivos de más de 100 MB y recomienda repos de menos de 1 GB. Para videos pesados, usa Git LFS o un hosting aparte.
