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

## Readme actualizado desde la interfaz de github

Lorem ipsum dolor sit amet consectetur adipiscing elit potenti pretium per, dapibus parturient eleifend maecenas neque laoreet sagittis euismod cursus, magna integer convallis rutrum turpis ultrices dictum praesent aliquam. Morbi fusce donec condimentum litora luctus lacus volutpat eleifend dignissim et, etiam fames porttitor vulputate nostra nullam vitae fermentum. Scelerisque ad libero ultricies natoque imperdiet felis neque, lobortis lacus nascetur consequat in hac leo, tortor facilisi dui non vehicula vestibulum.


## Preguntas sobre SSH

### 1. ¿Qué es SSH?  
Es un protocolo de red destinado principalmente a la conexión con máquinas a las que accedemos por línea de comandos.

### 2. ¿Qué diferencia existe entre una clave pública y una clave privada?
La clave privada se mantiene cifrada y almacenada de forma segura en el equipo local, el único que la conoce es el usuario, y la pública se comparte de forma libre con servidores SSH a los que el usuario se conecte. El servidor usa la clave para crear un autentificador y el usuario emplea la privada para iniciar sesión.

### 3. ¿Qué clave puede compartirse?
La clave pública.

### 4. ¿Qué clave no debe compartirse nunca?
La privada.

### 5. ¿Qué ventaja presenta SSH frente a introducir continuamente usuario y contraseña?
Permite a los administradores configurar claves SSH únicas, las cuales evitan contraseñas débiles que terminen siendo puntos de vulnerabilidad, reduce los ataques a fuerza bruta y vuelve el proceso de identificación más rápido, permitiendo conexiones automáticas, automatizaciones y scripts de administración.

### 6. ¿Qué función cumple el archivo known_hosts?
Es donde se almacenan las claves públicas de los servidores. En el primer ingreso al servidor este graba la clave para futuras visitas; si se vuelve a intentar ingresar, se compararán las claves del archivo y la que devuelve el servidor. Si coinciden se accede sin problema, pero si no, el SSH bloquea el acceso y lanza una advertencia de peligro para evitar ataques donde intentan suplantar al servidor.

### 7. ¿Qué podría ocurrir si una clave privada se publica en GitHub?
Cualquier persona en internet podría suplantar la identidad del propietario y acceder al repositorio con los mismos permisos que el afectado.

---

## Preguntas sobre Fork

### 1. ¿Qué es un fork en GitHub?
Son "bifurcaciones", copias exactas de un repositorio que se copia en nuestro GitHub en vez de descargar directamente una copia en nuestro equipo, por lo que se termina teniendo dos repositorios exactamente iguales, con el mismo historial pero que los cambios que se hagan en uno no afectan al otro.

### 2. ¿En qué se diferencia un fork de una rama?
En que un fork es una copia completa del repositorio almacenada en otra cuenta que trabaja de forma totalmente independiente, mientras que una rama es una línea de desarrollo paralela creada dentro del mismo repositorio.

### 3. ¿En qué cuenta se almacena un fork?
En la cuenta del usuario que realiza la copia del repositorio original.

### 4. ¿Cuándo resulta útil trabajar mediante un fork?
Cuando se quiere probar cambios que podrían romper el proyecto original o proponer mejoras y colaboraciones en proyectos de código abierto de terceros sin necesidad de permisos de escritura directos.

### 5. ¿Qué relación existe entre el repositorio original y el fork?
Quitando que en el momento de la copia son iguales, no comparten cambios automáticamente, ya que trabajan de forma independiente el uno del otro a menos que se sincronicen.

### 6. ¿Qué es el repositorio upstream?
Es el repositorio original del que se ha hecho el fork.

### 7. ¿Qué diferencia existe entre origin y upstream?
`origin` apunta a tu propia copia remota del repositorio (tu fork), mientras que `upstream` apunta al repositorio original desde el que creaste dicho fork.

### 8. ¿Cómo se propone que un cambio del fork llegue al repositorio original?
Realizando una Pull Request desde GitHub, donde se deberá poner un título y una descripción de las mejoras que se implementan o los errores que se solucionan.

### 9. ¿Quién decide si se acepta la propuesta?
Los propietarios y/o administradores del repositorio original (`upstream`).

### 10. ¿Puede seguir evolucionando el repositorio original mientras existe el fork?
Sí, aunque el fork se quedará desactualizado según se vaya modificando el original. Para solucionar esto se debe hacer un "Sync fork".