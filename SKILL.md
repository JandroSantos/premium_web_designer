---
name: premium-3d-web-design
description: "Creación de páginas web, componentes y animaciones 3D de alta gama (estilo Awwwards/premium). Úsalo para: portfolios interactivos, landing pages cinematográficas, efectos de glassmorphism avanzado, integraciones de video/3D y animaciones con GSAP o Framer Motion."
---

# Premium 3D Web Design Skill

Esta skill proporciona las directrices y patrones necesarios para replicar el estilo visual "premium" visto en los ejemplos del usuario, caracterizado por el uso intensivo de video, profundidad 3D, tipografía audaz y animaciones fluidas.

## Principios de Diseño

Para lograr el acabado "premium" esperado, debes seguir estas reglas:

1.  **Tipografía como Protagonista:** Utiliza fuentes display de alta calidad (como Ogg, Satoshi, Geist o Helvetica Now). No te limites a las fuentes del sistema; usa `@import` o `<link>` para cargar fuentes específicas que definan el carácter de la página.
2.  **Profundidad y Capas:** Implementa efectos de parallax multicanal. Divide las imágenes en capas (fondo, medio, primer plano) y muévelas a diferentes velocidades durante el scroll.
3.  **Estética "Liquid Glass":** Para componentes de UI, usa `backdrop-filter: blur()` combinado con bordes semitransparentes y sombras internas suaves para simular cristal líquido.
4.  **Movimiento Intencional:** Las animaciones no deben ser solo decorativas. Usa transiciones suaves (ease-out/in-out) para guiar la atención del usuario.

## Tecnologías Preferidas

Dependiendo de la complejidad del proyecto, selecciona el stack adecuado:

| Stack | Uso Recomendado | Librerías Clave |
| :--- | :--- | :--- |
| **Vanilla Premium** | Páginas de scroll cinematográfico puro. | GSAP, ScrollTrigger, CSS Variables. |
| **React Interactive** | Aplicaciones modernas y componentes dinámicos. | Framer Motion, Lucide Icons, Tailwind CSS. |
| **3D Inmersivo** | Experiencias con modelos 3D y partículas. | Three.js, React Three Fiber, Spline. |

## Flujo de Trabajo

Cuando el usuario pida una página o componente basado en esta skill:

1.  **Análisis de Activos:** Identifica si el usuario proporciona videos, modelos 3D o imágenes. Si no, busca activos de alta calidad que encajen con el estilo "oscuro/futurista" o "limpio/minimalista".
2.  **Configuración de Variables CSS:** Define un bloque `:root` con variables para colores, desenfoques y estados de animación. Esto permite un control preciso y animaciones fluidas mediante la manipulación de variables desde JavaScript.
3.  **Implementación de Animaciones:**
    *   Usa **Framer Motion** para animaciones de entrada (fade-up, stagger children).
    *   Usa **GSAP** para secuencias complejas basadas en el scroll (scrubbing).
    *   Usa **Tailwind** para el layout base y estados hover rápidos.

## Ejemplo de Patrón: Liquid Glass

Para crear un contenedor de cristal líquido, aplica este estilo CSS:

```css
.liquid-glass {
  background: rgba(255, 255, 255, 0.01);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 1px rgba(255, 255, 255, 0.1);
  border-radius: 24px;
}
```

> **Nota:** Para referencias detalladas sobre los prompts originales y sus estructuras exactas, consulta `/home/ubuntu/skills/premium-3d-web-design/references/original_prompts.md`.
