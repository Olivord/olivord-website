# 🚀 GUÍA COMPLETA - PROYECTO APSARA WEB

## ¿Qué has recibido?

Te he proporcionado:

1. **index.html** → HTML/CSS/JS funcional (descarga y abre en el navegador ahora)
2. **Estructura de proyecto Astro** → Para escalar cuando tengas muchos capítulos
3. **Ejemplos de archivos `.md`** → Para los capítulos y galería

---

## 🎯 OPCIÓN 1: EMPEZAR RÁPIDO (Recomendado para ahora)

### Paso 1: Descarga el archivo HTML

1. Ve a `index.html` en el repositorio
2. Descárgalo o cópialo completo
3. Crea una carpeta en tu ordenador: `Mi-web-apsara/`
4. Guarda el archivo como `index.html` dentro

### Paso 2: Abre en el navegador

- Haz doble click en `index.html`
- ¡Listo! Ya ves tu web funcionando

### Paso 3: Personaliza (sin tocar código)

**Para cambiar el texto principal:**
- Abre `index.html` con un editor de texto (Notepad, VS Code, etc.)
- Busca: `<h1>APSARA</h1>`
- Cambias el texto que quieras
- Guardas (Ctrl+S)
- Actualizas el navegador (F5)

**Para cambiar las imágenes:**
- En la sección "CAPÍTULOS", busca: `<img src="https://..."`
- Cambia la URL por la de tu imagen

---

## 🎨 OPCIÓN 2: ESCALAR CON ASTRO (Cuando tengas 5+ capítulos)

### ¿Cuándo cambiar a Astro?

- Ahora: Usa HTML simple (estás en Cap 0)
- Cuando: Tengas Cap 0, 1, 2... (3-5 capítulos)
- Por qué: Astro genera automáticamente todas las páginas de capítulos

### Cómo hacer la migración

Cuando llegues a ese punto:

1. Instalamos Astro
2. Organizamos los archivos en la estructura
3. Tú solo añades `.md` con contenido
4. La web se genera automáticamente

---

## 📝 CÓMO AÑADIR TU PRIMER CAPÍTULO (EN HTML)

### Opción: Copiar + Modificar la tarjeta existente

En `index.html`, busca esta sección:

```html
<article class="chapter-card">
  <img src="..." class="chapter-image" />
  <div class="chapter-content">
    <div class="chapter-number">CAPÍTULO 0</div>
    <h3 class="chapter-title">La Chica de las Ruinas</h3>
    <p class="chapter-description">...</p>
    <a href="#cap-0" class="read-button">LEER AHORA</a>
  </div>
</article>
```

**Para añadir un Cap 1, copías esto debajo y cambias:**

```html
<article class="chapter-card">
  <img src="TU-IMAGEN-CAP-1.jpg" class="chapter-image" />
  <div class="chapter-content">
    <div class="chapter-number">CAPÍTULO 1</div>
    <h3 class="chapter-title">Tu Título Aquí</h3>
    <p class="chapter-description">Tu descripción aquí...</p>
    <a href="#cap-1" class="read-button">LEER AHORA</a>
  </div>
</article>
```

---

## 🖌️ CÓMO ORGANIZAR TUS IMÁGENES

### Opción 1: Imágenes en línea (ahora mismo)

Subes tus imágenes a un servicio gratis:
- **Imgur.com** (anónimo, gratis)
- **imgbb.com** (anónimo, gratis)
- **Cloudinary** (250MB gratis/mes)

Copias la URL y la pegas en el HTML:

```html
<img src="https://i.imgur.com/ABC123.jpg" />
```

### Opción 2: Imágenes locales (cuando publiques la web)

Creas una carpeta `uploads/` junto a `index.html`:

```
Mi-web-apsara/
├── index.html
└── uploads/
    ├── cap-0-1.jpg
    ├── cap-0-2.jpg
    └── ...
```

Y luego:

```html
<img src="uploads/cap-0-1.jpg" />
```

---

## 📱 PUBLICAR LA WEB (Gratis en 5 min)

### Opción A: GitHub Pages (Recomendado)

1. Tu repositorio ya está configurado en GitHub
2. Ve a Settings → Pages → elige "main branch"
3. ¡Listo! Tu web estará en: `https://olivord.github.io/olivord-website`

### Opción B: Netlify (Aún más fácil)

1. Ve a **netlify.com**
2. Conecta tu repositorio de GitHub
3. ¡Listo! Te da un link automáticamente
4. Bonus: Puedes conectar tu dominio personalizado

### Opción C: Vercel (También gratis)

Mismo proceso que Netlify, pero con **vercel.com**

---

## 🎨 PERSONALIZAR COLORES (Sin tocar código)

Si quieres cambiar los colores:

En `index.html`, al principio, hay una sección `:root {`:

```css
:root {
  --color-primary: #0a0e27;        /* Negro-azul oscuro */
  --color-secondary: #1a1f3a;      /* Negro-morado */
  --color-accent: #7c3aed;         /* Morado brillante */
  --color-accent-light: #a78bfa;   /* Morado claro */
  --color-text: #e5e7eb;           /* Blanco cremoso */
}
```

Cambias los códigos hexadecimales:
- **#0a0e27** → Fondo oscuro principal
- **#7c3aed** → Color de acentos (botones, líneas)
- **#e5e7eb** → Color del texto

Ejemplo: Si quieres más cyan en lugar de morado:
- `--color-accent: #06b6d4;` (cyan)
- `--color-accent-light: #22d3ee;` (cyan claro)

---

## 🚦 PRÓXIMOS PASOS (Mi recomendación)

### Semana 1-2:
1. Activa GitHub Pages para ver tu web online ✅
2. Personaliza los textos y colores
3. Prepara las imágenes del Cap 0
4. Publica

### Semana 3+:
5. Crea el Cap 0 completo (4-6 imágenes + narrativa)
6. Publica
7. Recibe feedback en redes
8. Crea Cap 1

### Cuando tengas 3-4 capítulos:
9. Migramos a Astro
10. Sistema automático de páginas
11. Añades la galería
12. Conectas tienda

---

## ❓ PREGUNTAS FRECUENTES

**P: ¿Puedo editar el HTML sin saber programación?**
R: Sí. Solo cambias texto dentro de los tags. No toques los `<` y `>`.

**P: ¿Dónde pongo mis imágenes?**
R: En una carpeta `uploads/` junto al `index.html` (cuando publiques). Mientras, usa URLs en línea.

**P: ¿Cómo hago más rápido cuando tenga muchos capítulos?**
R: Entonces migramos a Astro. Ese día solo creas archivos `.md` y la web se genera sola.

**P: ¿La web es responsive (funciona en móvil)?**
R: Sí, totalmente. Ya está implementado en el CSS.

---

**¿Listo para empezar? 🚀**

Descarga el `index.html`, abre en navegador, y ¡a crear!

¡VAMOS!