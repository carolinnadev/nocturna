# 🚲 Rueda Nocturna — Proyecto Tailwind CSS

Plataforma de recorridos nocturnos guiados en bicicleta por la ciudad de Medellín.

## Framework Elegido: Tailwind CSS

**Por qué:**  
El proyecto Rueda Nocturna requiere una identidad visual propia con tonos oscuros, contrastes de alta visibilidad para la noche y una experiencia personalizada. Tailwind CSS nos permite construir exactamente la interfaz que buscamos combinando utilidades de bajo nivel sin depender del diseño estándar de otros frameworks.

**Qué gano:**  
- Un diseño visual único con colores y sombras propias de la marca.
- Generación de un archivo CSS final sumamente ligero y optimizado mediante Tailwind CLI.
- Adaptabilidad total con clases responsive mobile-first (`sm:`, `md:`, `lg:`).
- Modo oscuro nativo integrado mediante la variante `dark:`.

**Qué acepto:**  
- Un HTML más denso debido al uso explícito de múltiples clases de utilidad.
- Programar manualmente cualquier interacción JavaScript (como modales o menús colapsables).

**Cómo lo mitigo:**  
- Mantengo un kit de componentes unificado en `componentes.html`.
- Utilizo la directiva `@theme` en CSS para centralizar las variables del diseño y mantener la consistencia cromática.

# Rueda Nocturna — Landing Page y Ecosistema

Sitio modular responsive enfocado en recorridos nocturnos guiados en bicicleta por la ciudad de Medellín.

**Sitio publicado en GitHub Pages:** [https://tu-usuario.github.io/tu-repositorio/](https://tu-usuario.github.io/tu-repositorio/)

## Páginas y Secciones
- `index.html` (Landing Rueda Nocturna): Hero, rutas interactivas, sección de pasos, planes comerciales y formulario de inscripción validado.
- Sitio principal (v2.0 en Bootstrap): Integrado con navegación cruzada y coherencia visual de marca.

## Tecnologías Utilizadas
- HTML5 semántico
- Tailwind CSS v4 (con Tailwind CLI y compilación minificada `--minify`)
- Git y GitHub / GitHub Pages

## Framework Elegido y Justificación
Se seleccionó **Tailwind CSS** por la necesidad de construir una identidad visual única con colores oscuros y alta visibilidad nocturna (`#FFD166`), logrando un rendimiento superior y un archivo CSS final muy ligero (~11 KB) en comparación con frameworks pesados basados en componentes genéricos.

## Autor
Caro — Coder de Riwi (2026)