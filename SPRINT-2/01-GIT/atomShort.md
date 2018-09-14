# ATOM
Atom es un editor de código de fuente de código abierto para macOS, Linux, y Windows​ con soporte para plug-ins escritos en Node.js y control de versiones Git integrado, desarrollado por GitHub. Atom es una aplicación de escritorio construida utilizando tecnologías web.​

![ATOM](https://icon2.kisspng.com/20180810/ojp/kisspng-computer-icons-react-javascript-desktop-wallpaper-atom-icon-macaron-iconset-goescat-5b6d61715acf14.798922431533895025372.jpg)

## Core Settings
Estos son ajustes de núcleo de **atom** que afectan el comportamiento no relacionado con la edición de texto. Los paquetes individuales pueden tener su propia configuración adicional encontrada dentro de su tarjeta de paquete en la lista de paquetes.

- **Allow pending pane items**: Permite previsualizar los elementos sin agregarlos a un panel haciendo clic en los archivos en la vista de árbol.
- **Audio Beep**: Activa el beep del sistema cuando ciertas acciones no se pueden ejecutar o no hay resultados.
- **Automatically update**: Actualiza automáticamente el atom cuando hay una nueva versión disponible.
- **Close deleted file tabs**: Cierre los editores correspondientes cuando se elimine un archivo de un atom.
- **Close the empty windows**: Cuando una ventana sin abrir las pestañas o paneles da el comando `Cerrar pestaña (Close tab)`, cierra esa ventana.

###### Color profile
Especifica si atom debe usar el perfil de color del sistema operativo (recomendado) o un perfil de color alternativo. Cambiar esta configuración requerirá un relanzamiento del atom para tener un efecto.  
`Use color configured in the operating system`
- **Remove empty panes**: Cuando se cierra la última pestaña de un panel, elimina ese panel también.
- **Exclude VCS ignored paths**: Los archivos y directorios ignorados por los proyectos actuales `vcs` serán ignorados por algunos paquetes, como el buscador difuso y buscar y reemplazar. Por ejemplo, los proyectos que usan git tienen estas rutas definidas en el archivo `.gitignore`. Los paquetes individuales pueden tener una configuración  adicional para ignorar `vcs` archivos y carpetas ignorados.

###### File enconding
Codificación de conjunto de carácteres predeterminada para usar al leer y escribir archivos.  
`Unicode (UTF-8)`
##### File system watcher
Elija la implementación subyacente utilizada para vigilar los cambios en el sistema de archivos. Al emular cambios, se perderán todos los eventos causados ​​por aplicaciones distintas de atom, pero pueden ayudar a prevenir bloqueos o congelamientos.
- **Follow symlinks**: Sigue los enlaces simbólicos al buscar archivos y al abrir archivos con el buscador difuso.

##### Ignored names
Lista de patrones `glob`. Los archivos y directorios que coincidan con estos patrones serán ignorados por algunos paquetes, como el buscador difuso y la vista de árbol. Los paquetes individuales pueden tener configuraciones adicionales para ignorar los nombres.  
`Default: .git, .hg, .svn, .DS_Store, ._*, Thumbs.db, desktop.ini`  
- **Open empty editor in start**: Cuando está marcado abre un editor sin título cuando se carga un entorno en blanco (como con el *archivo*> *nueva ventana* o cuando "restauración de ventanas anteriores al inicio" está desmarcada); de lo contrario, no se abrirá ningún editor cuando cargue un entorno en blanco. Esta configuración no tiene efecto al restaurar un estado anterior.

###### Project home
El directorio donde se supone que se ubicarán los proyectos. Los paquetes creados usando el generador de paquetes se almacenarán aquí de forma predeterminada.
Ejemplo:
`/Users/HDH-V/github`
###### Reopen projects menu count
Cuántos proyectos recientes se muestran en el proyecto de reabrir.  
`Default : 15`

###### Restore previous windows on start
Cuando se selecciona 'no', se carga un entorno en blanco. Cuando se selecciona *'sí'* y el atom se inicia desde el ícono o `atom` por sí mismo desde la línea de comando, restaura el último estado de todas las ventanas de atom; de lo contrario, se carga un entorno en blanco. Cuando se selecciona *'always'*, restaura el último estado de todas las ventanas de atom siempre, sin importar cómo se inicie el atom.  
Ejemplo: `yes`

###### Send telemetry to the atom team
Permita que las estadísticas de uso y los informes de excepción se envíen al equipo atom para ayudar a mejorar el producto.    
Ejemplo: `Allow limited anonymous usage stats, exception and crash reporting`

###### Title bar
Experimental: una barra de título de aduana se adapta a los colores del tema. Elegir la inserción personalizada agrega un poco más de relleno. La barra de título también puede estar completamente oculta.  
Nota: cambiar a una barra de título personalizada u oculta comprometerá alguna funcionalidad. Esta configuración requerirá un relanzamiento del atom para que tenga efecto.  
Ejemplo: `native`.
- **Use Proxy Settings When Calling APM**: Utilizar la configuración de proxy detectada al llamar a la herramienta de línea de comandos `apm`.

- **Use Tree Sitter Parsers**: Experimental: utilice el nuevo sistema de análisis de tres personas para los idiomas admitidos.

###### Version Pinned Packages
Lista de nombres de paquetes instalados que no se actualizan automáticamente.

###### Warn On large File limit
Advertir antes de abrir archivos mayores a esta cantidad de megabytes


![Core settings](https://cdn-images-1.medium.com/max/456/1*0Y2BR9V0MCvrkFNRDc1U-Q.png)

Ahora ya estás preparado para presonalizar el entorno de tu `atom`, recuerda no caer en un agujero negro!!

`Paula Sshun 2018 ®`
