# CLAUDE.md

Este archivo lo lee Claude cada vez que trabaja en esta carpeta, sin que se lo pidas.
Lo vas a llenar en la sesión. Por ahora trae solo las reglas que aplican desde el
primer minuto.

---

## 1. Qué es este proyecto y quién lo usa

RO

## 2. De dónde sale cada cifra

Los datos de esta página viven en una tabla de Supabase llamada `registros`.
Ninguna cifra ni ningún texto que se muestre se escribe a mano en el HTML: todo
sale de esa tabla o de lo que la persona escriba en el formulario.

*(En la sesión le agregas las columnas que acabes usando.)*

## 3. Cómo quiero que trabajes aquí

- Antes de un cambio grande, dame el plan por escrito y espera mi visto bueno.
- Un cambio a la vez. Enséñame qué cambió antes de escribirlo.
- Trabaja siempre en una rama, nunca directo sobre `main`.
- No publiques a producción sin que yo lo pida: fusionar es una decisión mía.
- **Si tienes acceso a mi base de datos, enséñame el SQL antes de correrlo y espera mi
  respuesta.** Crear o borrar tablas, agregar o quitar columnas y cambiar permisos no se
  deshacen con una rama: en cuanto corren, ya está.

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
- La página publicada está en la liga que da Netlify.
- La base de datos está en supabase.com, en el proyecto de esta cuenta.

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
