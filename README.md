# LoL Caster HUD — descarga

Overlay de retransmisión para el modo espectador de League of Legends (OBS), con panel de control en el navegador.

**[Descargar la última versión](https://github.com/Choice-AG/lol-caster-hud-descargas/releases/latest)** → `LoL-Caster-HUD.exe` (~80 MB, no hace falta instalar nada).

## Qué necesitas

- Windows 10 u 11 (64 bits) con League of Legends.
- OBS 28 o posterior (para añadir la escena desde el panel).

## Cómo se usa

1. Pon `LoL-Caster-HUD.exe` en una carpeta propia (por ejemplo `Documentos\LoL Caster HUD`): al abrirlo crea ahí la carpeta `datos` con tus ajustes, logos y patrocinadores.
2. Ábrelo con doble clic. Windows puede avisar de que es una aplicación desconocida (no está firmada): «Más información → Ejecutar de todas formas».
3. Se abre una ventana negra (déjala abierta mientras retransmites; al cerrarla se apaga) y el panel de control en el navegador (`http://localhost:8787/control`).
4. En el panel, **Puesta en marcha**:
   - **API de repeticiones del juego:** si sale desactivada, cierra el juego y pulsa «Activar».
   - **Añadir a OBS:** en OBS activa *Herramientas → Ajustes del servidor WebSocket*, copia la contraseña, pégala en el panel y pulsa «Añadir a OBS».
5. Entra como espectador en la sala personalizada (o abre una repetición).

## Bueno es saber

- El CS, los números de los objetos y la recompensa se leen del panel inferior del propio juego: déjalo visible en el juego (en OBS lo tapa el del HUD). Probado a 2560×1440; con otras resoluciones puede no leerse y el HUD estima esos números.
- En directo el oro es el valor de los objetos. Para repeticiones de partidas terminadas puedes poner tu propia clave de la API de Riot en el panel (opcional).
