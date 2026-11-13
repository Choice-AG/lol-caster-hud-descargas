# LoL Caster HUD

Overlay para retransmitir partidas de **League of Legends** desde el modo espectador: se pone encima del juego en OBS y le da aspecto de emisión oficial (marcador, estadísticas 5v5, dragones, power plays, intros, pantallas de pausa…). Se controla desde un panel en el navegador, el móvil o atajos de teclado.

https://github.com/user-attachments/assets/1dacfd11-fb92-4412-833d-0823f5df337a

### **[⬇ Descargar la última versión](https://github.com/Choice-AG/lol-caster-hud-descargas/releases/latest)**

Un solo archivo, `LoL-Caster-HUD.exe` (~80 MB). No hay que instalar nada ni crear cuentas.

---

## Qué necesitas

- **Windows 10 u 11** (64 bits) con League of Legends.
- **OBS 28 o posterior.**
- Resolución del juego **1920×1080 o 2560×1440** (probadas las dos).

## Primera vez (5 minutos)

1. **Crea una carpeta** para el programa (por ejemplo `Documentos\LoL Caster HUD`) y mete ahí `LoL-Caster-HUD.exe`. Al abrirlo crea a su lado la carpeta `datos`, donde guarda tus ajustes, logos y patrocinadores.
2. **Ábrelo con doble clic.**
   - Si Windows dice «Windows protegió su PC»: **Más información → Ejecutar de todas formas**. Solo pasa esta vez: las actualizaciones se hacen desde el panel y ya no sale.
   - No sale ninguna ventana: el programa queda funcionando con su **icono junto al reloj de Windows** (si no lo ves, está en la flecha «^»). **Doble clic** en el icono abre el panel; **clic derecho → Cerrar LoL Caster HUD** lo apaga (también en el panel: Configuración → Programa).
   - Se abre el **panel de control** en el navegador. Si lo cierras, vuelve a abrir el `.exe` o entra en `http://localhost:8787/control`.
3. En el panel, pestaña **Configuración**:
   - **API de repeticiones del juego**: si sale desactivada, **cierra el LoL** y pulsa «Activar». Hace falta para ocultar la interfaz del juego y leer el CS exacto. Un punto naranja en la pestaña avisa si falta.
   - **Añadir a OBS**: en OBS ve a *Herramientas → Ajustes del servidor WebSocket*, marca «Habilitar servidor WebSocket», pulsa «Mostrar información de conexión», copia la contraseña, pégala en el panel y pulsa **«Añadir a OBS»**. Crea la escena **«LoL Caster HUD»** con la captura del juego y el HUD encima. La contraseña no se guarda.
4. Listo. No hace falta ninguna clave de Riot.

## En cada partida

1. Abre el `.exe` (y OBS).
2. Pestaña **Partida**:
   - **Equipos**: elige cada uno del desplegable **«Equipo guardado»** o escribe nombre, subtítulo y logo (con **«Guardar en la lista»** queda guardado para la próxima vez). **⇄ Intercambiar lados** lo cambia todo de golpe.
   - **Nombres de jugadores**: el nombre que sale en el HUD en lugar del Riot ID. **«Añadir los de la partida»** trae los 10 jugadores; escribe sus nombres y pulsa «Guardar nombres» (se quedan guardados).
   - Logo de la **liga** (sale bajo el reloj), formato de la serie (BO1/BO3/BO5) y marcador, y nombres de los **casters**.
3. Entra como **espectador** en la sala personalizada, o abre una **repetición**.
4. En el juego deja visible el **panel de abajo con los jugadores** (en OBS lo tapa el del HUD): de ahí se leen el CS, los números de los objetos y el oro exactos. Lo demás del juego (kill feed, timers, barra de la repetición) lo esconde el HUD solo.

Arriba del panel se ve si hay partida conectada y si hay línea de tiempo de Riot.

En la pestaña **En directo** tienes dos monitores con el juego de fondo: **Vista previa** y **En emisión** (lo que sale en OBS). Con «Vista previa antes de emitir» activada, al pulsar la intro, la gráfica de oro, el resumen de pelea o una pantalla, primero sale en la vista previa y no va a OBS hasta que pulsas **«Emitir ▶»**. Así ves cómo queda antes de sacarlo.

## Qué se ve en pantalla

**Siempre**
- **Marcador de arriba**: logos, nombres, serie (barras de partidas ganadas), kills, torres, oro y diferencia de oro, tiempo, y una franja con los dragones (y el alma), larvas y Barones de cada equipo.
- **Estadísticas 5v5 abajo**: campeón, nivel, vida y maná/energía/furia, **definitiva y hechizos** (con los segundos de recarga), KDA, CS, visión y objetos en el mismo orden y con los mismos números que el juego (Soberbia, Corazón de acero, pociones, Preferencia…; a 1080p se leen la mayoría y, si uno no se lee entero, no se pone). Junto al trinket, la **misión de rol** de cada jugador: en gris mientras está en curso y, al completarla, su recompensa con borde dorado (en el ADC, sus botas, que pasan a ese hueco). Se resalta al jugador que sigue la cámara.
- **Arriba a la izquierda**: cuenta atrás del próximo dragón y Barón, cajas de **power play** (Barón y Ancestral) con el oro ganado, y aviso cuando **aparece** un objetivo.
- **Kill feed** con asistencias, torres, inhibidores y objetivos, y timers de inhibidores y torres de nexo caídos.

