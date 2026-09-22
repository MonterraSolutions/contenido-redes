# Tony de Olarte · diseño floral

Lanzamiento de su sitio. **Tres publicaciones**, una carpeta cada una.

Etiquetar siempre a **@tonydeolarte.disenofloral**.
Sitio del cliente: **tonydeolartedisenofloral.com**

Diseño: dirección **Cumbre** de Monterra. Uno de los tres posts va en registro
**Señal** (Archivo Black sobre bloque plano) y los otros dos en **Editorial**.

---

## Post 01 · Ya está en línea

[`post-01-ya-en-linea/ya-en-linea.png`](post-01-ya-en-linea/ya-en-linea.png) — 2160×2160 · registro **Señal**

El anuncio. Es el único de los tres que grita.

Las dos capturas son del sitio **en producción**, tomadas del viewport completo a scroll 0,
así que se ve el encabezado entero: logo, los cinco enlaces y el botón *Cotizar*. Escritorio
1440×900 a 2x (2880×1800) y celular 430×932 a 3x (1290×2796). Los dos aparatos apoyan en la
misma línea y el celular queda a ras del margen derecho.

> Tony de Olarte ya tiene sitio.
> Diseño floral para bodas, XV y despedidas en Monterrey, ahora con galería, catálogo de ramos y cotización directa por WhatsApp.
>
> tonydeolartedisenofloral.com
>
> #MonterraSolutions #DiseñoWeb #Monterrey #DiseñoFloral

---

## Post 02 · El ramo

[`post-02-ramo/ramo-4x5.jpg`](post-02-ramo/ramo-4x5.jpg) — 2160×2700 · registro **Editorial**
[`post-02-ramo/ramo-1x1.jpg`](post-02-ramo/ramo-1x1.jpg) — 2160×2160 (versión cuadrada)

Sólo la fotografía. Sin titular, sin marco, sin dominio: abajo a la izquierda
únicamente el monograma y **Cliente Monterra**, en chico. El original es de
3089×4633, así que aguanta cualquier recorte.

> Ramo de novia por Tony de Olarte.
> Casi treinta años decorando eventos en Monterrey.
>
> tonydeolartedisenofloral.com
>
> #DiseñoFloral #Bodas #RamoDeNovia #Monterrey #MonterraSolutions

---

## Post 03 · El video

| Archivo | Medida | Para |
|---|---|---|
| [`post-03-video/reel-celular-9x16.mp4`](post-03-video/reel-celular-9x16.mp4) | 1080×1920 · 34 s | El reel |
| [`post-03-video/reel-escritorio-4x5.mp4`](post-03-video/reel-escritorio-4x5.mp4) | 1080×1350 · 27 s | Feed — ver nota |
| [`post-03-video/portada-reel-9x16.png`](post-03-video/portada-reel-9x16.png) | 1080×1920 | Portada del reel |
| [`post-03-video/portada-feed-4x5.png`](post-03-video/portada-feed-4x5.png) | 1080×1350 | Portada en feed |
| [`post-03-video/portada-grid-1x1.png`](post-03-video/portada-grid-1x1.png) | 1080×1080 | Miniatura del perfil |

Las portadas son el logo de Tony y la frase sobre crema, sin barra de etiqueta ni tira
de crédito. Cada una está a la medida exacta que le toca, así que entran sin recorte.

El video va **sin audio a propósito**: la música se le pone en Instagram al publicar, así
queda ligada al catálogo de la app y no la tumban por derechos.

**Qué se ve:** un cursor recorre el sitio como lo haría una persona — abre el menú, entra
a la galería, cambia el estilo de bodas y pasa fotos. Al llegar a la cotización el
formulario está **vacío** y se llena en cámara: teclea el nombre letra por letra, abre el
desplegable y baja por las opciones hasta *Boda*, escribe la fecha por segmentos
(día → mes → año) y teclea el lugar del evento. Nada aparece prellenado.

> 30 años decorando eventos en Monterrey, y ahora también en internet.
> Así se navega el sitio de Tony de Olarte: galería por tipo de evento, estilos de boda y cotización que llega directo al WhatsApp.
>
> tonydeolartedisenofloral.com
>
> #MonterraSolutions #DiseñoWeb #Monterrey #DiseñoFloral #Bodas #XVAños

### Nota sobre el 4:5

La versión **4:5 de escritorio** es la original: su formulario todavía aparece
**prellenado**, no se llena en cámara como el 9:16. Se publica así por ahora; queda
pendiente regrabarla con la misma receta (`record.js`) para que las dos versiones
cuenten lo mismo. Si hay que elegir una sola para publicar, usar el 9:16.

---

## Capturas del sitio

[`capturas/sitio-escritorio-2880x1800.png`](capturas/sitio-escritorio-2880x1800.png)
[`capturas/sitio-celular-1290x2796.png`](capturas/sitio-celular-1290x2796.png)

El hero completo, sin recortar, listo para meterse en cualquier pieza nueva. Se vuelven a
tomar con `shot.js` (Chrome headless + CDP): se siembra `tdo_consentimiento` en localStorage
para que no salga el aviso de cookies, se dejan **terminar** las animaciones de entrada
(`a.finish()`, nunca `currentTime = 0`, que las deja invisibles) y se cancelan las infinitas
como el pulso del botón de WhatsApp.

**Nunca recortar el encabezado.** El sitio es el producto que se vende: si el logo o el menú
salen cortados, la pieza no se publica.

---

## Archivos de trabajo

Los HTML editables y el script de grabación (`record.js`) están en la Mac, en
`Monterra Solutions/Monterra_Solutions/Plantillas de posts/tony-de-olarte/`.
Los posts se exportan con una captura de ventana a la medida que toque; el video se
regraba con `record.js` (Chrome headless + CDP, frame por frame a 30 fps).
