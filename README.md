# Knova — landing page

Página de una sola pieza (`index.html`) con sus imágenes de portafolio y videos de ejemplo. No necesita build ni dependencias — es HTML/CSS/JS puro.

## Estructura

```
index.html
portfolio/   ← 8 capturas reales (plan Cloud y Multiplataforma)
video/       ← 4 clips de ejemplo (mp4 + webm, por compatibilidad)
```

## Subir al repo

```bash
git add .
git commit -m "Publicar landing Knova"
git push
```

## Publicar con GitHub Pages

1. En el repo, ve a **Settings → Pages**.
2. En "Build and deployment" → **Source**, elige **Deploy from a branch**.
3. Selecciona la rama (normalmente `main`) y la carpeta `/ (root)`.
4. Guarda — GitHub te da un link tipo `https://tu-usuario.github.io/tu-repo/` en uno o dos minutos.

Si usas un dominio propio (ej. `knova.com`), agrégalo en el mismo apartado de Pages y crea el registro DNS que GitHub te indique (normalmente un CNAME).

## Notas

- Todo carga por rutas relativas (`portfolio/...`, `video/...`), así que la carpeta debe subirse completa y junta — no muevas `index.html` a otro nivel sin mover las carpetas con él.
- Los videos están silenciados por defecto (política de autoplay de los navegadores); el visitante puede activar el audio desde los controles del reproductor.
- El formulario de contacto abre el correo del visitante con el mensaje ya armado (no envía nada a un servidor) — si más adelante quieres que llegue a un backend o a un correo de Knova, hay que conectarlo aparte.
