## Historial del proyecto

El desarrollo de este proyecto se ha llevado a cabo de forma progresiva mediante commits pequeños, atómicos y con un propósito claro.

### ¿Por qué es preferible realizar varios commits pequeños frente a uno solo?

1. **Facilidad para detectar y corregir errores:** Si surge un fallo o una regresión en el código, un historial detallado permite identificar exactamente en qué cambio se introdujo el problema. Esto hace que revertir o corregir dicho error sea mucho más sencillo y preciso.
2. **Revisiones de código más claras y eficientes:** Para otros desarrolladores o revisores (por ejemplo, en las Pull Requests), examinar cambios independientes y acotados resulta mucho más fácil e intuitivo que revisar un único commit masivo con todo el contenido del sitio web.
3. **Mejor trazabilidad y documentación:** Cada commit actúa como una nota en la bitácora del proyecto. Los mensajes descriptivos permiten entender la evolución y el contexto de las decisiones que se tomaron a lo largo del desarrollo.
4. **Facilidad para la colaboración y resolución de conflictos:** Al trabajar en ramas paralelas, realizar commits pequeños reduce el riesgo de tener conflictos complejos de fusión y simplifica la integración de nuevas funcionalidades en la rama principal (`main`).

## Cómo abrir la página

Para visualizar y probar la página web en tu entorno local, sigue estos pasos:

1. **Clonar el repositorio:**
   git clone git@github.com:tu-usuario/daw-project-hub.git

2. **Navegar a la carpeta del proyecto:**
   cd daw-project-hub

3. **Abrir el sitio web en el navegador:**
   - Puedes hacer doble clic directamente sobre el archivo index.html desde el explorador de archivos de tu sistema operativo.
   - O bien, si usas Visual Studio Code, haz clic derecho sobre index.html y selecciona Open with Live Server.