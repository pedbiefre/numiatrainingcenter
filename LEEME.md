# NúMia Training Center · web

Landing de una sola página. Todo está en `index.html` y los logos en `img/`.

## 1. Cambiar los datos de contacto

Abre `index.html`, baja casi al final y busca el bloque `const NUMIA = { ... }`.
Ahí se cambia todo de una vez:

- `whatsapp`: prefijo 34 + número, sin espacios ni "+" (ej. `34612345678`)
- `telefonoVisible`: cómo quieres que se lea (ej. `+34 612 345 678`)
- `email`, `instagram` (sin @), `direccion`, `horario`
- `mapa`: el enlace de Google Maps del local

**El teléfono ya es el real. El email, Instagram y dirección siguen siendo de ejemplo.**

## 2. Recibir el formulario en tu email (recomendado)

Sin configurar nada, el formulario prepara un mensaje de WhatsApp con los datos
de la persona y ella solo tiene que darle a enviar.

Para que los datos te lleguen directamente al email:
1. Crea una cuenta gratis en https://formspree.io y un formulario nuevo.
2. Copia la dirección que te da (tipo `https://formspree.io/f/abcdwxyz`).
3. Pégala en `formulario: ""` dentro del bloque `NUMIA`.

## 3. Añadir las fotos del centro

1. Guarda las fotos en la carpeta `img/` (mejor .jpg, de unos 1600 px de ancho).
2. En `index.html` busca la sección `<!-- EL ESPACIO (galería) -->`.
3. En cada `<figure>`, cambia el `<div class="pronto">…</div>` por:

```html
<img src="img/sala.jpg" alt="Sala de entrenamiento de NúMia">
<figcaption>Sala de fuerza</figcaption>
```

La primera foto (`foto grande`) es la más destacada.

## 4. Antes de publicar

- Páginas de Aviso legal, Privacidad y Cookies (los enlaces del pie ya están puestos).
- Cuando haya fecha de apertura, cambia el texto "En proceso · Abrimos muy pronto"
  y los estados de la sección "Estamos en proceso" (`hecho`, `ahora` o nada).
