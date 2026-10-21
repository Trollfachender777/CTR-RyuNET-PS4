# Guía de uso: desde las carpetas hasta el primer arranque

Esta guía corresponde al constructor **CTR_RyuNET_Builder_EN**. Aunque la explicación está en español, los nombres de carpetas, archivos y botones se mantienen como aparecen en esa edición.

**Estado del borrador:** el constructor todavía no se ha adjuntado a este repositorio. El primer paso describe la descarga que se habilitará después de la revisión.

## 1. Extraer el constructor

Cuando esté disponible, descarga `CTR_RyuNET_Builder_EN.zip`. Haz clic derecho sobre él, elige **Extraer todo** y abre la carpeta `CTR_RyuNET_Builder_EN` que se obtiene. Trabaja desde esa carpeta extraída, sin ejecutar los botones desde el interior del ZIP.

**Para qué sirve:** el constructor necesita encontrar juntas sus carpetas, sus scripts y sus herramientas portátiles. Extraerlo completo evita errores por archivos que no se hayan copiado. En la edición portátil no necesitas instalar Python o el compilador por separado.

Deja espacio para los archivos temporales y el instalador, además de tus originales. El constructor comprueba el espacio al comenzar; con el ejemplo de juego base, actualización y DLC, el chequeo pide aproximadamente **55 GB libres**. La cantidad depende de tus entradas.

## 2. Entrar en Input y colocar el juego

Dentro de `CTR_RyuNET_Builder_EN`, abre **Input** y después **Game**. Coloca ahí un único PKG del juego base de **CUSA13795**.

**Para qué sirve:** `Input/Game` es la entrada del juego principal. El constructor lee sus metadatos para identificarlo. Cambiar el nombre de un archivo no cambia su CUSA ni vuelve compatible otra edición.

Si tu único PKG ya contiene el juego completo actualizado a **1.21**, también puede ir aquí: en ese caso deja `Input/Update` vacía. Un PKG que contiene solamente una actualización no sustituye al juego completo.

## 3. Colocar la actualización

Vuelve a **Input**, abre **Update** y coloca un único PKG de la actualización **1.21 para CUSA13795**, salvo que ya esté integrada en el juego completo del paso anterior.

**Para qué sirve:** la actualización aporta los ejecutables y datos que espera esta integración. El constructor prepara una combinación temporal del juego y la actualización; conserva los archivos originales que has colocado en las carpetas de entrada.

Si la comprobación rechaza la edición o los ejecutables, revisa tus entradas. Una actualización de otro CUSA no se vuelve compatible por renombrarla.

## 4. Añadir los DLC, si los tienes

Abre **Input/DLC** y coloca ahí los PKG de tus DLC compatibles con **CUSA13795**. Si no vas a utilizar DLC, deja la carpeta vacía. No pongas aquí el juego base ni la actualización.

**Para qué sirve:** el constructor reconoce los complementos por separado y prepara instaladores asociados a la aplicación resultante. Los DLC son opcionales y sus PKG se instalan después del principal; no se fusionan todos en un único instalador.

El ejemplo utilizado durante el desarrollo incluye Deluxe Pack. Eso no equivale a haber comprobado todos los DLC existentes en todas las consolas.

## 5. Revisar las herramientas

Vuelve a la carpeta principal y abre **0_DIAGNOSTICS.cmd**. Lee el resultado de la ventana y cierra el diagnóstico cuando termine.

**Para qué sirve:** comprueba que las herramientas portátiles incluidas pueden ejecutarse. No genera un PKG ni modifica la PS4. Si indica que falta el runtime, vuelve a extraer el ZIP completo antes de continuar.

## 6. Comprobar lo que has colocado

Abre **1_CHECK_FILES.cmd**. Revisa que reconozca el juego, el CUSA, la actualización y los DLC que hayas añadido.

**Para qué sirve:** comprueba la distribución de las entradas y sus metadatos antes de comenzar el trabajo largo. Todavía no construye el instalador. La extracción y las comprobaciones posteriores validan también los ejecutables que necesita el port.

## 7. Crear el PKG

Abre **3_BUILD_PKG.cmd** y deja la ventana abierta hasta que muestre **Finished** y la carpeta del resultado. No ejecutes dos construcciones al mismo tiempo.

**Para qué sirve:** este paso extrae las entradas, prepara los datos, compila y prueba la integración, construye el paquete y comprueba el instalador. Usa **Work** como espacio temporal y deja el resultado en **Output**.

La línea inferior muestra el porcentaje aproximado, la etapa y el tiempo transcurrido. **Stage left (~): calculating...** significa que todavía no hay una estimación fiable del tiempo de esa etapa. Durante **Building and testing** puede permanecer un rato en el mismo paso mientras se ejecutan pruebas.

