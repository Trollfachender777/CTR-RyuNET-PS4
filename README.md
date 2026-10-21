# CTR Nitro-Fueled Online - RyuNET

**Borrador privado en revisión.** Por ahora este repositorio contiene la presentación, las instrucciones y los créditos. Las descargas y la publicación pública quedan pendientes de revisión.

Una adaptación no oficial para jugar a **Crash Team Racing: Nitro-Fueled en PS4 con RyuNET**, el servicio comunitario utilizado por OCTR en PC. El juego se ejecuta en la consola; la laptop se utiliza para preparar el instalador.

La idea es facilitar la preparación de una instalación a partir de los archivos de cada jugador y ofrecer ajustes propios para PS4 desde **L3+R3**.

## Qué ofrece esta adaptación

- Constructor local para Windows de 64 bits, con sus herramientas portátiles.
- Asistente inicial e identidad de RyuNET independiente para cada usuario local de PS4.
- Apodo propio de RyuNET, separado del nombre de PSN.
- Límites de 30 y 60 FPS, con «Unlimited» como opción aparte.
- Resolución interna Native, 720p o 480p, opciones de desenfoque y sombras dinámicas, y restauración de gráficos.
- Gestión de contactos y unión a partidas mediante el menú Amigos del propio CTR, con clientes compatibles.

El límite de 60 FPS es un tope: el rendimiento real depende de la pista y de la consola. Las invitaciones no están implementadas en esta adaptación.

## Antes de empezar

Esta integración admite **CUSA13795 con la actualización 1.21 y ejecutables compatibles**. Cada persona aporta su juego, actualización y DLC opcionales. No se distribuyen archivos del juego, partidas, cuentas ni claves personales.

La referencia de red utilizada es **OCTR 0.5.3**. Las versiones posteriores de PC pueden incorporar funciones que todavía no están adaptadas o comprobadas aquí. No se garantiza compatibilidad con todos los CUSA, versiones de firmware ni condiciones de red.

## Lee las instrucciones en este orden

1. [Preparar los archivos, construir el PKG e instalarlo](GUIA_DE_USO.md).
2. [Configurar los FPS, los gráficos, el apodo y los amigos](MENU_L3_R3.md).
3. [Autores, proyectos de referencia y herramientas](CREDITOS.md).

La guía explica primero **qué hacer** y, debajo de cada paso, **para qué sirve**. Sus nombres de carpetas y botones corresponden a la edición inglesa `CTR_RyuNET_Builder_EN`.

## Agradecimientos principales

Este trabajo parte de [OCTR y RyuNET, de Ryu7w7 y sus colaboradores](https://github.com/Ryu7w7/OCTR-NitroFueled-PC), y del [port de Windows de GetLostIn](https://github.com/GetLostIn/CTR-NitroFueled-PC). Los créditos completos incluyen SacredFire, bbport, shadPS4 y las herramientas de desarrollo.

La adaptación para PS4 no se atribuye la creación del port original de PC ni del servidor RyuNET. Es un proyecto comunitario independiente, sin afiliación oficial con los titulares del juego.

## Estado de las comprobaciones

Se han comprobado la construcción completa con archivos propios, la lectura de ejecutables desde el PKG generado y las pruebas locales del módulo. El autor ha confirmado el arranque, el acceso a Online y perfiles distintos al cambiar de usuario local en su consola. Una prueba en una consola no demuestra funcionamiento en todos los equipos o redes.

Antes de la publicación se revisarán juntos estos textos, los archivos que se compartirán y los avisos de licencia correspondientes.
