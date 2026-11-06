# Día 1: Introducción a Tailwind CSS (Rueda Nocturna)

## 1. Comparación de Enfoques: Componentes vs. Utility-First
* **Cómo se construía un botón en Bootstrap (Semana 2):** Se utilizaban clases de componentes predefinidas y cerradas provistas por el framework, como `class="btn btn-primary"`. El diseño, los colores y los radios venían prediseñados y solo se aplicaban o personalizaban de manera global.
* **Cómo se construye un botón con Tailwind CSS (Día 1):** Se compone el diseño directamente en el elemento combinando clases utilitarias de bajo nivel y de un solo propósito. Por ejemplo: `class="rounded-lg bg-amber-800 px-5 py-2.5 font-semibold text-white shadow-md hover:bg-amber-900 focus:ring-4 focus:ring-amber-300 focus:outline-hidden"`.
* **Diferencia clave:** Bootstrap entrega componentes terminados con un aspecto predeterminado que suele lucir idéntico si no se modifica profundamente. Tailwind CSS es un framework *utility-first* que no trae componentes prediseñados, sino utilidades puras para que cada interfaz sea completamente única y adaptada al diseño sin salir del código HTML.

## 2. Verificación de Generación de Clases (Tailwind CLI)
* **Comportamiento observado en `src/output.css`:** Al utilizar Tailwind CLI en modo observación (`--watch`), la herramienta escanea los archivos del proyecto y genera un archivo CSS optimizado que contiene **únicamente** las clases de utilidad que se están usando activamente en el código HTML.
* **Por qué una clase que no usas no aparece:** Si en el código no se invoca una clase específica (por ejemplo, `bg-pink-500`), Tailwind la omite por completo del archivo compilado final. Esto garantiza un rendimiento óptimo y un archivo CSS final muy ligero, razón por la cual siempre se deben escribir las clases de utilidad completas y evitar construirlas mediante concatenaciones dinámicas de strings en JavaScript.

## 3. Reglas del Kit de Componentes
Para garantizar la consistencia visual de la campaña **Rueda Nocturna** en todos sus elementos (botones, cards, alertas e inputs), se establecieron y aplicaron las siguientes reglas de diseño:
* **Radios de borde:** Se utiliza una escala unificada de bordes redondeados (`rounded-lg` para componentes interactivos y contenedores pequeños, y `rounded-xl` para las cards principales).
* **Escala de espaciado:** Se mantiene una estructura simétrica de rellenos y márgenes basada en la escala modular de Tailwind (múltiplos coherentes como `p-4`, `p-6`, `px-5 py-2.5`, etc.).
* **Paleta de colores y estados:** Uso estricto de la gama cromática principal basada en tonos ámbar (`amber-800`, `amber-900`, `amber-700`, `amber-50`) combinados con grises neutros de soporte, asegurando estados interactivos consistentes mediante prefijos de eventos como `hover:` y anillos de enfoque visibles (`focus:ring-2`, `focus:ring-amber-300`, `focus:outline-hidden`) para cumplir con los estándares de accesibilidad con teclado.