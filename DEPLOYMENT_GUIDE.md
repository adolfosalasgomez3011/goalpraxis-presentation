# 🚀 Guía de Deployment - GoalPraxis Presentación

## ✅ Archivos Listos para Vercel

Tu presentación está **100% lista** para deployment. Todos los archivos necesarios están en:
```
BusinessPlan/Presentations/HTML_Full/
```

---

## 📦 Estructura del Proyecto

```
GoalPraxis/
├── BusinessPlan/
│   └── Presentations/
│       └── HTML_Full/                    ← CARPETA PRINCIPAL
│           ├── index.html                ← Landing page con navegación
│           ├── presentation_complete.html ← Presentación completa (RECOMENDADA)
│           ├── slide_01_title.html       ← Portada (PowerPoint integrado)
│           ├── slide_02_cv_erick.html    ← CV Erick Enríquez
│           ├── slide_03_cv_mauricio.html ← CV Mauricio San Roman
│           ├── slide_04_cv_adolfo.html   ← CV Adolfo Salas
│           ├── slide_05_problem.html     ← Desafíos de la industria
│           ├── slide_06_solution.html    ← Modelo SolaaS
│           ├── slide_07_value.html       ← Propuesta de valor
│           ├── slide_08_differentiation.html ← Diferenciadores
│           ├── slide_09_business_model.html  ← Modelo de negocio
│           ├── slide_10_gtm.html         ← Go-to-Market
│           ├── slide_11_ecosystem.html   ← Ecosistema de partners
│           ├── slide_12_validation_questions.html ← 7 preguntas clave
│           ├── slide_13_thank_you.html   ← Agradecimiento
│           ├── slide_14_closing.html     ← Cierre dinámico con logo
│           ├── vercel.json               ← Configuración de Vercel
│           └── README.md                 ← Documentación técnica
└── Logos/
    └── logo_variant_4.png                ← Logo GoalPraxis
```

---

## 🎯 Opción 1: Deploy con Vercel CLI (Más Rápido)

### Paso 1: Instalar Vercel CLI
```bash
npm install -g vercel
```

### Paso 2: Login en Vercel
```bash
vercel login
```

### Paso 3: Deploy
```bash
cd "c:/Users/USER/OneDrive/GoalPraxis"
vercel
```

### Paso 4: Seguir el Wizard
- **Set up and deploy?** → Yes
- **Which scope?** → Selecciona tu cuenta/organización
- **Link to existing project?** → No
- **Project name?** → goalpraxis-presentation (o el nombre que prefieras)
- **In which directory is your code located?** → `./BusinessPlan/Presentations/HTML_Full`
- **Want to override settings?** → No

### Paso 5: Deploy a Producción
```bash
vercel --prod
```

✅ **Listo!** Vercel te dará una URL como: `https://goalpraxis-presentation.vercel.app`

---

## 🎯 Opción 2: Deploy con Vercel Dashboard (Sin CLI)

### Paso 1: Preparar Archivos
1. Abre tu explorador de archivos
2. Ve a: `c:\Users\USER\OneDrive\GoalPraxis\`
3. Crea una carpeta temporal: `vercel-deploy`
4. Copia estas carpetas dentro:
   - `BusinessPlan\Presentations\HTML_Full\` (todo el contenido)
   - `Logos\` (solo la carpeta completa)

Tu estructura temporal debería verse así:
```
vercel-deploy/
├── HTML_Full/
│   ├── index.html
│   ├── presentation_complete.html
│   ├── slide_*.html
│   ├── vercel.json
│   └── README.md
└── Logos/
    └── logo_variant_4.png
```

### Paso 2: Subir a GitHub (Recomendado)

#### 2.1: Crear Repositorio en GitHub
1. Ve a https://github.com/new
2. Nombre: `goalpraxis-presentation`
3. Descripción: "GoalPraxis Market Validation Presentation"
4. Público o Privado (tu elección)
5. **NO** inicializar con README
6. Click "Create repository"

#### 2.2: Push tu código
```bash
cd vercel-deploy
git init
git add .
git commit -m "Initial commit: GoalPraxis presentation for Vercel"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/goalpraxis-presentation.git
git push -u origin main
```

### Paso 3: Conectar con Vercel
1. Ve a https://vercel.com/
2. Click "Add New..." → "Project"
3. Import tu repositorio de GitHub
4. **Root Directory**: Déjalo en raíz `/` (ya que subiste todo junto)
5. **Framework Preset**: Other
6. **Build Command**: (dejar vacío)
7. **Output Directory**: (dejar vacío)
8. Click "Deploy"

✅ **Listo!** En 30-60 segundos estará desplegado.

---

## 🎯 Opción 3: Deploy Drag & Drop (Más Simple)

### Paso 1: Comprimir Archivos
1. Crea la carpeta `vercel-deploy` como en Opción 2
2. Comprime en un archivo `.zip`

### Paso 2: Upload en Vercel
1. Ve a https://vercel.com/new
2. Arrastra el archivo `.zip` a la ventana
3. Vercel lo procesa automáticamente
4. Click "Deploy"

✅ **Listo!** En minutos estará en línea.

---

## 🔧 Configuración Post-Deploy

### URLs Disponibles

Después del deploy, tendrás acceso a:

- **Landing Page**: `https://tu-proyecto.vercel.app/`
- **Presentación Completa**: `https://tu-proyecto.vercel.app/presentation_complete.html`
- **Shortcut**: `https://tu-proyecto.vercel.app/presentacion` (redirige a la presentación)
- **Slides Individuales**: `https://tu-proyecto.vercel.app/slide_01_title.html`

