# Tarjetas Románticas Personalizadas 💕

Plataforma profesional para crear tarjetas digitales románticas personalizadas con música de fondo, efectos animados y diseño responsive. Ideal para negocios de detalles románticos y sorpresas digitales.

## 🚀 Características Principales

- ✅ **Plantillas Profesionales:** 3 diseños únicos completamente personalizables
- ✅ **Responsive Design:** Optimizado para móvil y desktop
- ✅ **Audio Integration:** Música de fondo con múltiples formatos de compatibilidad
- ✅ **Efectos Animados:** Corazones y estrellas flotantes
- ✅ **Deploy Ready:** Estructura lista para Vercel con URLs personalizadas
- ✅ **Per-Client Folders:** Sistema organizado para múltiples clientes

## 📁 Estructura del Proyecto

```
tarjetas-parejas/
├── README.md                    # Este archivo
├── plantillas/                  # Plantillas base limpias
│   ├── README.md               # Documentación de plantillas
│   ├── carta-nueva.html        # Tarjeta interactiva con modal
│   ├── estandar1.html          # Tarjeta clásica con panel transparente
│   └── estandar2.html          # Tarjeta romántica extendida
├── ejemplo-cliente/             # Ejemplo completo de implementación
│   ├── README.md               # Documentación del ejemplo
│   ├── index.html              # Tarjeta personalizada para Ana y Carlos
│   ├── images/                 # Carpeta de imágenes del cliente
│   └── music/                  # Carpeta de música del cliente
└── archivos-originales/         # Archivos de desarrollo históricos
    ├── estandar1.html
    ├── estandar2.html
    ├── carta-nueva.html
    └── flore.html
```

## 🎯 Tipos de Tarjetas Disponibles

### 1. **Carta Interactiva** (`carta-nueva.html`)
- **Funcionalidad:** Botón "Abrir" que despliega modal con foto y mensaje
- **Ideal para:** Cartas de amor, propuestas, aniversarios
- **Efectos:** Corazones flotantes, música automática
- **Mobile:** Completamente optimizada

### 2. **Tarjeta Clásica** (`estandar1.html`)
- **Funcionalidad:** Panel transparente elegante sobre imagen de fondo
- **Ideal para:** Mensajes simples, dedicatorias, saludos
- **Efectos:** Estrellas flotantes, música automática
- **Mobile:** Diseño adaptativo

### 3. **Tarjeta Extendida** (`estandar2.html`)
- **Funcionalidad:** Contenedor amplio para mensajes largos
- **Ideal para:** Cartas extensas, poemas, declaraciones
- **Efectos:** Corazones rotatorios, música automática
- **Mobile:** Scroll vertical si es necesario

## 🛠️ Guía de Uso Rápido

### Para Usuarios (Crear nueva tarjeta):

1. **Elegir plantilla** desde `plantillas/`
2. **Crear carpeta del cliente:** `nombre-cliente/`
3. **Copiar plantilla:** `cp plantillas/carta-nueva.html nombre-cliente/index.html`
4. **Personalizar marcadores:** Reemplazar `{{TITULO_PERSONALIZADO}}`, etc.
5. **Subir archivos:** Agregar imágenes y música a subcarpetas
6. **Deploy a Vercel:** Una carpeta = un proyecto

### Para Desarrolladores:

```bash
# Clonar repositorio
git clone [repository-url]
cd tarjetas-parejas

# Revisar ejemplo completo
cd ejemplo-cliente
# Abrir index.html en navegador

# Crear nuevo cliente
mkdir nuevo-cliente
mkdir nuevo-cliente/images
mkdir nuevo-cliente/music
cp plantillas/carta-nueva.html nuevo-cliente/index.html

# Personalizar y deployar
# Seguir documentación en plantillas/README.md
```

## 📋 Campos Personalizables

Cada plantilla incluye marcadores que se deben reemplazar:

### Universales:
- `{{TITULO_PERSONALIZADO}}` - Título de la página
- `{{IMAGEN_FONDO}}` - Imagen de fondo (en images/)
- `{{ARCHIVO_MUSICA}}` - Música principal MP3 (en music/)
- `{{ARCHIVO_MUSICA_OGG}}` - Música OGG (opcional)
- `{{ARCHIVO_MUSICA_WAV}}` - Música WAV (opcional)

