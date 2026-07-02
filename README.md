# Inspector PNA — Inspecciones Ordinarias de Seguridad

**Prefectura Naval Argentina · Dirección de Policía de Seguridad de la Navegación**

Sistema digital para la realización de inspecciones ordinarias de seguridad a bordo, basado en el Reglamento General PNA 4-016. Funciona como aplicación instalable en celular o computadora, sin necesidad de internet una vez instalada.

---

## 📋 ¿Qué hace esta app?

- Genera el **checklist de inspección** automáticamente según la especialidad (Radio, Casco, Máquinas, Electricidad, Equipo, Ambiental) y el tipo de inspección (inicial, renovación, anual, intermedia) conforme al RG PNA 4-016
- Permite registrar **deficiencias** con código oficial (Formulario B/2 – RG PNA 3-036) y **medida adoptada** (código 00 al 99)
- Permite adjuntar **fotos** a cada deficiencia
- Guarda el **historial** de todas las inspecciones realizadas
- Exporta el **acta de inspección** en formato Word (.docx) con ítems conformes y deficiencias
- Funciona **100% offline** en celular y computadora

---

## 📱 Instalación en iPhone / iPad

> ⚠️ **Importante:** en iOS, la instalación solo funciona desde **Safari**. No usar Chrome ni Firefox.

1. Abrí **Safari** en tu iPhone o iPad
2. Ingresá a la dirección de la app: `https://[TU-USUARIO].github.io/inspector-pna/`
3. Tocá el botón de **compartir** (el ícono de cuadrado con flecha ↑, en la barra inferior)
4. Scrolleá hacia abajo en el menú y tocá **"Agregar a pantalla de inicio"**
5. Confirmá el nombre y tocá **"Agregar"**
6. El ícono de la PNA aparece en tu pantalla de inicio como cualquier app

> La primera vez que abrás la app necesitás conexión a internet para que se descarguen todos los archivos. Después funciona sin conexión.

---

## 🤖 Instalación en Android

1. Abrí **Chrome** en tu celular Android
2. Ingresá a la dirección de la app: `https://[TU-USUARIO].github.io/inspector-pna/`
3. Chrome muestra automáticamente un banner en la parte inferior: tocá **"Instalar"** o **"Agregar a pantalla de inicio"**
4. Si no aparece el banner: tocá los **tres puntos** (⋮) arriba a la derecha → **"Agregar a pantalla de inicio"**
5. Confirmá y listo

---

## 💻 Instalación en computadora (Windows / Mac)

1. Abrí **Chrome** o **Edge** en tu computadora
2. Ingresá a la dirección de la app
3. En la barra de direcciones aparece un ícono de instalación (⊕) a la derecha — hacé clic
4. Confirmá la instalación
5. La app queda disponible como acceso directo en el escritorio

---

## 🚀 Cómo usar la app

### Primera vez
1. Tocá el chip **"Configurar inspector"** arriba e ingresá tu nombre, legajo y dependencia. Esto queda guardado para todas las inspecciones.

### Nueva inspección
1. Tocá **"+ Nueva inspección"**
2. Completá los datos del buque (nombre, matrícula, tipo, eslora, AB, kW, etc.)
3. Indicá el **lugar** y la **fecha** de la inspección
4. Seleccioná las **especialidades** a inspeccionar
5. Para cada especialidad, elegí el **tipo de inspección** según el RG PNA 4-016
6. Tocá **"Generar checklist"**

### Durante la inspección
- **✓** = Ítem conforme
- **✗** = Deficiencia detectada (abre el registro de deficiencia)
- **–** = No aplica

Al registrar una deficiencia podés indicar:
- Código de deficiencia (Formulario B/2)
- Medida adoptada (código 00–99)
- Observación del inspector
- Fotos

### Exportar el acta
- Tocá **"Ver acta"** durante la inspección o desde el historial
- Tocá **"Exportar"** para descargar el acta en Word (.docx)

El documento incluye:
1. Datos del buque, inspector, lugar, fecha y alcance de la inspección
2. Resumen numérico
3. Todos los ítems conformes, agrupados por especialidad y sección
4. Todas las deficiencias detectadas con código, medida adoptada y observaciones

---

## 📁 Archivos del repositorio

| Archivo | Descripción |
|---|---|
| `index.html` | La aplicación completa |
| `manifest.json` | Configuración de la PWA (nombre, ícono, colores) |
| `sw.js` | Service Worker — permite el funcionamiento offline |
| `docx.umd.js` | Librería para generar archivos Word (sin internet) |
| `icon-192.png` | Ícono de la app (pantalla de inicio) |
| `icon-512.png` | Ícono de la app (alta resolución) |

---

## ⚙️ Base normativa

- **RG PNA 4-016** — Normas de Inspección de Buques (Caps. I a VI)
- **RG PNA 3-036** — Formulario B/2, Códigos de Deficiencias y Medidas Adoptadas
- **Ordenanzas DPSN** — Tomo 1 al Tomo 6 (Régimen Técnico, Administrativo, Operativo, Náutico-Deportivo y Prevención de la Contaminación)

---

## 🔒 Privacidad y datos

Todos los datos de las inspecciones se almacenan **exclusivamente en el dispositivo del inspector** (IndexedDB local). No se envía ningún dato a servidores externos. Al desinstalar la app o borrar los datos del navegador, se eliminan todas las inspecciones guardadas.

---

*Desarrollado para uso interno de la Dirección de Policía de Seguridad de la Navegación — PNA*
