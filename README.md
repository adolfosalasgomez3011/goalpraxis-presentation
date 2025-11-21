# GoalPraxis - Presentación de Validación de Mercado

## 📌 Descripción

Presentación profesional para validación de mercado en la industria minera. Incluye 14 slides HTML optimizadas para web y dispositivos móviles.

## 🎯 Contenido de la Presentación

### Estructura (14 Slides)

1. **Portada** - Transforming Mining through IoT, Analytics, and AI
2. **Erick Enríquez** - Co-Fundador | Telecomunicaciones & IoT
3. **Mauricio San Roman** - Co-Fundador | Telecomunicaciones & IoT
4. **Adolfo Salas** - Co-Fundador | Minería & Energía | Hatch Partner
5. **Desafíos** - Problemas operacionales de la industria
6. **Solución** - Modelo SolaaS (Consultoría → Implementación → Operación)
7. **Valor** - Propuesta de valor y beneficios
8. **Diferenciación** - Ventajas competitivas
9. **Modelo de Negocio** - 4 flujos de ingresos
10. **Go-to-Market** - Estrategia de entrada en 3 fases
11. **Ecosistema** - Partners tecnológicos (IoT, Cloud, Analytics, OEMs)
12. **Validación** - 7 preguntas clave para expertos
13. **Agradecimiento** - Fase de validación
14. **Cierre Dinámico** - Call to action y contacto

## 🚀 Deployment en Vercel

### Archivos Necesarios

```
HTML_Full/
├── presentation_complete.html    ← Archivo principal
├── index.html                     ← Landing page
├── slide_01_title.html
├── slide_02_cv_erick.html
├── slide_03_cv_mauricio.html
├── slide_04_cv_adolfo.html
├── slide_05_problem.html
├── slide_06_solution.html
├── slide_07_value.html
├── slide_08_differentiation.html
├── slide_09_business_model.html
├── slide_10_gtm.html
├── slide_11_ecosystem.html
├── slide_12_validation_questions.html
├── slide_13_thank_you.html
└── slide_14_closing.html
```

### También Incluir

```
Logos/
└── logo_variant_4.png    ← Logo de GoalPraxis (usado en footer y cierre)
```

### Pasos para Deploy

1. **Crear repositorio en Vercel**
   ```bash
   # Opción 1: Deploy directo desde carpeta local
   cd HTML_Full
   vercel
   
   # Opción 2: Deploy desde GitHub
   # Push la carpeta HTML_Full a tu repositorio
   # Conecta el repo en Vercel Dashboard
   ```

2. **Configuración de Vercel**
   - Root Directory: `HTML_Full` (o `/` si subes solo esta carpeta)
   - Build Command: (ninguno - es HTML estático)
   - Output Directory: (vacío - usa el root)

3. **Variables de entorno**: No necesarias

4. **Dominio personalizado** (opcional):
   - Configura en Vercel Dashboard
   - Ejemplo: `presentation.goalpraxis.com`

## 📱 Características Técnicas

- **Dimensiones**: 1080x720 pixels (aspect ratio 3:2)
- **Responsive**: Auto-escalado para mobile, tablet, desktop
- **Navegación**:
  - Teclado: ← → flechas, Home, End, Espacio
  - Mouse: Botones en pantalla
  - Touch: Menú lateral con puntos
- **Tecnologías**: HTML5, CSS3, Vanilla JavaScript
- **Compatibilidad**: Chrome, Firefox, Safari, Edge
- **No requiere**: Frameworks, librerías externas, Node.js, build process

## 🎨 Paleta de Colores

- **Azul**: `#1E40AF` / `#3B82F6` (Telecomunicaciones/IoT)
- **Verde**: `#16A34A` / `#22C55E` (Operación/Sostenibilidad)
- **Púrpura**: `#7C3AED` / `#A78BFA` (Minería/Energía)
- **Naranja**: `#F59E0B` / `#EF4444` (Call to Action)
- **Fondo oscuro**: `#0F172A` / `#1E293B`
- **Fondo claro**: `#F8FAFC` / `#E2E8F0`

## 👥 Equipo

- **Erick Enríquez**: MBA, Telecomunicaciones, 25+ años experiencia, 5 directorios
- **Mauricio San Roman**: MBA, Telecomunicaciones, 25+ años experiencia
- **Adolfo Salas**: Wharton Executive, Mining/Energy, 24+ años, Hatch Partner, USD 350M+ revenue

## 📧 Contacto

- **Website**: www.goalpraxis.com
- **Email**: contacto@goalpraxis.com

## 📄 Licencia

© 2025 GoalPraxis Technology. Todos los derechos reservados.

## 🔧 Notas Técnicas

### Estructura de Archivos para Vercel

```
proyecto-vercel/
├── HTML_Full/
│   ├── presentation_complete.html
│   ├── index.html
│   └── slide_*.html
└── Logos/
    └── logo_variant_4.png
```

### Ruta del Logo

En los HTML files, el logo se referencia como:
```html
<img src="../../Logos/logo_variant_4.png" alt="GoalPraxis">
```

**Importante**: Mantén la estructura de carpetas exacta para que las rutas relativas funcionen correctamente.

### Optimización para Producción

- ✅ Minificación no necesaria (HTML simple)
- ✅ Lazy loading no necesario (slides cargan bajo demanda)
- ✅ CDN automático de Vercel
- ✅ HTTPS automático
- ✅ Compresión Gzip automática

### Performance

- **Tamaño total**: ~100 KB (14 HTML files + 1 PNG logo)
- **Primera carga**: < 1 segundo
- **Navegación entre slides**: Instantánea
- **Mobile**: 100% responsive

---

**Última actualización**: Enero 2025  
**Versión**: 1.0  
**Propósito**: Validación de mercado con expertos mineros