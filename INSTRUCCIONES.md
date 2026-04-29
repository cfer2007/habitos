# 📱 Rastreador de Hábitos — PWA

## ¿Qué incluye?
- ✅ App instalable en Android e iOS (PWA)
- ✅ Funciona sin internet
- ✅ Recordatorio diario configurable
- ✅ Sincronización con Google Drive
- ✅ Vista mensual, anual (heatmap) y comparativa
- ✅ Rachas (streaks), gráficas, colores por objetivo

---

## 🚀 Opción 1: Abrir localmente (más rápido)
1. Descarga toda la carpeta `habitos-pwa`
2. Abre `index.html` en Chrome o Edge
3. ¡Listo! Los datos se guardan automáticamente

> ⚠️ Las notificaciones y la instalación como app requieren HTTPS (Opción 2)

---

## 🌐 Opción 2: Publicar en GitHub Pages (recomendado)

### Paso 1 — Crear cuenta en GitHub
Ve a github.com y crea una cuenta gratuita si no tienes.

### Paso 2 — Crear repositorio
1. Haz clic en "New repository"
2. Nombre: `habitos` (o el que quieras)
3. Marca "Public"
4. Clic en "Create repository"

### Paso 3 — Subir archivos
1. En el repositorio, clic en "uploading an existing file"
2. Arrastra TODOS los archivos de la carpeta `habitos-pwa`
   - index.html
   - manifest.json
   - sw.js
   - carpeta icons/ (con todas las imágenes)
3. Clic en "Commit changes"

### Paso 4 — Activar GitHub Pages
1. Ve a Settings → Pages
2. En "Source" selecciona: Branch: main, / (root)
3. Clic en "Save"
4. En ~1 minuto tendrás tu URL: `https://TU_USUARIO.github.io/habitos`

### Paso 5 — Instalar en tu teléfono
**Android (Chrome):**
1. Abre la URL en Chrome
2. Menú (⋮) → "Añadir a pantalla de inicio"
3. ¡Aparece el ícono como una app!

**iOS (Safari):**
1. Abre la URL en Safari
2. Botón compartir (□↑) → "Añadir a pantalla de inicio"
3. ¡Aparece el ícono como una app!

---

## ☁️ Configurar Google Drive (opcional pero recomendado)

Para que los datos persistan al cambiar de teléfono:

### Paso 1 — Google Cloud Console
1. Ve a console.cloud.google.com
2. Crea un proyecto nuevo
3. Ve a "APIs y servicios" → "Biblioteca"
4. Busca "Google Drive API" y actívala

### Paso 2 — Crear credenciales
1. Ve a "APIs y servicios" → "Credenciales"
2. Clic en "Crear credenciales" → "ID de cliente OAuth 2.0"
3. Tipo de aplicación: "Aplicación web"
4. Nombre: "Rastreador de Hábitos"
5. En "Orígenes autorizados de JavaScript" agrega:
   - `https://TU_USUARIO.github.io`
6. Clic en "Crear"
7. Copia el "ID de cliente"

### Paso 3 — Conectar en la app
1. Abre la app → pestaña "Ajustes"
2. Sección "Google Drive" → "Conectar Google Drive"
3. Pega tu Client ID
4. Autoriza el acceso
5. ¡Listo! Se sincroniza automáticamente

---

## 🔔 Activar recordatorios
1. Ve a Ajustes → Recordatorios
2. Activa el toggle
3. Selecciona la hora
4. Acepta el permiso de notificaciones

---

## 💾 Respaldo manual
- **Exportar:** Botón "Export" → guarda un archivo JSON
- **Importar:** Botón "Import" → carga un archivo JSON guardado
- Guarda el JSON en Google Drive o Dropbox como respaldo adicional