Si necesitas comprobar qué hace, utiliza la ruta de **Build log** que imprime la ventana. No concluyas que terminó por ver un archivo grande: el cifrado y las verificaciones todavía pueden estar trabajando.

### ¿Y para qué sirve 2_PREPARE_FILES.cmd?

Es una alternativa opcional para **extraer y comprobar los archivos sin crear un PKG**. No es un requisito del paso 3. Si ejecutas el 2 y después el 3, el 3 vuelve a preparar las entradas en otra carpeta de trabajo.

Para el uso habitual basta con comprobar las entradas y ejecutar el **3**. El **2** sirve cuando solo quieres obtener una preparación y revisar sus archivos.

## 8. Encontrar el instalador terminado

Abre **Output** y entra en la carpeta de la construcción más reciente. Dentro encontrarás:

```text
CTR Nitro-Fueled Online - RyuNET.pkg
INSTALL.txt
DLC/                                  ← si añadiste DLC
```

**Para qué sirve:** el PKG principal es la aplicación que instalarás en PS4. `INSTALL.txt` recuerda el orden de instalación. La subcarpeta `DLC` contiene los instaladores de los complementos que hayas preparado.

Para compartir el constructor limpio, conserva el ZIP original. Tus carpetas `Input`, `Work` y `Output`, una vez utilizadas, contienen material propio y no forman parte del constructor limpio.

## 9. Llevar el resultado a PS4 e instalarlo

Con el juego cerrado, copia el PKG principal al medio de instalación que ya utilices con tu PS4. Abre **Package Installer** en tu configuración de GoldHEN e instala primero **CTR Nitro-Fueled Online - RyuNET.pkg**. Si generaste DLC, instala después los PKG de la carpeta **DLC**.

**Para qué sirve:** primero se instala la aplicación a la que pertenecen los complementos. El constructor de la laptop prepara los archivos; la instalación se realiza en la consola. El medio utilizado debe admitir un archivo de más de 4 GB.

Si sustituyes una instalación que utilizabas, conserva antes una copia de tus partidas. No necesitas borrar tus datos para que otro usuario local tenga su propia identidad de RyuNET.

## 10. Elegir tu identidad de RyuNET

Abre la aplicación en PS4. En el asistente, elige un apodo de **3 a 16 caracteres** usando letras, números, guion o guion bajo. Guarda el cambio, cierra el juego normalmente y vuelve a abrirlo.

**Para qué sirve:** se prepara una identidad de RyuNET para ese usuario local. Al abrir el juego desde otra cuenta local de PS4, esa cuenta puede configurar su propio perfil. No tienes que utilizar como apodo tu nombre de PSN ni el de otra persona.

Si omites el asistente, puedes jugar offline y configurar después el apodo desde **L3+R3 → Online → My nickname**. Las identidades y claves personales se guardan en tu consola; no se comparten con el constructor.

## 11. Entrar a Online y abrir los ajustes

Entra en **Online** desde el menú del juego. Para los ajustes adicionales, presiona a la vez **L3+R3**, es decir, pulsa ambos sticks hacia dentro. Consulta [la guía del menú](MENU_L3_R3.md) para cada opción.

**Para qué sirve:** el Online utiliza RyuNET. L3+R3 abre los ajustes propios de esta adaptación para gestionar el apodo, los contactos y los gráficos. La disponibilidad del servicio y la compatibilidad de los clientes también intervienen en la conexión.

## Si aparece un problema

### El menú sigue en español después de instalar la edición inglesa

Si utilizaste una prueba antigua con un parche de GoldHEN que cargaba el módulo externo de RyuNET, cierra el juego y revisa esa redirección antigua antes de reconstruir otro PKG. Desactiva únicamente ese parche y vuelve a abrir la aplicación instalada.

**Por qué puede pasar:** el parche antiguo puede cargar el módulo español de `/data/ryunet/ctr_online.prx` en lugar del módulo incluido en el PKG. El idioma del menú personalizado corresponde a su módulo; cambiar el idioma del sistema no traduce esos textos. Esta incidencia no requiere desactivar GoldHEN entero.

### No hay espacio suficiente

Libera espacio o utiliza una ubicación con capacidad suficiente y vuelve a ejecutar el paso correspondiente. Conserva tus originales y partidas al elegir qué retirar.

**Por qué ocurre:** durante la construcción conviven las entradas, los datos preparados y el instalador. El espacio necesario supera el tamaño del ZIP del constructor.

### No aparece el amigo o no permite unirse

Comprueba el apodo exacto de RyuNET, que ambos clientes sean compatibles y que exista una sala con plazas esperando antes de la carrera. Si la lista conserva un estado antiguo, cierra y vuelve a abrir los clientes para renovar la consulta.

**Para qué sirve:** distingue un contacto mal escrito, una consulta antigua o una sala no disponible de un fallo de construcción. Una prueba en la misma red no demuestra que funcionen todas las conexiones entre casas o países.
