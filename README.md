<div align="center">

<img src="favicon.svg" alt="Escudo de El Salvador" width="110">

# Editor de Marca Institucional

**Gobierno de El Salvador · 2019–2026**

Herramienta web para aplicar correctamente la marca de Gobierno en documentos, logotipos y videos, siguiendo el *Manual de Uso de Marca*.

![HTML](https://img.shields.io/badge/HTML-single%20file-001A70?style=for-the-badge)
![Sin servidor](https://img.shields.io/badge/Backend-no%20requiere-0A3BB5?style=for-the-badge)
![Idioma](https://img.shields.io/badge/Idioma-Espa%C3%B1ol-555?style=for-the-badge)

</div>

---

## 🧭 Vista general

```
┌──────────────────────────────────────────────────────────────┐
│                 EDITOR DE MARCA INSTITUCIONAL                │
│            Gobierno de El Salvador · 2019–2026               │
├──────────────────┬───────────────────┬───────────────────────┤
│  💧 MARCA DE     │  🛡️ CREAR         │  🎬 CREAR             │
│     AGUA         │     LOGOTIPO      │     ANIMACIÓN         │
│                  │                   │                       │
│  Sobre un PDF    │  Escudo + hasta   │  Intro / Outro con    │
│  coloca escudo,  │  3 bloques de     │  el escudo que se     │
│  logo o texto    │  texto            │  revela y da paso     │
│                  │                   │  al logo              │
│  [Abrir →]       │  [Abrir →]        │  [Abrir →]            │
└──────────────────┴───────────────────┴───────────────────────┘
        📖 Botón «Manual de Uso de Marca 2019–2026» bajo el título
```

| Herramienta | Qué hace | Resultado |
|---|---|---|
| **Insertar Marca de Agua** | Coloca el escudo, el logo del ministerio o texto (*Documento Oficial*, *Borrador*, *Confidencial*) sobre un PDF | PDF con marca de agua |
| **Crear Logotipo** | Compone un logotipo horizontal o vertical: escudo + hasta 3 bloques (ministerio, dirección, unidad) | Logotipo institucional |
| **Crear Animación** | Genera un video de intro u outro estilo Cadena Nacional | Archivo de video real |
| **Crear Carnet** | Diseña el carnet institucional (frente y reverso) con foto, nombre, ID, QR y logos | PNG de alta resolución (2×) |

---

## 💧 1. Insertar Marca de Agua

```
┌─────────────── PDF ───────────────┐
│                                   │
│        ┌───────────────┐          │
│        │   🛡️ / texto  │  ← 5 %   │
│        │  (marca agua) │  opacidad│
│        └───────────────┘          │
│                                   │
└───────────────────────────────────┘
```

| Función | Detalle |
|---|---|
| Documento | Sube un PDF y trabaja sobre sus páginas |
| Tipos de marca | Escudo institucional, logo del ministerio o texto |
| Textos rápidos | Documento Oficial, Borrador, Confidencial o texto personalizado |
| Transparencia | **5 %** recomendado por el manual (ajustable con deslizador y atajos 5 / 25 / 50 / 75 / 100 %) |
| Posición | Centrar horizontal, vertical o en página; bloquear, duplicar y eliminar objetos |
| Tipografía | Fuentes PDF estándar y fuente propia (`.ttf`, `.otf`, `.woff`) |
| Alcance | Aplicar a páginas seleccionadas del documento |

---

## 🛡️ 2. Crear Logotipo

```
 Vertical                    Horizontal
 ┌──────────┐                ┌──────────────────────────────────┐
 │    🛡️    │                │ GOBIERNO DE │ 🛡️ │ EL SALVADOR     │
 │ Gobierno │                └──────────────────────────────────┘
 │ de ES    │
 └──────────┘                Escudo + | Ministerio | Dirección | Unidad
```

**Color del bloque institucional.** En los módulos *Color* y *Color de sub bloques* hay una sección desplegable, «Color del bloque institucional» (escudo + «Gobierno de El Salvador»), con interruptor, colores del Manual, selector libre, campo HEX y botón **Azul oficial**. Es el mismo editor en ambos módulos. Con el color propio activo tiene **prioridad** sobre el color global y el color común de sub bloques; apagado, todo funciona como antes.

**Panel de controles** (todos los módulos inician plegados):

| Módulo | Para qué sirve |
|---|---|
| Guía de marca | Referencia rápida del manual |
| Institucional | Escudo oficial vectorial, orientación (vertical / horizontal) y opción de usar tu propia imagen |
| Bloques | Hasta 3 bloques de texto: ministerio, dirección y unidad |
| Tipografía | Fuente, tamaño y fuente personalizada |
| Separadores | Líneas divisorias entre bloques |
| Color | Color global del logotipo (por defecto azul oficial `#001A70`) y editor de **color del bloque institucional** |
| Subcolor | Color común para sub bloques (con alcance) y el mismo editor del bloque institucional |
| Tamaño | Proporciones del escudo y del conjunto |
| Presets | Composiciones listas: Gobierno + Ministerio, + Dirección, + Unidad |
| Exportar | Descarga del logotipo terminado |

---

## 🎬 3. Crear Animación

```
 Fase 1              Fase 2               Fase 3
┌────────┐         ┌────────┐          ┌──────────────┐
│        │         │   🛡️   │          │ 🛡️ │ Logo    │
│  ···   │   →     │ revela │    →     │    │ completo│
│        │         │        │          │              │
└────────┘         └────────┘          └──────────────┘
   inicio          escudo aparece       logo institucional
```

| Módulo | Opciones |
|---|---|
| **Tipo de video** | **Intro**, **Outro** o **Intro + Outro** (un solo video con intro, pausa con el logo fijo y outro) |
| **Animaciones** | Efectos de entrada y salida (desvanecer, deslizar, zoom, difuso, cortinas, abrir) y el efecto **«Desde el divisor (Cadena Nacional)»**: la línea divisoria crece y de ella salen el escudo y el texto; al salir hacen el recorrido inverso |
| **Contenido** | Usa automáticamente el logotipo creado en *Crear Logotipo*; **secuencia del video** (interruptores), color del escudo al revelarse y colores del logo completo |
| **Fondo** | Color (paleta o personalizado en HEX), imagen, transparente o croma |
| **Duración y resolución** | Duración con deslizador; en *Intro + Outro* tres controles independientes: **Intro**, **Pausa con el logo fijo** y **Outro** |
| **Exportar** | Genera el archivo de video (MP4 si el navegador lo permite; si no, WebM) |

**Secuencia del video (interruptores en *Contenido*, excluyentes entre sí):**

| Interruptor | Resultado |
|---|---|
| **Escudo → logo editado → escudo** | Sale primero el escudo solo, luego el logo editado, vuelve el escudo y se despide |
| **Solo el logo editado** | Aparece únicamente el logo editado, sin el escudo solo |
| *(ambos apagados)* | La secuencia depende de *Tipo de video* (Intro, Outro o Intro + Outro) |

**Intro + Outro.** La intro se detiene cuando el logo ya está completo, se mantiene quieto durante la pausa y el outro arranca desde ahí, sin saltos. Con la pausa en 0 s, el logo pasa directo de la intro al outro. Duración total = intro + pausa + outro (hasta 24 s).

**Efecto «Desde el divisor».** Requiere un logo con al menos un separador (por ejemplo, escudo + ministerio). Con el escudo solo, cae en «Abrir horizontal».

**Exportación.** Los cuadros se entregan con ritmo exacto (sin acumular desfase) y el bitrate se ajusta a la resolución. El archivo se nombra según la secuencia: `animacion-intro-…`, `animacion-outro-…`, `animacion-intro-outro-…`, `animacion-escudo-logo-escudo-…` o `animacion-solo-logo-…`. El video se exporta **sin audio**.

> 🔗 El logo de la animación se sincroniza con *Crear Logotipo* (incluido el color del bloque institucional): cualquier cambio allí se refleja al volver a esta herramienta. El color propio del bloque institucional dentro de *Crear Animación* tiene prioridad sobre el de *Crear Logotipo* solo en el video.

---

## 🪪 4. Crear Carnet

Carnet institucional de 648 × 1020 px (frente y reverso), exportable a **1296 × 2040 px** (2×).

| Módulo | Opciones |
|---|---|
| Frente | Nombre (se ajusta solo en varias líneas), etiqueta y número de ID, unidad |
| Foto | Carga PNG/JPG con zoom y desplazamiento dentro del círculo |
| Reverso — textos | Contacto, correo, **enlace del QR (Documentos)**, etiqueta bajo el QR, institución becaria, fechas y dirección |
| Reverso — imágenes | QR propio, logo izquierdo (institución) y logos del proyecto / derecho |
| Colores | Encabezado, acento y fondo del reverso; escudo de fondo activable |
| Exportar | Frente y reverso juntos o por separado |

**Logos preestablecidos.** El *logo del proyecto* (Proyecto Continuidad) y el *logo derecho* (Florecimiento Salvadoreño) son fijos y se cargan solos desde dos archivos que viven **al lado de `index.html`**:

| Archivo | Se usa como |
|---|---|
| `logoproyecto.png` | Logo del proyecto (centro del reverso) |
| `logo_derecho.png` | Logo derecho del reverso |

- Deben ser PNG con **fondo transparente** y texto en blanco, pensados para el fondo azul del reverso.
- Para mejorar la calidad, reemplázalos por versiones de mayor resolución **con el mismo nombre y la misma proporción**; no hay que tocar el código.
- Si abres `index.html` con doble clic (`file://`) el navegador no deja leer archivos externos; en ese caso la app usa una copia ligera incrustada. Para ver los archivos externos, usa GitHub Pages o un servidor local.
- Cada logo se puede cambiar o quitar desde el panel *Reverso — imágenes*, y hay un enlace para **restaurar el predeterminado**.

**QR automático (Documentos).** En *Reverso — textos* pega el enlace (por ejemplo, la carpeta de Drive del becario) y el QR se genera solo, en vectorial y listo para exportar. Si escribes un dominio sin `https://`, la app lo agrega. El generador va incrustado en `index.html`, así que funciona sin internet. Si el campo está vacío, se usa la imagen de QR subida (si hay) o un recuadro de marcador.

**Escudo de fondo del reverso.** Usa el escudo con su anillo de estrellas, con la misma posición y proporción de la plantilla oficial (centrado a la derecha y recortado por el borde de la tarjeta).

---

## ⚙️ Funcionamiento

```
  ┌─────────┐    ┌──────────────┐    ┌───────────────┐    ┌──────────┐
  │  Inicio │ →  │ Elegir       │ →  │ Configurar    │ →  │ Exportar │
  │         │    │ herramienta  │    │ en el panel   │    │ archivo  │
  └─────────┘    └──────────────┘    └───────────────┘    └──────────┘
```

| Característica | Descripción |
|---|---|
| 🖥️ 100 % en el navegador | No hay servidor; los archivos que subes no salen de tu equipo |
| 📦 Un solo archivo de código | Todo el código vive en `index.html`; los logos del carnet, el manual, el manifest y el service worker son archivos aparte |
| 🗂️ Módulos plegados | Todos los paneles inician cerrados para una interfaz limpia |
| 💾 Guardar / Cargar proyecto | Guarda tu configuración en el navegador y retómala después |
| ♻️ Restablecer | Vuelve a los valores iniciales |
| 🌗 Modo claro / oscuro | Botón de tema en la barra superior |
| 🛡️ Escudo vectorial oficial | Se mantiene nítido a cualquier tamaño |
| 📖 Manual de Uso de Marca | Botón en el inicio que abre el PDF del manual en una pestaña nueva |
| 📲 Instalable (PWA) | En Android se instala desde el menú del navegador, con el escudo como ícono; no muestra avisos propios |

---

## 📖 Manual de Uso de Marca

En la pantalla de inicio, bajo el título, hay un botón **«Manual de Uso de Marca 2019–2026»** que abre `MANUAL DE USO DE MARCA GOB 2019-2026.pdf` en una pestaña nueva.

- El PDF debe estar **en la misma carpeta que `index.html`** y llamarse exactamente `MANUAL DE USO DE MARCA GOB 2019-2026.pdf`.
- Si el archivo no está, la app muestra un aviso con el nombre que falta (en lugar de un error 404). Con `file://` el botón abre el PDF directamente.

---

## 📲 Instalar como aplicación (Android)

La web es una **PWA**: en Android, Chrome ofrece **⋮ → Instalar aplicación** y se instala con el escudo de `favicon.svg` como ícono. La app **no muestra avisos ni botones de instalación propios**; solo aparece la opción nativa del navegador.

| Archivo | Para qué sirve |
|---|---|
| `manifest.webmanifest` | Nombre, colores (`#001A70`), modo pantalla completa e íconos |
| `sw.js` | Service worker: hace la web instalable y permite abrirla sin conexión (red primero; si no hay red, la copia guardada) |
| `icon-192.png`, `icon-512.png` | Íconos generados desde `favicon.svg` |
| `icon-maskable-512.png` | Ícono adaptable de Android (escudo con margen sobre azul sólido) |

- Requiere **https** (GitHub Pages ya lo es) o `localhost`; con `file://` el service worker no se registra, pero la web funciona igual.
- Sin conexión la app abre, pero las tipografías de Google se reemplazan por las del sistema.
- Al subir una versión nueva, si el navegador sigue mostrando la anterior, cambia `CACHE = 'marca-goes-v1'` en `sw.js` (por ejemplo a `v2`).

---

## 📁 Estructura del repositorio

```
📦 repositorio
 ┣ 📄 index.html            ← aplicación completa
 ┣ 🖼️ logoproyecto.png      ← logo del proyecto (carnet, reverso)
 ┣ 🖼️ logo_derecho.png      ← logo derecho (carnet, reverso)
 ┣ 📕 MANUAL DE USO DE MARCA GOB 2019-2026.pdf  ← manual (botón del inicio)
 ┣ 🖼️ favicon.svg           ← ícono de la pestaña y de la app instalada
 ┣ 🖼️ favicon-32.png        ← ícono de la pestaña (respaldo)
 ┣ 🖼️ apple-touch-icon.png  ← ícono en celulares
 ┣ 🖼️ og-image.png          ← vista previa al compartir el enlace
 ┣ 📄 manifest.webmanifest  ← datos de la app instalable
 ┣ 📄 sw.js                 ← service worker (instalación y uso sin conexión)
 ┣ 🖼️ icon-192.png          ← ícono de la app (192 px)
 ┣ 🖼️ icon-512.png          ← ícono de la app (512 px)
 ┣ 🖼️ icon-maskable-512.png ← ícono adaptable de Android
 ┗ 📄 README.md
```

---

## 🚀 Cómo usarlo

**Opción A: en línea con GitHub Pages**

1. Sube todos los archivos a tu repositorio (incluidos `logoproyecto.png`, `logo_derecho.png`, el PDF del manual, `manifest.webmanifest`, `sw.js` y los íconos, todos en la misma carpeta que `index.html`).
2. Ve a **Settings → Pages**.
3. En *Source* elige la rama `main` y la carpeta `/ (root)`.
4. Abre `https://TU-USUARIO.github.io/TU-REPOSITORIO/`.

**Opción B: local**

1. Descarga el repositorio.
2. Abre `index.html` en tu navegador. (Para que el carnet use los logos externos de mayor calidad, sírvelo con un servidor local, por ejemplo `python -m http.server`, y abre `http://localhost:8000`.)

---

## 🔗 Vista previa al compartir

Al compartir el enlace aparecen el escudo, el título **Editor de Marca Institucional** y el texto *Gobierno de El Salvador · 2019–2026*. En la pestaña del navegador se muestra el escudo como ícono.

> Si ya habías compartido el enlace antes, WhatsApp y Facebook pueden tardar en actualizar la vista previa.

---

## ⚠️ Uso y aviso

```
┌──────────────────────────────────────────────────────────────┐
│  Uso exclusivo del Gobierno de El Salvador (2019–2026).      │
│                                                              │
│  La aplicación del emblema es obligatoria en los documentos  │
│  oficiales; su composición, proporciones y colores no deben  │
│  alterarse.                                                  │
└──────────────────────────────────────────────────────────────┘
```

<div align="center">

**Editor de Marca Institucional** · Gobierno de El Salvador

</div>