### Dominio Personalizado (Opcional)

1. En Vercel Dashboard, ve a tu proyecto
2. Settings → Domains
3. Add Domain
4. Ingresa tu dominio (ej: `presentation.goalpraxis.com`)
5. Sigue las instrucciones para configurar DNS

### Variables de Entorno

No se requieren variables de entorno para este proyecto (es HTML estático).

---

## 🎨 Personalización Final

### Actualizar Logo
Si quieres cambiar el logo:
1. Reemplaza `Logos/logo_variant_4.png`
2. Mantén el nombre del archivo o actualiza las referencias en:
   - `slide_01_title.html` (footer)
   - `slide_02_cv_erick.html` (footer)
   - `slide_03_cv_mauricio.html` (footer)
   - `slide_04_cv_adolfo.html` (footer)
   - `slide_14_closing.html` (logo principal y footer)

### Actualizar Contacto
Edita `slide_14_closing.html`:
```html
<div class="contact-info">
    www.goalpraxis.com<br>
    contacto@goalpraxis.com
</div>
```

---

## 📱 Testing Post-Deploy

### Checklist de Verificación

- [ ] Landing page carga correctamente
- [ ] Botón "Ver Presentación Completa" funciona
- [ ] Navegación con flechas del teclado funciona (← →)
- [ ] Menú lateral con puntos funciona
- [ ] Logo aparece en slides 1, 2, 3, 4 y 14
- [ ] Todas las 14 slides cargan correctamente
- [ ] Responsive en móvil (prueba en tu celular)
- [ ] CV slides muestran información correcta de cada fundador

### Dispositivos para Probar
- Desktop (Chrome, Firefox, Safari, Edge)
- Tablet (iPad, Android)
- Mobile (iPhone, Android)

---

## 🐛 Troubleshooting

### Problema: Logo no aparece

**Causa**: Ruta relativa incorrecta
**Solución**: Asegúrate de que la carpeta `Logos` esté en el mismo nivel que `HTML_Full` en Vercel

Estructura correcta:
```
vercel-root/
├── HTML_Full/
└── Logos/
```

Si colocaste solo `HTML_Full` como root, modifica las rutas en los HTML de:
```html
<img src="../../Logos/logo_variant_4.png">
```
A:
```html
<img src="../Logos/logo_variant_4.png">
```

### Problema: Slides no cargan en presentation_complete.html

**Causa**: Rutas de iframe incorrectas
**Solución**: Verifica que todos los archivos `slide_*.html` estén en la misma carpeta que `presentation_complete.html`

### Problema: Navegación con teclado no funciona

**Causa**: JavaScript deshabilitado o conflicto de eventos
**Solución**: Abre la consola del navegador (F12) y busca errores en JavaScript

---

## 📊 Analytics (Opcional)

Para agregar Google Analytics:

1. Edita `presentation_complete.html`
2. Agrega antes del `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

3. Reemplaza `G-XXXXXXXXXX` con tu ID de Analytics

---

## 🔐 Seguridad

El archivo `vercel.json` incluye headers de seguridad básicos:
- `X-Content-Type-Options: nosniff`
- `X-Frame-Options: SAMEORIGIN`
- `X-XSS-Protection: 1; mode=block`

Para producción, considera agregar:
- HTTPS (automático en Vercel)
- CSP (Content Security Policy)
- CORS policy si planeas embedar en otros sitios

---

## 📈 Performance

Optimizaciones ya aplicadas:
- ✅ HTML estático (carga ultra rápida)
- ✅ CSS inline (no requests externos)
- ✅ JavaScript vanilla (sin frameworks pesados)
- ✅ Slides bajo demanda (iframe lazy loading)
- ✅ Responsive images
- ✅ Vercel CDN automático

**Resultado esperado:**
- First Contentful Paint: < 1 segundo
- Total Page Size: < 100 KB
- Lighthouse Score: 95-100

---

## 🎉 ¡Deployment Completo!

Tu presentación está lista para:
- ✅ Compartir con clientes potenciales
- ✅ Enviar por email
- ✅ Presentar en reuniones virtuales
- ✅ Validación con expertos mineros
- ✅ Meetings de fundraising

**URL para compartir**: `https://tu-proyecto.vercel.app/presentacion`

---

## 📞 Soporte

Si tienes problemas:
1. Revisa los logs en Vercel Dashboard
2. Verifica la estructura de archivos
3. Abre consola del navegador (F12) para ver errores
4. Consulta la documentación de Vercel: https://vercel.com/docs

---

**Última actualización**: Enero 2025  
**Versión**: 1.0  
**Status**: ✅ Listo para producción