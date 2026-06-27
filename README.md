# Portafolio EST334 — Ronald Alex Diaz Pari

Portafolio estático para el curso de Estadística Espacial (EST334), UNAP 2026-I.

---

## 📁 Estructura de carpetas

```
portafolio-EST334/
├── index.html                  ← Página principal (solo editar la sección TAREAS)
├── README.md                   ← Este archivo
├── assets/
│   └── foto/
│       └── foto.jpg            ← Tu foto de perfil (reemplaza este archivo)
└── tareas/
    ├── unidad1/                ← Archivos de la Unidad I
    │   ├── tarea01.pdf
    │   ├── tarea02.pdf
    │   └── ...
    └── unidad2/                ← Archivos de la Unidad II
        ├── tarea01.pdf
        └── ...
```

---

## ✅ Cómo agregar una tarea nueva

### Paso 1 — Sube el archivo al repositorio
- Copia tu archivo PDF/imagen/video a la carpeta `tareas/unidad1/` o `tareas/unidad2/`
- Nómbralo sin espacios ni tildes, por ejemplo: `tarea01.pdf`, `mapa_idw.png`

### Paso 2 — Edita el `index.html`
Abre `index.html` y busca la sección que dice `★ AGREGA TUS TAREAS AQUÍ ★`.

Copia este bloque y pégalo dentro del array `TAREAS = [ ... ]`:

```javascript
{
  id:    "T01",              // Número único de tarea (T01, T02, T03...)
  unit:  "1",               // "1" para Unidad I, "2" para Unidad II
  title: "Nombre de la tarea",
  desc:  "Descripción breve de lo que hiciste.",
  tags:  ["R", "SIG", "mapas"],   // etiquetas que quieras
  date:  "jun 2026",
  type:  "pdf",             // "pdf" | "imagen" | "video"
  file:  "tareas/unidad1/tarea01.pdf"   // ruta al archivo que subiste
},
```

### Paso 3 — Sube los cambios a GitHub
```bash
git add .
git commit -m "Agregar tarea T01"
git push
```

¡Listo! El sitio se actualiza automáticamente.

---

## 📌 Notas importantes

- **Los archivos NUNCA se borran** porque están en el repositorio, no en el navegador.
- Puedes ver el portafolio desde cualquier dispositivo y los archivos siempre estarán.
- Si el archivo pesa más de 25 MB, usa [Git LFS](https://git-lfs.github.com/) o súbelo a Google Drive y pon el enlace en el campo `file` (como URL directa).
- Para la foto de perfil: reemplaza `assets/foto/foto.jpg` con tu foto real.

---

## 🌐 Activar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Settings → Pages
3. Source: `Deploy from a branch` → rama `main` → carpeta `/ (root)`
4. Guarda y espera 1-2 minutos
5. Tu portafolio estará en: `https://TU-USUARIO.github.io/NOMBRE-REPO/`