**Cuando pasa algo**
- Retratos con splash art del asesino (KILL, DOUBLE KILL… PENTAKILL) y la víctima; anuncios grandes en el centro para pentas, aces y robos.
- Avisos de nivel 6/11/16, objetos completos y **shutdowns**.

**Lo que lanzas tú** (pestaña **En directo**, mando o atajos)
- **7 intros** de inicio y las **alineaciones** con las 10 splash arts (salen solas al empezar la partida).
- **Gráfica de la diferencia de oro** (15 s).
- **Pantallas**: «Empezamos en breve» (con cuenta atrás), «Pausa técnica», «Volvemos enseguida».
- **Pantallas de liga**: **Clasificación** (victorias, derrotas y % de cada equipo, ordenada sola, con los dos de la partida marcados) y **Próximo partido** (los dos equipos, la hora o una cuenta atrás y una nota), con el logo de la liga. Se rellenan en la pestaña **Partida** («Añadir los equipos guardados» mete toda tu lista).
- **Resumen de la última pelea** (botón «Resumen de la última pelea», también en el mando): por equipo sus kills, sus muertes y lo que ha gastado cada jugador (definitiva y hechizos); en el centro el resultado (p. ej. 1 – 3), quién gana y el oro movido. Si lo quieres automático al acabar cada pelea, actívalo en la pestaña HUD.
- **Pantalla de final**: VICTORIA con la comparativa de los dos equipos. En repeticiones sale sola.
- **Casters** y **patrocinadores** en la esquina de abajo a la izquierda (tapan el panel de cámara del juego, no la ficha del jugador): los casters a la izquierda y el patrocinador a la derecha; si solo hay uno, ocupa la esquina entera. Para los patrocinadores van mejor logos de unos **220×150** (pestaña **HUD**, con interruptor para apagarlos al momento).

## Atajos y mando

Funcionan aunque tengas el juego delante: **Ctrl + Alt + número**.

| Tecla | Acción | Tecla | Acción |
|---|---|---|---|
| 1 | Gráfica de oro | 6 | Quitar pantalla |
| 2 | Alineaciones | 7 | Gana azul |
| 3 | Pausa técnica | 8 | Gana rojo |
| 4 | Volvemos enseguida | 9 | Quitar final |
| 5 | Empezamos en breve | 0 | Intro |

**Desde el móvil** (misma WiFi que el PC): en **Configuración → Mando y atajos** aparecen la dirección y un **PIN de 6 cifras**. Ábrela en el móvil, mete el PIN y tendrás botones grandes con las mismas acciones. Sin el PIN no se puede tocar nada.

## Directo y repeticiones

| | En directo (espectador) | Repetición |
|---|---|---|
| CS, objetos, oro de cada equipo, vida, definitivas | Exactos (leídos del juego) | Exactos (leídos del juego) |
| Oro de cada jugador | Valor de sus objetos | Real (de la línea de tiempo de Riot) |
| Dragones, Barón, larvas, torres | Sí | Sí (de la línea de tiempo de Riot) |
| Pantalla de final | Con los botones «Gana azul / rojo» | Sale sola |

Las repeticiones usan la **línea de tiempo oficial de Riot**, que se descarga sola sin poner clave. Solo existe para partidas que Riot registra: las personalizadas sin código de torneo no suelen tenerla.

## Problemas frecuentes

- **No se ve nada en OBS**: comprueba que el icono del programa sigue junto al reloj (si no, vuelve a abrir el `.exe`) y pulsa **Configuración → Recargar el HUD en OBS**.
- **Algo falla y no sabes por qué**: lo que hace el programa queda apuntado en `datosegistro.txt` (y la vez anterior en `registro-anterior.txt`), junto al `.exe`.
- **El CS o los números de los objetos no cuadran**: el panel de abajo del juego tiene que estar visible y la ventana del LoL sin minimizar (puede estar detrás de otras). Usa 1920×1080 o 2560×1440 con la escala de la interfaz del juego por defecto. Si no se puede leer, el HUD estima esos números.
- **«Activar» la API de repeticiones no funciona**: tiene que estar el LoL **cerrado** (se guarda antes una copia de su configuración).
- **Un atajo sale como ocupado**: otro programa usa esa combinación; ciérralo o usa el panel o el mando.
- **El móvil no conecta**: tiene que estar en la misma WiFi. Si Windows pregunta, permite el programa en **redes privadas**.

## Actualizar

Cuando hay versión nueva (se mira cada 30 minutos), el panel la anuncia arriba: pulsa **«Actualizar ahora»** (mejor entre partidas, porque el HUD se recarga). El programa la descarga, se cambia solo y se reinicia; tus ajustes se conservan y **el aviso de Windows ya no sale**.

Si tienes la 0.1.3 o anterior, el botón aún no existe: esa vez cierra el programa, descarga el `.exe` nuevo y sustituye el viejo (la carpeta `datos` se conserva).

## Seguridad

Lee los datos de la API oficial que el propio juego expone en tu PC y capturas de la pantalla del juego: **no lee memoria ni modifica el juego**, así que no hay riesgo con el anti-cheat. Todo se queda en tu PC salvo las imágenes de campeones (Riot), la línea de tiempo de las repeticiones y la comprobación de versiones nuevas.
