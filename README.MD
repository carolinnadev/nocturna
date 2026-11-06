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