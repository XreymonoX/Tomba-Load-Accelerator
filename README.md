# Tomba Load Accelerator / Acelerador de carga para Tomba

Small Windows tool that speeds up CD loading times in the PC releases of **Tomba! 1** and **Tomba! 2**
by patching the running game **in memory**. The game `.exe` is never modified, and everything can be
undone with one click (or by closing the game).

Pequeña herramienta para Windows que acelera los tiempos de carga del CD en las versiones de PC de
**Tomba! 1** y **Tomba! 2** modificando el juego **en memoria**. El `.exe` del juego no se toca y todo
se puede deshacer con un clic (o cerrando el juego).

## Features / Funciones

|Option|What it does|
|-|-|
|Read speed (max 16)|Shortens the time between CD sectors. Audio (CDDA/XA) automatically keeps its original timing, so music is not sped up.|
|Seek / startup|Shortens seek and read-start delays (can go much higher than read speed, needs more testing).|
|Disable rewind|Disables the rewind feature (keyboard and gamepad).|
|Auto-apply|Applies the patch automatically whenever the game opens.|
|Restore original|Reverts everything without closing the game.|

Each option has its own checkbox. / Cada opción tiene su propia casilla.

## Usage / Uso

1. Start the game. / Abre el juego.
2. Run `Tomba-Accelerator.exe` (English) or `Tomba-Accelerator.exe` (Español).
3. Press **Find**, then **Apply patch**. / Pulsa **Buscar** y luego **Aplicar parche**.

If the game runs as administrator, run the tool as administrator too.
Si el juego se ejecuta como administrador, ejecuta también la herramienta como administrador.

Without building an exe you can use the scripts in `src/` through the included `.bat` launchers.

## Supported versions / Versiones compatibles

The patch checks the game's code before writing and refuses to do anything if it does not match.
It was written against these executables (SHA-256):

|Game|SHA-256|
|-|-|
|Tomba 2|`664d1508534a0c2975c95a9ccfb369d35a9d073c4363b4f8da7740568dc25ac8`|
|Tomba 1|`7c3d76cbb80b925d3586421c97f137af9909ba55d16718826ebf873a5af1d11e`|

Other builds have different offsets and will be rejected. / Otras versiones tienen otros offsets y serán rechazadas.

## Disclaimer

Not affiliated with or endorsed by the game's publishers or developers. No game files are included.
Use at your own risk, and only with copies of the game you legitimately own.

## 

