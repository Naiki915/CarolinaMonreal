# 🤠 Rodeo Night — Página de Cumpleaños de Carolina

Página de cumpleaños personalizada con tema country/vaquero, galería de fotos y muro de fotos para invitados.

---

## 📁 Estructura del proyecto

```
carolina18/
├── index.html                  ← Página principal
├── README.md                   ← Estas instrucciones
└── assets/
    └── fotos-carolina/         ← Aquí van las fotos de Carolina desde niña
        ├── bebe.jpg
        ├── 3anios.jpg
        ├── escuela.jpg
        ├── 10anios.jpg
        ├── 13anios.jpg
        └── carolina18.jpg      ← Foto actual (ya la tienes)
```

---

## 🚀 PASO 1 — Subir a GitHub Pages

1. Ve a [github.com](https://github.com) y crea una cuenta si no tienes
2. Crea un repositorio nuevo → **"carolina18"** (público)
3. Sube todos los archivos de esta carpeta
4. Ve a **Settings → Pages → Source → main branch**
5. Tu página quedará en: `https://TU_USUARIO.github.io/carolina18`

---

## ☁️ PASO 2 — Configurar Cloudinary (fotos de invitados)

### 2a. Crear cuenta gratuita
1. Ve a [cloudinary.com](https://cloudinary.com) y regístrate gratis
2. Anota tu **Cloud Name** (aparece en el dashboard, ej: `dxyz123abc`)

### 2b. Crear Upload Preset
1. En Cloudinary → **Settings → Upload → Upload Presets**
2. Clic en **"Add upload preset"**
3. Nombre: `carolina_fotos`
4. **Signing Mode: Unsigned** ← MUY IMPORTANTE
5. En "Folder" escribe: `carolina_fiesta`
6. Guarda

### 2c. Actualizar el código
Abre `index.html` y busca estas dos líneas (cerca del final):

```javascript
const CLOUD_NAME = 'TU_CLOUD_NAME';    // ← Cambia por tu Cloud Name
const UPLOAD_PRESET = 'carolina_fotos'; // ← Déjalo igual
```

Ejemplo:
```javascript
const CLOUD_NAME = 'dxyz123abc';
const UPLOAD_PRESET = 'carolina_fotos';
```

---

## 🖼️ PASO 3 — Agregar fotos de Carolina

Reemplaza los placeholders en la línea del tiempo con fotos reales:

1. Agrega las fotos a la carpeta `assets/fotos-carolina/`
2. Nómbralas igual: `bebe.jpg`, `3anios.jpg`, etc.
3. En `index.html` busca cada `timeline-photo-placeholder` y reemplaza con:
```html
<img src="assets/fotos-carolina/NOMBRE.jpg" alt="Carolina">
```

---

## 🌐 Compartir la página

Una vez todo configurado, comparte el link:
```
https://TU_USUARIO.github.io/carolina18
```

¡Ponlo en la invitación y en el grupo de WhatsApp! 🤠

---

## ✨ Funcionalidades incluidas

- ✅ Invitación animada con papel picado y serape
- ✅ Cuenta regresiva en tiempo real
- ✅ Línea del tiempo de 18 años de vida
- ✅ Muro de fotos de invitados (Cloudinary)
- ✅ Mensaje especial para Carolina
- ✅ Diseño 100% responsive (celular y desktop)
- ✅ Lightbox para ver fotos en grande

---

Hecho con 🤠 y mucho amor para Carolina
