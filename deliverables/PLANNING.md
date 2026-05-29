# Planificación de Estilos CSS

---

## Mapeo de instrucciones técnicas, elementos HTML y reglas CSS

Mapee cada instrucción técnica con el elemento HTML afectado y la regla CSS (el selector CSS y las propiedades CSS) que debe implementarse

| Versión | Fecha       | Instrucción del CHANGELOG.md | Elemento HTML en `index.html` | Selector CSS | Propiedad CSS principal |
|---------|------------|--------------------------------|-------------------------------|-------------|------------------------|
| [1.0.0] | 2026-03-04 | Reinicia todos los elementos del documento. | Todos los elementos HTML | `*` | `box-sizing`, `margin`, `padding` |
| [1.0.0] | 2026-03-04 | Define estilos base del cuerpo del documento (tipografía, fondo, color y line-height). | `<body>` | `body` | `font-family`, `background-color`, `color`, `line-height` |
| [1.1.0] | 2026-03-11 | Estiliza el logo con espaciado y color dorado. | `.logo` | `.logo` | `letter-spacing`, `text-transform`, `color` |
| [1.2.0] | 2026-03-18 | Convierte la barra de navegación en flex container. | `.navbar` | `.navbar` | `display`, `justify-content`, `align-items`, `padding`, `background-color` |
| [1.2.0] | 2026-03-18 | Organiza lista de navegación en fila horizontal. | `.navbar ul` | `.navbar ul` | `display`, `gap`, `list-style` |
| [1.3.0] | 2026-03-25 | Estiliza enlaces del menú sin subrayado y en negrita. | `.navbar a` | `.navbar a` | `color`, `text-decoration`, `font-weight` |
| [1.4.0] | 2026-04-01 | Cambia color de enlaces al pasar el cursor. | `.navbar a:hover` | `.navbar a:hover` | `color` |
| [1.5.0] | 2026-04-08 | Estiliza botones con fondo dorado, padding y bordes redondeados. | `.btn` | `.btn` | `display`, `color`, `background-color`, `padding`, `border-radius`, `margin-top`, `font-weight`, `text-decoration`, `transition` |
| [1.5.0] | 2026-04-08 | Cambia fondo del botón al pasar el cursor. | `.btn:hover` | `.btn:hover` | `background-color` |
| [1.6.0] | 2026-04-15 | Define espaciado general de secciones. | `.section` | `.section` | `padding` |

---

# Estructura y Organización del Archivo CSS

## Organización sugerida

```css
/* Reset y estilos globales */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Georgia, 'Times New Roman', serif;
    background-color: #080808;
    color: #f2f2f2;
    line-height: 1.6;
}

/* Navegación */
.navbar { }
.navbar ul { }
.navbar a { }
.navbar a:hover { }

/* Contenido de portada */
.hero { }
.hero-content { }

/* Multimedia */
.video-container { }

/* Botones */
.btn { }
.btn:hover { }

/* Tarjetas */
.card { }

/* Pie del sitio */
footer { }