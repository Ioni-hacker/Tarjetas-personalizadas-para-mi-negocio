# Ejemplo Cliente: Ana y Carlos

Este es un ejemplo completo de implementación para un cliente, mostrando cómo personalizar una plantilla base para crear una tarjeta romántica única.

## 📂 Estructura de Archivos

```
ejemplo-cliente/
├── index.html          # Tarjeta personalizada (basada en carta-nueva.html)
├── images/
│   ├── fondo-pareja.jpg    # Imagen de fondo personalizada
│   └── ana-carlos.jpg      # Foto principal de la pareja
├── music/
│   ├── nuestra-cancion.mp3 # Música de fondo principal
│   ├── nuestra-cancion.ogg # Música de fondo (formato alternativo)
│   └── nuestra-cancion.wav # Música de fondo (formato alternativo)
└── README.md           # Este archivo
```

## 🎨 Personalizaciones Aplicadas

### Información del Cliente
- **Nombres:** Ana y Carlos
- **Plantilla base:** `carta-nueva.html` (tarjeta interactiva con modal)
- **Tema:** Romántico con corazones flotantes
- **Color principal:** Rosa (#fcb6b6)

### Elementos Personalizados

#### 1. Título de la Página
```html
<title>Para Ana ❤ Carlos</title>
```

#### 2. Imagen de Fondo
```css
background: #fcb6b6 url('images/fondo-pareja.jpg') no-repeat center center fixed;
```

#### 3. Foto Principal
```html
<img src="images/ana-carlos.jpg" alt="Foto de Ana y Carlos" class="modal-foto" />
```

#### 4. Mensaje Personalizado
```html
<p class="modal-mensaje">
Mi amor, cada día contigo es una nueva aventura. Tu sonrisa ilumina mis mañanas y tu amor llena mi corazón de felicidad infinita. Gracias por ser mi compañera de vida, mi mejor amiga y mi gran amor. ❤️
</p>
```

#### 5. Música de Fondo
```html
<source src="music/nuestra-cancion.mp3" type="audio/mpeg">
<source src="music/nuestra-cancion.ogg" type="audio/ogg">
<source src="music/nuestra-cancion.wav" type="audio/wav">
```

## 🚀 Instrucciones de Deployment

### Para Vercel:
1. **Crear proyecto nuevo en Vercel**
2. **Subir esta carpeta completa**
3. **Configurar dominio personalizado:** `ana-carlos.vercel.app`
4. **Verificar que todos los archivos se suban correctamente**

### Comandos de Vercel CLI:
```bash
# Navegar a la carpeta del cliente
cd ejemplo-cliente/

# Deployar a Vercel
vercel --prod

# Configurar dominio personalizado
vercel domains add ana-carlos.vercel.app
```

## ✅ Lista de Verificación

### Antes del Deploy:
- [x] Archivo `index.html` personalizado
- [x] Imagen de fondo en `images/fondo-pareja.jpg`
- [x] Foto de la pareja en `images/ana-carlos.jpg`
- [x] Música en `music/nuestra-cancion.mp3`
- [x] Todos los marcadores `{{...}}` reemplazados
- [x] Prueba local exitosa

### Después del Deploy:
- [ ] URL funciona correctamente
- [ ] Imágenes se cargan sin errores
- [ ] Música reproduce automáticamente
- [ ] Funcionalidad móvil correcta
- [ ] Modal se abre y cierra correctamente
- [ ] Botón desaparece al abrir carta

## 📱 Características Implementadas

### Funcionalidad Principal:
- ✅ **Botón "Abrir"** centrado sobre imagen de fondo
- ✅ **Modal interactivo** que se despliega al hacer clic
- ✅ **Foto de la pareja** mostrada en el modal
- ✅ **Mensaje romántico personalizado**
- ✅ **Música de fondo** que inicia automáticamente

### Responsividad:
- ✅ **Mobile-first design** optimizado para teléfonos
- ✅ **Botón adaptativo** que se ajusta al tamaño de pantalla
- ✅ **Modal responsive** con scroll si es necesario
- ✅ **Imágenes adaptativas** que mantienen proporción

### Animaciones:
- ✅ **Corazones flotantes** animados continuamente
- ✅ **Efectos de entrada** suaves para el modal
- ✅ **Transiciones fluidas** en botones y elementos

### Compatibilidad:
- ✅ **Multi-browser support** (Chrome, Safari, Firefox, Edge)
- ✅ **Cross-platform audio** con múltiples formatos
- ✅ **Touch-friendly** para dispositivos móviles

## 🎯 URL Final

Una vez deployado en Vercel, la tarjeta estará disponible en:
**https://ana-carlos.vercel.app**

## 💡 Notas para el Cliente

### Cómo usar:
1. **Abrir la URL** en cualquier dispositivo
2. **Hacer clic en "Abrir"** para ver la tarjeta
3. **Disfrutar** de la música y animaciones
4. **Compartir la URL** con quien quieran

### Compatibilidad:
- ✅ Funciona en todos los teléfonos modernos
- ✅ Compatible con navegadores de escritorio
- ✅ La música puede requerir interacción del usuario en algunos navegadores (política de autoplay)

---

**Este ejemplo sirve como referencia para crear tarjetas similares para otros clientes, simplemente replicando el proceso de personalización con sus propios contenidos.**