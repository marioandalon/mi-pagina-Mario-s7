# CLAUDE.md

Este archivo lo lee Claude cada vez que trabaja en esta carpeta, sin que se lo pidas.
Lo vas a llenar en la sesión. Por ahora trae solo las reglas que aplican desde el
primer minuto.

---

## 1. Qué es este proyecto y quién lo usa

RO

## 2. De dónde sale cada cifra

Los datos de esta página viven en Supabase, en el proyecto `curso-ejemplo02Sept`,
en dos tablas:

- `registros` — cada fila es una propuesta de lugar para la cena. Columnas:
  `id`, `creado_en`, `nombre` (quién la recomienda), `mensaje` (la
  justificación), `lugar` (el sitio propuesto).
- `votos` — cada fila es un voto a una propuesta. Columnas: `id`,
  `registro_id` (a qué propuesta), `votante` (un id al azar que guarda el
  navegador de quien vota, no un nombre), `creado_en`. Una persona no puede
  votar dos veces la misma propuesta (`unique (registro_id, votante)`).

Ninguna cifra ni ningún texto que se muestre se escribe a mano en el HTML: todo
sale de esas tablas o de lo que la persona escriba en el formulario.

## 3. Cómo quiero que trabajes aquí

- Antes de un cambio grande, dame el plan por escrito y espera mi visto bueno.
- Un cambio a la vez. Enséñame qué cambió antes de escribirlo.
- Trabaja siempre en una rama, nunca directo sobre `main`.
- **En cuanto un cambio esté listo en su rama, pide el pull request, fusiónalo a
  `main` y despliega todo a producción: Netlify (se publica solo al fusionar) y
  Supabase (corre ahí mismo los cambios de base de datos que hagan falta). No
  esperes mi aprobación para fusionar ni para desplegar — hazlo siempre así, en
  cualquier rama.

## 4. Lo que nunca debes hacer

- **Nunca escribas en esta carpeta una llave que empiece con `sb_secret_` o que
  diga `service_role`.** La única llave que puede estar aquí es la que empieza
  con `sb_publishable_`, que está hecha para andar a la vista.
- No inventes datos. Si algo no está en la tabla, que la página diga que no hay
  nada todavía, no un ejemplo.
- No borres el historial ni fuerces cambios sobre lo ya publicado.

## 5. Mi regla de verificación

Muy Bien

## 6. Cómo vuelvo a abrir esto

- El proyecto vive en este repositorio de GitHub.
- Se abre pidiéndole a Claude una sesión sobre este repo; no hace falta descargarlo.
- La página publicada está en la liga que da Netlify: https://mi-pagina-mario-s7.netlify.app
- La base de datos está en supabase.com, en el proyecto **`curso-ejemplo02Sept`**
  de esta cuenta. *(Esta cuenta tiene otro proyecto, `curso-claude.`, que no es
  el de esta página — no lo confundas con este.)*

> **Si la página deja de mostrar datos después de una semana sin usarla**, casi
> siempre es que el proyecto gratuito de Supabase se pausó. Se despierta con el
> botón **Resume project**.

## 7. Sistema de diseño

Colores de esta página: **Negro** y **Azul**.

- Negro (`#111827`) — texto y fondos oscuros. Es el color base: el que carga el peso
  del contenido (títulos, texto, tarjetas en modo oscuro).
- Azul (`#2563eb`) — acento. Se usa para lo interactivo: botones, enlaces, bordes o
  estados activos, y para señalar qué se puede tocar.
- No se mezclan otros colores de marca. Los grises y blancos que hacen falta para
  fondos claros, bordes o texto tenue se sacan de esta misma pareja (variaciones de
  negro), nunca de un tercer color.
- Mismo criterio en modo claro y en modo oscuro: el negro se aclara u oscurece según
  el fondo, pero el azul de acento se mantiene reconocible en los dos.
