# Patitas & Hogar — Efectos Visuales con CSS

Proyecto de práctica para el video **"Efectos Visuales con CSS: Transiciones, Pseudoclases e Interactividad"**.  
Página web de adopción de mascotas construida con HTML5 y CSS3 puro

---

## Cómo abrir el proyecto

No requiere instalación ni servidor. Abre `index.html` directamente en el navegador.

Si usas VS Code, instala la extensión **Live Server** y haz clic en *Open with Live Server* para ver los cambios en tiempo real mientras editas.

---

## Archivos del proyecto

### `index.html`
Contiene toda la estructura de la página: navegación, hero, cards de animales, formulario de adopción y footer. No se modifica durante el video.

### `styles/styles.css`
Define la apariencia base de todos los elementos: variables de color, tipografía, layout con Grid y Flexbox, y tamaños. No contiene ningún efecto interactivo.

### `styles/efectos.css`
El archivo central del video. Contiene todos los efectos interactivos.

---

## Efectos visuales y transiciones aplicados

**`transition`**  
Hace que los cambios de estado ocurran de forma gradual. Siempre va en el estado base del elemento, nunca dentro del `:hover`.

**`@keyframes`**  
Define animaciones que corren solas, sin interacción del usuario. Se nombran libremente y se aplican con la propiedad `animation`.

**`::before` y `::after`**  
Pseudo-elementos que crean contenido decorativo sin modificar el HTML. Requieren `content: ''` para existir. Se usan en el proyecto para crear capas de color deslizantes en los botones y líneas animadas en los links.

**`:focus` y `:focus-within`**  
`:focus` actúa sobre el elemento que tiene foco. `:focus-within` actúa sobre el padre cuando cualquier hijo tiene foco — permite cambiar el estilo del label cuando el usuario hace clic en el input.

---

## Variables CSS disponibles

Definidas en `styles.css` y disponibles en todo el proyecto:

```css
--crema:     #fdf6ee
--arena:     #f0e4d0
--caramelo:  #d97c3a  
--terracota: #b85c2a
--carbon:    #2b2118   
--cafe:      #6b4226
--muted:     #9a7d65
--blanco:    #ffffff
```

---

## Tecnologías

- HTML5 semántico
- CSS3 puro — sin frameworks, sin JavaScript
- Google Fonts: Playfair Display + Nunito

---

## Créditos

Proyecto desarrollado como material de apoyo para clase de Desarrollo Web.  
Refugio ficticio — las imágenes son de mascotas reales.