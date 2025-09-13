# Plantillas Base - Tarjetas Románticas Personalizables

Este directorio contiene las plantillas base limpias y organizadas para crear tarjetas románticas personalizadas.

## 📁 Contenido de Plantillas

### `carta-nueva.html` - Tarjeta Interactiva con Modal
**Funcionalidad:** Tarjeta con botón "Abrir" que despliega un modal con foto y mensaje personalizado.

**Campos personalizables:**
- `{{TITULO_PERSONALIZADO}}` - Título de la página
- `{{IMAGEN_FONDO}}` - Archivo de imagen de fondo (en carpeta images/)
- `{{FOTO_PAREJA}}` - Foto principal en el modal (en carpeta images/)
- `{{NOMBRE_CLIENTE}}` - Nombre para el alt de la imagen
- `{{MENSAJE_PERSONALIZADO}}` - Mensaje principal del modal
- `{{ARCHIVO_MUSICA}}` - Archivo de música MP3 (en carpeta music/)
- `{{ARCHIVO_MUSICA_OGG}}` - Archivo de música OGG (opcional)
- `{{ARCHIVO_MUSICA_WAV}}` - Archivo de música WAV (opcional)

**Características:**
- ✅ Completamente responsive para móvil y desktop
- ✅ Modal interactivo con botón que desaparece al abrirse
- ✅ Corazones flotantes animados
- ✅ Música de fondo automática
- ✅ Compatibilidad cross-browser para audio

---

### `estandar1.html` - Tarjeta Clásica con Panel Transparente
**Funcionalidad:** Tarjeta elegante con panel transparente sobre imagen de fondo.

**Campos personalizables:**
- `{{TITULO_PERSONALIZADO}}` - Título principal
- `{{IMAGEN_FONDO}}` - Imagen de fondo (en carpeta images/)
- `{{MENSAJE_PERSONALIZADO}}` - Mensaje principal
- `{{FIRMA_PERSONALIZADA}}` - Firma o dedicatoria
- `{{ARCHIVO_MUSICA}}` - Archivo de música MP3 (en carpeta music/)
- `{{ARCHIVO_MUSICA_OGG}}` - Archivo de música OGG (opcional)
- `{{ARCHIVO_MUSICA_WAV}}` - Archivo de música WAV (opcional)

**Características:**
- ✅ Panel transparente con efecto blur
- ✅ Estrellas flotantes animadas
- ✅ Diseño responsivo optimizado
- ✅ Música de fondo automática
- ✅ Tipografía elegante y legible

---

### `estandar2.html` - Tarjeta Romántica Extendida
**Funcionalidad:** Tarjeta con mayor espacio para contenido, ideal para mensajes largos.

**Campos personalizables:**
- `{{TITULO_PERSONALIZADO}}` - Título principal
- `{{SUBTITULO_PERSONALIZADO}}` - Subtítulo o dedicatoria
- `{{IMAGEN_FONDO}}` - Imagen de fondo (en carpeta images/)
- `{{MENSAJE_PERSONALIZADO}}` - Mensaje extenso (soporta HTML)
- `{{PIE_PERSONALIZADO}}` - Pie de página o firma
- `{{ARCHIVO_MUSICA}}` - Archivo de música MP3 (en carpeta music/)
- `{{ARCHIVO_MUSICA_OGG}}` - Archivo de música OGG (opcional)
- `{{ARCHIVO_MUSICA_WAV}}` - Archivo de música WAV (opcional)

**Características:**
- ✅ Contenedor con scroll para mensajes largos
- ✅ Corazones flotantes con rotación
- ✅ Diseño elegante con bordes y sombras
- ✅ Música de fondo automática
- ✅ Responsive con ajustes específicos para móvil

---

## 🔧 Instrucciones de Personalización

### 1. Copia la plantilla deseada
```bash
# Ejemplo para un cliente llamado "ana-carlos"
mkdir ana-carlos
mkdir ana-carlos/images
mkdir ana-carlos/music
cp plantillas/carta-nueva.html ana-carlos/index.html
```

### 2. Reemplaza los marcadores de posición
En el archivo `index.html` del cliente, busca y reemplaza:

