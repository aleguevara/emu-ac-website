# Sitio Web — Entidad Masónica Universal (EMU)

Sitio institucional estático (página principal + página del Aviso de Privacidad). Publicado en https://emu-ac.mx. Sin servidor, sin base de datos, sin cookies de seguimiento. Pensado para alojarse en **GitHub Pages** y publicarse en **https://emu-ac.org**.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | Página principal pública: inicio, quiénes somos, valores, actividades, **Estudios de la Maestría Universal** (ensayos del blog con Lectura del día) y contacto con redes sociales. Sin datos de contacto del Responsable. Los logotipos van incrustados dentro del archivo (no requiere subir imágenes). |
| `aviso.html` | Todo lo relativo a privacidad: Aviso de Privacidad Integral (con los datos legales del Responsable que exige la LFPDPPP), botones para ejercer derechos ARCO y preguntas frecuentes. |
| `CNAME` | Indica a GitHub el dominio `emu-ac.org`. No borrar. |
| `robots.txt` | Reglas para buscadores. |

## Publicar en GitHub Pages (una vez)

1. Crear un repositorio en GitHub (por ejemplo `emu-sitio`).
2. Subir a la raíz del repositorio: `index.html`, `aviso.html`, `CNAME` y `robots.txt`. Los logotipos y los estilos ya van dentro de cada HTML: no hay imágenes ni hojas de estilo que subir por separado. Si existe un `styles.css` viejo en el repositorio, puede borrarse.
3. En el repositorio: **Settings → Pages → Build and deployment → Source: "Deploy from a branch"**, rama `main`, carpeta `/ (root)`. Guardar.
4. En **Settings → Pages → Custom domain**, escribir `emu-ac.mx` y guardar. Marcar **Enforce HTTPS** cuando se habilite.
5. En el proveedor del dominio (DNS), apuntar `emu-ac.mx` a GitHub Pages:
   - Registros `A` a: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Registro `CNAME` de `www` → `usuario.github.io`
6. Esperar la propagación (minutos a unas horas). El sitio queda en vivo en `https://emu-ac.mx`.

## Editar textos (sin conocimientos técnicos)

- Abrir `index.html` (contenido público) o `aviso.html` (texto legal) con cualquier editor de texto.
- Buscar el texto a cambiar (por ejemplo el de "Quiénes somos") y reemplazarlo. **No tocar** lo que está dentro de `< >`.
- El bloque marcado como *"Sección institucional de muestra"* en "Quiénes somos" debe sustituirse por el texto que la Maestría apruebe hacer público.
- Guardar y volver a subir el archivo a GitHub. El sitio se actualiza solo.

## Notas de cumplimiento

- El Aviso de Privacidad Integral vive en `aviso.html`, enlazado desde la navegación, el inicio y el pie: queda "puesto a disposición" del titular (Art. 15-16 LFPDPPP; Art. 26 del Reglamento). Los datos de contacto del Responsable constan únicamente ahí, por decisión de discreción de la página pública.
- Los botones de derechos ARCO abren un correo a `emuac33@gmail.com` con el asunto correcto. El sitio **no recibe ni guarda** datos sensibles.
- Si la ley o el aviso cambian, actualizar el texto en `aviso.html` y la fecha de "Última actualización".
- Los enlaces a redes sociales (Facebook, Instagram, YouTube) están en Contacto y en el pie de página. Regla de difusión en esos canales: no publicar caras de miembros ni identificar afiliados.

---
Preparado por **Adir Data Invictus** como caso de referencia. Marca y contenido propiedad de EMU.

## Sección "Estudios de la Maestría Universal"

- Se alimenta sola del blog https://carlosvaldesmartin.blogspot.com/ (últimos 3 ensayos + "Lectura del día").
- La "Lectura del día" es la misma para todos los visitantes y cambia automáticamente cada medianoche. Nadie tiene que administrarla.
- No requiere configuración: cuando Carlos publica en el blog, el sitio se actualiza solo.
- Los botones de compartir abren WhatsApp y Facebook con el enlace del ensayo listo para enviar.
