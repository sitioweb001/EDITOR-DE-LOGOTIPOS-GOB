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
```

| Herramienta | Qué hace | Resultado |
|---|---|---|
| **Insertar Marca de Agua** | Coloca el escudo, el logo del ministerio o texto (*Documento Oficial*, *Borrador*, *Confidencial*) sobre un PDF | PDF con marca de agua |
| **Crear Logotipo** | Compone un logotipo horizontal o vertical: escudo + hasta 3 bloques (ministerio, dirección, unidad) | Logotipo institucional |
| **Crear Animación** | Genera un video de intro u outro estilo Cadena Nacional | Archivo de video real |

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

**Panel de controles** (todos los módulos inician plegados):

| Módulo | Para qué sirve |
|---|---|
| Guía de marca | Referencia rápida del manual |
| Institucional | Escudo oficial vectorial, orientación (vertical / horizontal) y opción de usar tu propia imagen |
| Bloques | Hasta 3 bloques de texto: ministerio, dirección y unidad |
| Tipografía | Fuente, tamaño y fuente personalizada |
| Separadores | Líneas divisorias entre bloques |
| Color | Color global del logotipo (por defecto azul oficial `#001A70`) |
| Subcolor | Color independiente por bloque |
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
| **Tipo de video** | Intro u Outro |
| **Animaciones** | Efectos de revelado y transición |
| **Contenido** | Usa automáticamente el logotipo creado en *Crear Logotipo*; color del escudo al revelarse (fase inicial) y colores del logo completo |
| **Fondo** | Color (paleta o personalizado en HEX) o imagen |
| **Duración y resolución** | Duración con deslizador (ej. 6.0 s) y resolución de salida |
| **Exportar** | Genera el archivo de video |

> 🔗 El logo de la animación se sincroniza con *Crear Logotipo*: cualquier cambio allí se refleja al volver a esta herramienta.

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
| 📦 Un solo archivo | Todo el código vive en `index.html` |
| 🗂️ Módulos plegados | Todos los paneles inician cerrados para una interfaz limpia |
| 💾 Guardar / Cargar proyecto | Guarda tu configuración en el navegador y retómala después |
| ♻️ Restablecer | Vuelve a los valores iniciales |
| 🌗 Modo claro / oscuro | Botón de tema en la barra superior |
| 🛡️ Escudo vectorial oficial | Se mantiene nítido a cualquier tamaño |

---

## 📁 Estructura del repositorio

```
📦 repositorio
 ┣ 📄 index.html            ← aplicación completa
 ┣ 🖼️ favicon.svg           ← ícono de la pestaña
 ┣ 🖼️ favicon-32.png        ← ícono de la pestaña (respaldo)
 ┣ 🖼️ apple-touch-icon.png  ← ícono en celulares
 ┣ 🖼️ og-image.png          ← vista previa al compartir el enlace
 ┗ 📄 README.md
```

---


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