**Ejemplo para carta-nueva.html:**
```html
<!-- ANTES -->
<title>{{TITULO_PERSONALIZADO}}</title>
background: #fcb6b6 url('images/{{IMAGEN_FONDO}}') no-repeat center center fixed;
<img src="images/{{FOTO_PAREJA}}" alt="Foto de {{NOMBRE_CLIENTE}}" class="modal-foto" />
<p class="modal-mensaje">{{MENSAJE_PERSONALIZADO}}</p>
<source src="music/{{ARCHIVO_MUSICA}}" type="audio/mpeg">

<!-- DESPUÉS -->
<title>Para Ana ❤ Carlos</title>
background: #fcb6b6 url('images/fondo-pareja.jpg') no-repeat center center fixed;
<img src="images/ana-carlos.jpg" alt="Foto de Ana y Carlos" class="modal-foto" />
<p class="modal-mensaje">Mi amor, cada día contigo es una nueva aventura...</p>
<source src="music/nuestra-cancion.mp3" type="audio/mpeg">
```

### 3. Sube los archivos multimedia
- **Imágenes:** Coloca en `ana-carlos/images/`
  - Foto de fondo: `fondo-pareja.jpg`
  - Foto principal: `ana-carlos.jpg`
- **Música:** Coloca en `ana-carlos/music/`
  - Archivo principal: `nuestra-cancion.mp3`

### 4. Prueba localmente
Abre `ana-carlos/index.html` en el navegador para verificar que todo funcione correctamente.

---

## 📱 Características Técnicas

### Responsividad
- ✅ Diseño adaptativo para móviles y desktop
- ✅ Media queries optimizadas para pantallas pequeñas
- ✅ Controles táctiles compatibles con dispositivos móviles

### Audio
- ✅ Soporte para múltiples formatos (MP3, OGG, WAV)
- ✅ Reproducción automática con fallbacks para políticas del navegador
- ✅ Eventos múltiples para iniciar música (click, touch, pointer)

### Animaciones
- ✅ Elementos flotantes animados (corazones, estrellas)
- ✅ Efectos de entrada suaves
- ✅ Transiciones fluidas entre estados

### Compatibilidad
- ✅ Todos los navegadores modernos
- ✅ Dispositivos iOS y Android
- ✅ Políticas de autoplay de audio respetadas

---

## 🎨 Personalización Avanzada

### Colores
Para cambiar los colores de una plantilla, busca estos valores en el CSS:
- `#fcb6b6` - Rosa principal
- `#d72660` - Rosa oscuro
- `#fff` - Blanco
- `rgba(255, 255, 255, 0.2)` - Transparencias

### Tipografía
Las fuentes utilizadas:
- `'Arial Rounded MT Bold'` - Título principal
- `'Segoe Script'` - Botones (carta-nueva)
- `Arial, sans-serif` - Texto general

### Efectos
- **Blur:** `backdrop-filter: blur(10px)`
- **Sombras:** `box-shadow: 0 8px 32px rgba(...)`
- **Transparencias:** `rgba(255, 255, 255, 0.2)`

---

## 📦 Lista de Verificación por Cliente

- [ ] Crear carpeta del cliente: `nombre-cliente/`
- [ ] Crear subcarpetas: `images/` y `music/`
- [ ] Copiar plantilla elegida como `index.html`
- [ ] Reemplazar todos los marcadores `{{...}}`
- [ ] Subir imagen de fondo a `images/`
- [ ] Subir foto principal a `images/` (si aplica)
- [ ] Subir archivo de música a `music/`
- [ ] Probar en navegador local
- [ ] Probar en dispositivo móvil
- [ ] Subir a Vercel con URL personalizada

---

## 🚀 Notas para Deployment

### Para Vercel:
1. Cada carpeta de cliente es un proyecto independiente
2. La URL será: `https://nombre-cliente.vercel.app`
3. El archivo principal debe llamarse `index.html`
4. Las carpetas `images/` y `music/` se suben junto con `index.html`

### Archivos requeridos por carpeta de cliente:
```
nombre-cliente/
├── index.html          (plantilla personalizada)
├── images/
│   ├── fondo.jpg      (imagen de fondo)
│   └── foto.jpg       (foto principal, si aplica)
└── music/
    └── cancion.mp3    (música de fondo)
```

Esta estructura garantiza que cada cliente tenga su propia URL personalizada y todos los archivos necesarios para funcionamiento completo.