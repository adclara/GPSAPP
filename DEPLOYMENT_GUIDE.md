# 🚀 Guía de Despliegue en GitHub Pages

## Pasos Rápidos (5 minutos)

### 1️⃣ Crear Repositorio en GitHub

1. Ve a [github.com](https://github.com) e inicia sesión
2. Haz clic en el botón **"+"** (arriba derecha) → **"New repository"**
3. Configura:
   - **Repository name**: `digital-theodolite` (o el nombre que prefieras)
   - **Description**: "Professional Digital Theodolite for Samsung Galaxy S23 Ultra"
   - **Public** (debe ser público para GitHub Pages gratis)
   - ✅ Marca "Add a README file"
4. Haz clic en **"Create repository"**

### 2️⃣ Subir los Archivos

**Opción A: Interfaz Web (más fácil)**

1. En tu nuevo repositorio, haz clic en **"Add file"** → **"Upload files"**
2. Arrastra estos 4 archivos:
   - `index.html`
   - `README.md` (reemplazar el existente)
   - `LICENSE`
   - `.gitignore`
3. En el cuadro de commit (abajo):
   - Mensaje: "Add Digital Theodolite Pro app"
4. Haz clic en **"Commit changes"**

**Opción B: Git Command Line**

```bash
# 1. Clona tu repositorio
git clone https://github.com/TU_USUARIO/digital-theodolite.git
cd digital-theodolite

# 2. Copia los archivos descargados al directorio

# 3. Agrega y sube
git add .
git commit -m "Add Digital Theodolite Pro app"
git push origin main
```

### 3️⃣ Activar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **"Settings"** (⚙️ arriba)
3. En el menú lateral izquierdo, busca **"Pages"**
4. En la sección **"Build and deployment"**:
   - **Source**: Deploy from a branch
   - **Branch**: `main` → `/ (root)` → **Save**
5. Espera 2-3 minutos

### 4️⃣ ¡Listo! 🎉

Tu app estará disponible en:
```
https://TU_USUARIO.github.io/digital-theodolite/
```

---

## 📱 Usar la App en tu S23 Ultra

### Primera Vez

1. Abre Chrome en tu teléfono
2. Ve a tu URL de GitHub Pages
3. Acepta todos los permisos cuando se soliciten:
   - ✅ Cámara
   - ✅ Ubicación
   - ✅ Sensores de movimiento
4. Calibración automática se iniciará

### Agregar a Pantalla de Inicio (PWA)

1. En Chrome, abre el menú (⋮)
2. **"Agregar a pantalla de inicio"** o **"Instalar app"**
3. Ahora puedes abrirla como una app nativa

---

## 🔧 Configuración Avanzada

### Dominio Personalizado (Opcional)

Si tienes un dominio propio:

1. **Crear archivo CNAME**
   - En tu repositorio, crea un archivo llamado `CNAME` (sin extensión)
   - Contenido: `theodolite.tudominio.com`

2. **Configurar DNS**
   - En tu proveedor de dominio, agrega:
   - Tipo: `CNAME`
   - Nombre: `theodolite` (o lo que prefieras)
   - Valor: `TU_USUARIO.github.io`

3. **Esperar propagación DNS** (puede tomar hasta 24h)

### HTTPS (Automático)

GitHub Pages fuerza HTTPS automáticamente - requerido para sensores.

---

## 🛠️ Personalización

### Cambiar Título y Colores

Edita `index.html` en GitHub:
1. Haz clic en el archivo `index.html`
2. Haz clic en el ícono de lápiz (✏️) para editar
3. Busca y modifica:
   - Línea ~10: `<title>` - Cambia el título
   - Línea ~400+: CSS colors - Cambia colores
4. **"Commit changes"** para guardar

### Agregar tu Logo

1. Sube tu imagen a GitHub
2. En `index.html`, busca la sección header
3. Agrega: `<img src="tu-logo.png" alt="Logo">`

---

## 📊 Estadísticas y Monitoreo

### Ver Visitantes

1. Ve a Settings → Pages
2. **"Insights"** muestra estadísticas básicas

### Google Analytics (Opcional)

Agrega antes de `</head>` en index.html:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=TU-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'TU-ID');
</script>
```

---

## 🐛 Solución de Problemas

### La página muestra 404

- **Causa**: GitHub Pages no activado o aún procesando
- **Solución**: 
  1. Verifica en Settings → Pages que esté activado
  2. Espera 5 minutos más
  3. Borra caché del navegador (Ctrl+Shift+R)

### Los permisos no funcionan

- **Causa**: No estás en HTTPS
- **Solución**: 
  - GitHub Pages siempre usa HTTPS, pero asegúrate de abrir `https://` (no `http://`)
  - Si usas dominio propio, espera a que HTTPS se active

### Errores de Git

```bash
# Si tienes conflictos:
git pull origin main --rebase
git push origin main

# Si te pide credenciales:
# Usa Personal Access Token en lugar de password
# Genera uno en: Settings → Developer settings → Personal access tokens
```

---

## 🔄 Actualizaciones Futuras

### Método Web
1. Ve a tu repositorio en GitHub
2. Haz clic en `index.html`
3. Clic en ✏️ para editar
4. Haz cambios
5. **"Commit changes"**
6. Espera 1-2 minutos, refresh la página

### Método Git
```bash
git pull origin main
# Edita archivos
git add .
git commit -m "Update: descripción de cambios"
git push origin main
```

---

## 📋 Checklist de Despliegue

- [ ] Repositorio creado en GitHub
- [ ] Archivos subidos correctamente
- [ ] GitHub Pages activado
- [ ] URL funciona (https://usuario.github.io/repo)
- [ ] Permisos de cámara se solicitan
- [ ] Permisos de ubicación se solicitan
- [ ] Sensores funcionan (mover el teléfono cambia valores)
- [ ] Calibración completada
- [ ] Crosshair visible
- [ ] Burbujas de nivel responden
- [ ] GPS obtiene coordenadas
- [ ] Captura de mediciones funciona
- [ ] Exportar CSV funciona

---

## 💡 Tips Pro

1. **Bookmark la URL** en tu S23 Ultra para acceso rápido
2. **Modo pantalla completa**: Toca F11 en escritorio o "Agregar a inicio" en móvil
3. **Batería**: Conecta cargador para sesiones largas
4. **Trípode**: Usa adaptador de trípode para teléfono para mejores resultados
5. **Backup**: GitHub mantiene todo el historial, puedes revertir cambios

---

## 🆘 Soporte

Si algo no funciona:
1. Revisa la consola del navegador (F12 → Console)
2. Verifica los permisos en configuración del navegador
3. Prueba en modo incógnito
4. Reinicia el navegador

---

## ✅ Verificación Final

Abre tu URL y verifica:
```
✓ Se ve la cámara trasera
✓ Crosshair verde en el centro
✓ Burbujas de nivel arriba
✓ Ángulos abajo actualizándose
✓ Brújula a la derecha girando
✓ GPS mostrando coordenadas
✓ Botón verde 📍 abajo
```

Si todo funciona → **¡Éxito!** 🎉

Tu Samsung Galaxy S23 Ultra es ahora un teodolito digital profesional.

---

**Última actualización**: Febrero 2024
**Versión**: 1.0.0