### Específicos por Plantilla:
- **carta-nueva.html:** `{{FOTO_PAREJA}}`, `{{NOMBRE_CLIENTE}}`, `{{MENSAJE_PERSONALIZADO}}`
- **estandar1.html:** `{{MENSAJE_PERSONALIZADO}}`, `{{FIRMA_PERSONALIZADA}}`
- **estandar2.html:** `{{SUBTITULO_PERSONALIZADO}}`, `{{MENSAJE_PERSONALIZADO}}`, `{{PIE_PERSONALIZADO}}`

## 🌐 Deployment en Vercel

### Configuración por Cliente:

1. **Una carpeta = Un proyecto Vercel**
2. **URL personalizada:** `nombre-cliente.vercel.app`
3. **Archivos requeridos por cliente:**
   ```
   cliente/
   ├── index.html    (plantilla personalizada)
   ├── images/       (fotos y fondos)
   └── music/        (música de fondo)
   ```

### Comandos Vercel CLI:
```bash
# Instalar Vercel CLI
npm i -g vercel

# Navegar a carpeta del cliente
cd nombre-cliente/

# Deploy
vercel --prod

# Configurar dominio personalizado
vercel domains add nombre-cliente.vercel.app
```

## � Modelo de Negocio Implementado

### Estructura de Costos:
- **Vercel Free Tier:** 100GB bandwidth/mes, proyectos ilimitados
- **Costo por cliente:** $0 (dentro del límite gratuito)
- **Escalabilidad:** Perfecto para negocios de detalles románticos

### Beneficios vs Netlify:
- ❌ **Netlify:** $19/mes después de límites
- ✅ **Vercel:** Gratis hasta 100GB total
- ✅ **URLs personalizadas ilimitadas**
- ✅ **Deploy automático desde GitHub**

## 📱 Características Técnicas

### Compatibilidad:
- ✅ **Mobile-first responsive design**
- ✅ **Cross-browser compatibility** (Chrome, Safari, Firefox, Edge)
- ✅ **Touch-friendly controls**
- ✅ **iOS y Android optimizado**

### Audio:
- ✅ **Múltiples formatos** (MP3, OGG, WAV)
- ✅ **Autoplay con fallbacks** para políticas del navegador
- ✅ **Eventos múltiples** para iniciar música

### Efectos:
- ✅ **CSS3 animations** con hardware acceleration
- ✅ **Elementos flotantes** con physics básicas
- ✅ **Transiciones fluidas** entre estados

## 🔧 Personalización Avanzada

### Colores del Tema:
```css
/* Rosa principal */
#fcb6b6

/* Rosa oscuro */
#d72660

/* Transparencias */
rgba(255, 255, 255, 0.2)
```

### Tipografías:
- **Títulos:** 'Arial Rounded MT Bold'
- **Botones:** 'Segoe Script', 'Comic Sans MS'
- **Texto:** Arial, sans-serif

## 📞 Soporte y Documentación

- **Documentación completa:** Ver `plantillas/README.md`
- **Ejemplo funcional:** Ver `ejemplo-cliente/`
- **Troubleshooting:** Issues conocidos y soluciones en documentación

## 🚀 Próximos Pasos

1. **Completar migración a GitHub** (en progreso)
2. **Configurar CI/CD** para deploy automático
3. **Crear más plantillas** temáticas
4. **Agregar admin panel** para personalización sin código

---

## ⭐ Estado del Proyecto

- ✅ **Plantillas:** 3 diseños listos y documentados
- ✅ **Responsividad:** Optimizado para todos los dispositivos
- ✅ **Compatibilidad Audio:** Testado cross-platform
- ✅ **Estructura de Negocio:** Lista para escalabilidad
- 🟡 **GitHub Setup:** En proceso
- 🟡 **Vercel Migration:** Pendiente
- 🟡 **Client Workflow:** Documentado, pendiente de testing

**Última actualización:** Diciembre 2024
**Versión:** 2.0 - Business Ready