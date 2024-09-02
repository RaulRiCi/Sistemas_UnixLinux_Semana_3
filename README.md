# Laboratorio 3 - En desarrollo

# Asegurar Bootloader

## Introduccion

### Bootloader

El bootloader, o cargador de arranque, es un programa esencial en el proceso de inicio de una computadora. Su función principal es cargar el sistema operativo en la memoria del sistema y transferirle el control para que pueda comenzar a ejecutarse.

### Carga el kernel y el initrd en memoria:

El bootloader es el primer software que se ejecuta al iniciar una computadora. Su función principal es cargar el núcleo del sistema operativo (el kernel) y el disco inicial (initrd) en la memoria. El kernel es el componente central del sistema operativo que gestiona el hardware y proporciona servicios a las aplicaciones, mientras que el initrd es un sistema de archivos en memoria utilizado para preparar el entorno antes de que el sistema operativo principal se inicie.

### Establece parámetros de inicio en el kernel:

Antes de cargar el kernel, el bootloader puede establecer parámetros de inicio que configuran cómo se debe iniciar el sistema. Estos parámetros pueden influir en el comportamiento del kernel y del sistema operativo durante el arranque.

### Una vez cargado en memoria ejecuta el kernel y transfiere el control del equipo:

Después de cargar el kernel y el initrd en la memoria, el bootloader transfiere el control al kernel. En este punto, el kernel toma el control del proceso de arranque y comienza a inicializar el sistema operativo.

### Es posible cambiar los parámetros de inicio para manipular el sistema:

Los parámetros de inicio pueden modificarse para influir en cómo el kernel y el sistema operativo se comportan durante el arranque. Esto puede ser útil para solucionar problemas, hacer pruebas o cambiar configuraciones específicas.

## Shell de root desde el bootloader

Modificando los parámetros de inicio del kernel es posible obtener un shell de root: Al modificar los parámetros de inicio del kernel desde el bootloader, puedes obtener acceso a una línea de comandos (shell) como usuario root. Esto es útil para realizar tareas administrativas, solucionar problemas o cambiar configuraciones sin necesidad de iniciar el sistema operativo normalmente.

### Pasos a seguir

Al presionar la tecla "e" en el inicio de Debian, accedes al menú de edición de las entradas del GRUB (GRand Unified Bootloader). Este menú te permite modificar temporalmente los parámetros de arranque de Debian, como las opciones del kernel o las rutas de los dispositivos. Los cambios que realices en este menú no se guardan de forma permanente, solo se aplican para esa sesión de arranque.
