---
name: premium-3d-web-design
description: "Creación de páginas web, componentes y animaciones 3D de alta gama (estilo Awwwards/premium). Úsalo para: portfolios interactivos, landing pages cinematográficas, efectos de glassmorphism avanzado, integraciones de video/3D y animaciones con GSAP o Framer Motion."
---

# Premium 3D Web Design Skill (Smart Adaptive Mode)

Esta skill permite a la IA actuar como un selector y adaptador inteligente de diseños de alta gama. No aplica un estilo fijo, sino que busca en su biblioteca el patrón que mejor se adapta a la necesidad del usuario.

## 🧠 Lógica de Ejecución (Paso a Paso)

Cuando el usuario pida un diseño, debes seguir este proceso mental:

1.  **Análisis de Contexto:** Identifica el sector (ej: lujo, tech, minimalista, industrial) y el objetivo (ej: landing, portfolio, app).
2.  **Búsqueda por Similitud:** Escanea la biblioteca en `references/full_prompts_library.txt` para encontrar el prompt cuyo estilo visual y estructura mejor encajen con el pedido.
3.  **Extracción de Estructura:** Identifica los componentes clave del prompt elegido (ej: el rig de scroll, el sistema de variables CSS, las librerías de animación).
4.  **Adaptación y Clonación:** Crea un nuevo prompt interno que mantenga la "magia" técnica del original pero sustituya:
    *   Textos y copys por los del nuevo negocio.
    *   Activos (imágenes/videos) por los proporcionados o sugeridos.
    *   Colores y tipografías para alinearlos con la marca.
5.  **Auto-Generación:** Ejecuta el código resultante siguiendo la precisión técnica del prompt de referencia.

## 🎨 Estilos Disponibles en la Biblioteca

*   **Cinematic Scroll (Parallax Profundo):** Ideal para storytelling y destinos (Referencia: Mostar City).
*   **Liquid Glass (Glassmorphism Avanzado):** Ideal para apps modernas y bienestar (Referencia: Equilibrium).
*   **Clean Tech / Dark Premium:** Ideal para seguridad, SaaS y servicios de lujo (Referencia: VaultShield / FluxEngine).
*   **Interactive Typewriter:** Ideal para portfolios y agencias creativas.

## 🛠️ Reglas Técnicas Innegociables

*   **Variables CSS:** Siempre usa un bloque `:root` para manejar estados de animación.
*   **Tipografía:** Nunca uses fuentes genéricas; busca la declaración `@font-face` o `<link>` en el prompt de referencia.
*   **Interacción:** Si el prompt original usa GSAP o Framer Motion, mantén esa misma librería para asegurar la fluidez.

> **IMPORTANTE:** Consulta siempre `references/full_prompts_library.txt` antes de empezar cualquier desarrollo para asegurar la fidelidad al estilo premium.
