# Resident Evil 5 — Mejoras de calidad de vida

Lista completa de correcciones, restauraciones, mejoras y modificaciones opcionales.

## Índice

- [Correcciones generales](#correcciones-generales)
- [Correcciones del modo de pantalla dividida](#correcciones-del-modo-de-pantalla-dividida)
- [Correcciones del teclado y ratón](#correcciones-del-teclado-y-ratón)
- [Correcciones de idiomas](#correcciones-de-idiomas)
- [Correcciones para partidas con mods](#correcciones-para-partidas-con-mods)
- [Modificaciones opcionales](#modificaciones-opcionales)

## Correcciones generales

*Correcciones que mejoran la experiencia del juego original.*

- Se ha restaurado la búsqueda de rutas de los enemigos. Esto **no** está relacionado con los problemas de colisión provocados por las tasas de fotogramas elevadas.
- Se han incorporado opciones de gestión del inventario de la versión de Nintendo Switch, aplicables a los objetos del juego (armas, munición, granadas, hierbas curativas, etc.):
  - **Dar todo** y **Pedir todo** permiten transferir objetos sin respetar la cantidad máxima establecida para cada entrega (por ejemplo, 30 balas de pistola o 1 huevo). La segunda opción solo está disponible con un compañero controlado por la CPU, ya que corresponde al otro jugador decidir cuánto quiere darte. Si pulsas el botón de dar con el inventario cerrado, se utilizará la última opción seleccionada. Esta preferencia se restablece al cargar un nivel y vuelve a la opción original «Dar».
  - La opción **Intercambiar** permanece disponible en el inventario del compañero, incluso cuando el tuyo no está lleno.
  - La opción **Combinar** solo aparece cuando el objeto puede combinarse con otro.
- Se han restaurado los iconos del inventario eliminados en la actualización 1.2.0:
  - El resaltado del objeto equipado.
  - La letra «E» que indica que un objeto está equipado.
  - El indicador de munición infinita.
- Se han añadido nuevos ajustes de calidad de sombras. Las opciones anteriores LOW, MEDIUM y HIGH pasan a ser OFF, LOWEST y LOW, respectivamente. Las resoluciones de los mapas de sombras, en orden, son: desactivadas, 512, 1024, 2048, 3072 y 4096.
- Los giros rápidos al apuntar ahora se muestran correctamente en partidas en línea con tasas distintas de 30 FPS.
- Se ha corregido un bloqueo en la lista de sesiones que se producía al intentar entrar en una sala y recibir un mensaje de error.
- Ya no es posible cambiar repetidamente de personaje en las salas de Mercenarios y Versus manteniendo pulsados ambos gatillos. Esto reproduce el comportamiento del parche original de consolas y debería evitar actualizaciones excesivas en línea y posibles problemas de sincronización en las salas.
- En la versión 1.2.0, el mensaje «El otro jugador no está preparado» de las salas de Mercenarios y Versus mostraba el botón y el texto «Atrás» tanto al anfitrión como al invitado. Se ha corregido este error visual para que no aparezcan cuando no eres el anfitrión.
- Se ha corregido la posición del nombre del personaje en el inventario durante la partida. Consulta `InventoryNameType` en Modificaciones opcionales para obtener más información.
- Se ha añadido **Sin piedad** a Mercenarios Reunión, tomando como referencia Mercenarios Unidos, incluido su sistema de puntuación. En esta versión no es posible guardar récords y se desconoce si esto cambiará en el futuro.
- La pantalla de selección de personajes de Sin piedad ahora muestra correctamente los rangos de ese modo, en lugar de los del modo individual.
- Entrar mediante una invitación a una sala de Mercenarios en dúo desde los menús de Sin piedad ya no provoca que ese modo permanezca activado para uno de los jugadores, lo que ocasionaba problemas de sincronización.
- Se ha corregido la posición de un indicador del mando en la pantalla de resultados de Versus (error introducido en la actualización 1.2.0).
- Se ha renovado el menú de opciones:
  - Se han corregido las animaciones de transición entre menús.
  - Se han ajustado las coordenadas verticales para que coincidan con las animaciones de transición.
  - Se ha sustituido la opción «Predeterminado» por un acceso directo para restablecer los valores predeterminados.
- Se ha corregido parcialmente el ajuste de calidad general. Algunos parámetros, como el nivel de detalle (LOD), ahora se configuran correctamente tomando como referencia la versión de Games for Windows Live, aunque todavía falta bastante código.
- Se han recuperado líneas de voz del DLC que faltaban para Chris, Sheva y Jill. Aunque esto afecta principalmente a partidas con mods, ahora, por ejemplo, podrás oír a Chris o Sheva gritar «¡Josh!» cuando este muere en la campaña principal. Puede desactivarse desde Modificaciones opcionales.
- Jill (y cualquier otra mujer diestra) ahora dispone de una animación de recarga más adecuada para el S&W M29. Puede desactivarse desde Modificaciones opcionales.
- Se ha ampliado la compatibilidad con caracteres especiales en los nombres de usuario de Steam. Los caracteres no admitidos deberían aparecer como un cuadrado blanco («□») en lugar de símbolos ilegibles.
- Se han corregido bloqueos provocados al intentar descartar una casilla vacía del inventario. Había dos formas de reproducirlos:
  - Disparar un lanzacohetes sin munición infinita y dejar preparada la orden de descartarlo antes de que desapareciera.
  - Recargar un arma y dejar preparada la orden de descartar su munición antes de que desapareciera.
- El mensaje de la pantalla de título puede alternar libremente entre «Pulsa cualquier tecla» y «Pulsa Start», como ocurría antes de la versión 1.2.0.
- La animación de transición de letras desordenadas entre la selección de dificultad y los ajustes de red ahora espera a que aparezca el aviso de asistencia de acciones cuando se elige la dificultad Aficionado.
- Se ha corregido el funcionamiento defectuoso del bloqueo regional.
- Al intentar abrir el perfil de Steam de tu compañero desde una sala de Mercenarios como cliente (jugador 2), ya no se muestra tu propio perfil.
- Se ha eliminado la opción LAN, ya que dependía del código de Games for Windows Live y no funciona en Steam. Se recuperará si llega a corregirse.
- Se ha eliminado el concepto de tipo de partida de Versus, que era principalmente un vestigio de las versiones de Xbox y Games for Windows Live.
- Se han corregido varios problemas en los menús de Lost in Nightmares y Desperate Escape.
- Se ha corregido la escala (tamaño) de los personajes Josh, Barry y Rebecca (corrección realizada originalmente por maluc).
- Se han eliminado los contornos negros alrededor de objetos y personajes que aparecían al activar simultáneamente las sombras y el suavizado de bordes (antialiasing).
- Se ha adaptado una versión corregida de la pantalla de título ampliada verticalmente de Games for Windows Live (visible en relaciones de aspecto más estrechas, como 4:3) y se han restaurado las animaciones de células sanguíneas ausentes en todas las reediciones posteriores.
- El fondo negro semitransparente que aparece al leer documentos ahora se adapta correctamente a relaciones de aspecto más estrechas en Lost in Nightmares.
- Se ha corregido el funcionamiento del gestor de perfiles de jugador, lo que soluciona problemas como la imposibilidad de intercambiar armas con un compañero controlado por la CPU.
- Los avisos que aparecen al disponer por primera vez de contenido descargable ahora tienen en cuenta si ya se cumplen sus requisitos de desbloqueo. También se ha añadido el aviso que faltaba de Figuras adicionales.
- Todos los personajes controlados por la CPU ahora pueden ejecutar la mayoría de los ataques cuerpo a cuerpo. Aunque esto afecta principalmente a partidas con mods, antes Chris, por ejemplo, se negaba a ejecutar el golpe de seguimiento Haymaker contra enemigos como el Majini de ametralladora Gatling y el Majini gigante.
- El estilo del aviso Sí/No de la política de privacidad ahora coincide con el de los demás avisos del juego.
- La pistola M93R ya no da la impresión de atravesar enemigos cuando en realidad no lo hace (el efecto se apreciaba originalmente en paredes y suelos).
- El Reaper ya no se pasa exageradamente de altura en algunos de sus saltos verticales.
- Los indicadores de botones de pantalla dividida ya no aparecen en la pantalla de gestión de objetos después de intentar iniciar una partida de Lost in Nightmares o Desperate Escape en pantalla dividida y regresar al menú principal.
- La pistola enfundada de Jill BSAA ahora aparece y desaparece correctamente al equipar una pistola también en Mercenarios (en parte gracias a Henry).
- El modelo de baja resolución poligonal del lanzacohetes ya no aparece parcialmente invisible.
- Se han corregido las zonas de impacto de las estrellas de puntuación destructibles (corrección realizada originalmente por Syndeh).
- Se ha reducido la resolución mínima de 800×600 a 640×360. **ADVERTENCIA:** Algunas escenas pueden provocar un cierre inesperado en determinados momentos con el mensaje «Unsupported function». La resolución panorámica (16:9) más baja que debería evitar estos fallos es 1024×576. El juego sigue siendo completamente jugable si se omiten esas escenas antes de llegar a los planos problemáticos. Los casos conocidos son «Medicine» y «A Message from Jill», además de la escena equivalente a esta última en Desperate Escape.

## Correcciones del modo de pantalla dividida

*Correcciones destinadas a mejorar la experiencia en pantalla dividida.*

- La configuración de prioridad de objetos y el método de control ahora se respetan correctamente al entregar objetos desde la pantalla de gestión de objetos.
- La intensidad de vibración del mando funciona correctamente con cualquier combinación de métodos de control en pantalla dividida.
- Los indicadores en pantalla ya no aparecen más pequeños en chino al jugar en pantalla dividida.
- El nombre del jugador 2 siempre aparece como «Guest» en las salas de Mercenarios, en lugar de quedar en blanco con determinadas combinaciones de métodos de control.
- El jugador 2 vuelve a incorporarse correctamente como Chris Heavy Metal en Mercenarios Reunión, en lugar de Excella.
- Se ha añadido una solución provisional para el bloqueo en la pantalla «Save successful.». Ahora debería ser posible continuar hasta el menú principal utilizando el teclado.
- El desenfoque de movimiento funciona en pantalla dividida (y en otros modos de cámara sin utilizar) si se activa en los ajustes del sistema, lo que convierte a esta en la única versión del juego compatible con esta función.
- El archivo del tutorial de controles del capítulo 1-1 ahora se muestra correctamente para cada jugador cuando se combinan distintos métodos de control.

## Correcciones del teclado y ratón

*Ajustes y opciones adicionales para personalizar los controles con teclado y ratón.*

- Se han añadido nuevas opciones de teclado y ratón:
  - **Tipo de movimiento:**
    - **Tipo A:** gira al personaje con el ratón y desplázate lateralmente con las teclas A y D.
    - **Tipo B:** gira al personaje con las teclas A y D (controles tipo tanque). Los controles de cámara podrían cambiar en el futuro.
  - **Tipo de apuntado:**
    - **Predeterminado:** apuntas con la cámara y el personaje la sigue con cierto retraso.
    - **Clásico:** apuntas controlando directamente los brazos del personaje. La cámara los sigue con cierto retraso y dispone de una zona muerta en el centro (obliga a utilizar la mira láser).
    - **Apuntado con cursor:** la retícula se mueve libremente por la pantalla y permanece visible en todo momento (obliga a utilizar controles tipo tanque y la retícula de apuntado).
  - **Retícula de apuntado:**
    - **Predeterminada:** retícula de apuntado.
    - **Clásica:** mira láser (incluye la corrección del ángulo del láser).
  - Valores de sensibilidad del ratón independientes para la cámara y el apuntado.
  - Configuración alternativa de teclas para eventos de acción rápida (QTE): apuntar + disparar.
- Ahora es posible navegar por los menús con las teclas WASD.
- La tecla asignada a la acción contextual también sirve como acceso directo para mover objetos en el inventario.
- La rueda del ratón también permite cambiar de personaje en las salas de Versus.
- La tecla para alternar entre récord/rango máximo y enemigos eliminados/combo máximo en la selección de escenario vuelve a ser Mayús izquierda en lugar de Z, como en la opción equivalente de las clasificaciones del juego original y en nuestro parche anterior.
- Se ha añadido o corregido la compatibilidad con el ratón en numerosos menús.
- Se ha habilitado el movimiento de cámara con el ratón en las introducciones y secuencias finales de Versus y Mercenarios al utilizar controles con desplazamiento lateral.
- Se ha restaurado y ampliado la compatibilidad con la distribución numérica del inventario en varios modos de juego. Para utilizarla, hay que seleccionar manualmente la prioridad «Numérica» en los ajustes de teclado y ratón. Por motivos de compatibilidad, se desactiva al jugar con usuarios que no tengan el parche fuera de los modos Survivors y Team Survivors.
- Los controles de navegación por los menús ya no dejan de responder parcialmente en una sala en línea de Mercenarios después de completar una partida como cliente (jugador 2).
- Se han corregido algunos casos en los que la leyenda de controles del menú mostraba las teclas del teclado pese a utilizar un mando («(B)Back» en lugar de «(LS)Select (A)OK (B)Back»).
- Se han reorganizado las asignaciones de teclas de las salas de Versus para ajustarlas mejor a los menús originales.
- La tecla Inicio (Home) ahora puede asignarse a una función, ya que no se utiliza para abrir la interfaz de Games for Windows Live.
- El secreto de la cámara fija de Lost in Nightmares ahora puede jugarse por completo con teclado y ratón.

## Correcciones de idiomas

*Correcciones destinadas a mejorar la compatibilidad con distintos idiomas.*

- Se han corregido pequeñas erratas en inglés y español.
- Se ha incorporado la traducción al ruso del contenido descargable realizada por INSERTHERE, junto con mejoras generales de Infernal.
- Algunos textos del juego ya no están definidos directamente en el código, lo que permite realizar determinadas correcciones específicas de cada idioma:
  - «Chris Redfield» y «Sheva Alomar» en la selección de atuendos.
  - «Chris Redfield», «Josh Stone» y «Jill Valentine» en las listas de sesiones y clasificaciones de Lost in Nightmares y Desperate Escape.
  - Los nombres de los personajes en el inventario.
- Los sistemas de clasificación en ruso ya no utilizan el alfabeto cirílico, como habían solicitado varios miembros de la comunidad.
- Se ha recuperado la textura separadora de la selección de capítulos que faltaba en los idiomas eslavos.
- Se han restaurado los textos eslavos del menú de selección de personajes en los modos originales de Mercenarios y Versus.
- El tutorial del capítulo 2-1 ya no muestra nombres de personajes en ruso superpuestos a los ingleses.
- En español, a la pantalla «Tu compañero ha muerto» ya no le falta la letra que indica el género.
- Se ha recuperado el icono de la tecla «X» para abrir el inventario del compañero en español.
- Algunos nombres de la interfaz en ruso ya no aparecen en inglés (texturas proporcionadas por Syndeh).

## Correcciones para partidas con mods

*Correcciones que mejoran la experiencia al utilizar mods.*

- La reducción de potencia de la porra eléctrica de Mercenarios Reunión ahora también se aplica a Mercenarios original y a Versus.
- Los Blobs/Guardianes de la locura explotan al morir si se incorporan mediante mods a Versus, Desperate Escape o cualquiera de los dos modos de Mercenarios.
- Se han corregido los tiempos necesarios para romper las bonificaciones de tiempo con personajes para los que no estaban previstas originalmente (por ejemplo, Wesker en Mercenarios Reunión/Unidos).
- Algunas armas ahora deberían poder utilizarse con cualquier personaje, aunque no siempre sin fallos: arco largo, ametralladora Gatling, farol y lanzallamas.
- Se ha eliminado parcialmente una restricción que impedía a los personajes controlados por la CPU rematar a jefes y subjefes (solo en Mercenarios y Versus).
- Se han eliminado las restricciones que impedían intercambiar la Px4 y los cuchillos durante la partida.
- Se han corregido las líneas de voz para solicitar la Samurai Edge de Barry y todos los cuchillos.
- Se han corregido algunos iconos de objetos en la pantalla de gestión de objetos y se han reorganizado otros, como los de la Px4, las pistolas Samurai Edge y el escarabajo esmeralda sin utilizar.
- El escarabajo esmeralda ahora se vende por ₦2500 en lugar de 9.
- Al utilizar determinadas manivelas en Lost in Nightmares, los personajes ahora llaman correctamente a su compañero por su nombre real.
- Algunas animaciones, como las de accionar manivelas y palancas, ahora se orientan correctamente independientemente del género y la mano dominante del personaje.
- Correcciones de animaciones de armas:
  - Todas las mujeres diestras pueden utilizar la animación de recarga de Rebecca para la Jail Breaker.
  - Los cuchillos (excepto el de Jill) y las pistolas Px4 y Samurai Edge utilizan los conjuntos de animaciones correctos para personajes del género opuesto.
- Sustituir a Chris por otro personaje en Lost in Nightmares ya no bloquea la secuencia del piano cuando el personaje está controlado por la CPU.
- La animación de caminar tranquilamente del capítulo 1-1 ahora funciona con cualquier personaje y atuendo.
- Cambiar de personaje en la campaña principal ya no interrumpe el funcionamiento de la munición infinita.
- Se han corregido las animaciones de daño que faltaban al recibir ataques de los Blobs/Guardianes de la locura y de Wesker en Lost in Nightmares. La corrección puede desactivarse desde Modificaciones opcionales.
- El cuchillo del DLC y la Samurai Edge de Barry ahora otorgan puntos por el daño infligido a otros jugadores en Survivors y Team Survivors.
- La interfaz y los elementos del escenario se muestran cuando se fuerza a la cámara a seguir a un personaje controlado por la CPU.
- Los disparos de la Samurai Edge de Barry ya no se contabilizan automáticamente como fallidos.
- Se han corregido los ataques cuerpo a cuerpo Headbutt de Barry y Humiliate de Excella fuera de Mercenarios Reunión. Además, First Aid ya no provoca el cierre del juego.
- Se ha corregido el desplazamiento de la posición de la mano con el rifle S75 en personajes femeninos diestros. Todavía se necesita un conjunto de animaciones adecuado para que se vea correctamente.
- Se han corregido numerosos eventos de acciones cooperativas en los que el juego utilizaba el género para decidir qué debía hacer cada personaje; ahora se comprueba el número de jugador. Algunos ejemplos son las ayudas para saltar, la posición al derribar puertas de una patada, la apertura de portones grandes, el empuje de contenedores, la sección de la torreta y las escenas de la aerodeslizadora.

## Modificaciones opcionales

*Opciones que pueden añadir variedad, dificultad o diversión a la experiencia.*

> **OFF** y **0** = comportamiento original o previsto, salvo que se indique lo contrario.

Los valores numéricos suelen indicar que hay dos o más opciones disponibles.

### Jugabilidad

- `DisableInventoryReloads` — **ON:** impide recargar armas combinándolas con munición en el inventario.
- `SkipDyingState` — **ON:** cuando la barra de salud se vacía por completo, mueres inmediatamente, como en la mayoría de las entregas para un jugador de la saga (no funciona en Versus).
- `ProDyingBarOverride` — **1:** concede 3 segundos para reanimar o curar al compañero en Lost in Nightmares y Desperate Escape en dificultad Profesional. **2:** concede 8 segundos para reanimar o curar al compañero en la campaña principal en dificultad Profesional.
- `ExtraVoiceCommands` — **ON:** permite que los jugadores utilicen determinadas órdenes de voz que antes eran exclusivas de los personajes controlados por la CPU (función implementada originalmente por maluc, aunque de forma ligeramente distinta):
  - Al curar o reanimar al compañero.
  - Al entregarle objetos.
  - Al recargar (10 % de probabilidad).
- `ExtraGestureCommands` — **ON:** permite que los jugadores utilicen la orden para pedir al compañero que recoja munición, antes exclusiva de los personajes controlados por la CPU.
- `ExtraAICommands` — **ON:** habilita las órdenes «Gracias» y «Alto» al jugar con un compañero controlado por la CPU.
- `HideReticles` — **ON:** oculta por completo las retículas de apuntado y las miras láser.
- `LaserDotType` — **ON:** hace visible el punto del láser en todas las superficies sólidas, como en RE6.
- `AimDisablesMelee` — **ON:** oculta los indicadores de ataques cuerpo a cuerpo mientras apuntas. Solo se aplica a los tipos de control A y C del mando.
- `ReloadAiming` — **ON:** permite apuntar durante la recarga, de forma similar a apuntar entre disparos con el rifle de francotirador S75. Está inspirada directamente en los tráileres y demostraciones del E3 y, al parecer, se eliminó en una fase avanzada del desarrollo. Solo funciona con mando y con el tipo de apuntado clásico de teclado y ratón.

### Interfaz de usuario

- `InvertConfirmCancel` — **ON:** invierte los botones de confirmar y cancelar al navegar por los menús, como en las PS3 japonesas y Nintendo Switch.
- `InvertBumperTrigger` — **ON:** intercambia LB/LT y RB/RT en determinadas situaciones, tomando como referencia principalmente la versión de PS3. En esta versión, los QTE no cambian y los tipos de control A y C no muestran correctamente el botón para localizar al compañero cuando este está esperando o agonizando fuera de la pantalla.
- `DisableInputNotification` — **ON:** deja de mostrar un mensaje cada vez que se cambia entre mando y teclado y ratón (implementado originalmente por maluc).
- `DisableHUDNames` — **1:** oculta únicamente los nombres de los personajes, pero conserva la textura de fondo que facilita su lectura. **2:** elimina por completo los nombres, como en The Mercenaries 3D (útil si cambias de mods de personajes constantemente).
- `DisableGameVerText` — **ON:** elimina el texto de versión de la pantalla de título (originalmente «1.2.0» y ahora «QOL YY/MM/DD»).
- `InventoryNameType` — **0:** coloca el nombre ligeramente desplazado hacia la izquierda, como en la mayoría de las versiones de consola. **1:** centra tu nombre, ya que no es necesario reservar espacio para el botón del inventario del compañero. **2:** oculta por completo los nombres del inventario (útil si cambias de mods de personajes constantemente).
- `InventoryNumberFontSize` — **ON:** aumenta el tamaño de los números del inventario para facilitar su lectura en pantallas pequeñas, especialmente en pantalla dividida (basado directamente en la versión de Nintendo Switch).
- `TitleLogoOverride` — **1:** fuerza el título «Biohazard 5». **2:** fuerza el título «Resident Evil 5».
- `GoldLogoOverride` — **1:** fuerza el logotipo «Alternative Edition». **2:** fuerza el logotipo «Gold Edition». **3:** lo desactiva por completo.
- `SkipTitleVoiceDelay` — **ON:** al seleccionar «Start Game», el juego comienza inmediatamente a crear o cargar la partida guardada mientras el narrador sigue hablando. Es **similar** al comportamiento de la versión de Nintendo Switch.
- `CustomFrameRate` — Debe establecerse un valor entre 10 y 10000. Sustituye el ajuste del límite de 120 FPS (originalmente llamado «Unlocked» o «Variable», según el idioma).
- `ControllerIcons` — **0:** Xbox 360. **1:** PS4. Es posible que esta función se rediseñe en el futuro y se añada compatibilidad con los iconos de PS3 y Nintendo Switch.
- `UnitedTitleScreen` — **ON:** cambio **SOLO VISUAL** que sustituye la pantalla de título de Mercenarios Reunión por la de Mercenarios Unidos, utilizada en las reediciones posteriores para consolas.
- `RemoveLetterboxing` — **ON:** fuerza el modo de cámara estándar cuando el juego intenta cambiar al cinematográfico, que añade franjas negras arriba y abajo de la pantalla. Ten en cuenta que, si juegas en 16:9 (panorámico), el campo de visión será más estrecho, ya que las versiones originales utilizaban una relación de aspecto similar a la ultrapanorámica para esas escenas.
- `ExtraHudTweaks` — **ON:** activa el contador de enemigos eliminados en Mercenarios.

### Varios

- `CheapVsCharacters` — **ON:** todos los personajes de Versus cuestan 2000 puntos en el menú de características adicionales. Basado directamente en las reediciones posteriores para consolas.
- `UnlockMercs` — **ON:** permite acceder a los dos modos de Mercenarios sin necesidad de terminar primero el juego. Basado directamente en las reediciones posteriores para consolas.
- `UnlockPro` — **ON:** permite acceder a la dificultad Profesional sin tener que completar primero los distintos modos en Veterano ni unirse a una partida de un anfitrión en Profesional para desbloquearla permanentemente en el perfil local.
- `UnlockStoryCharacters` — **ON:** permite jugar con Sheva, Jill y Josh en la campaña principal, Lost in Nightmares y Desperate Escape, respectivamente, sin tener que completar antes esos modos.
- `RemoveFilter` — **1:** opción menos agresiva. Conserva ciertos efectos, como los que aparecen cuando estás agonizando, pero no funciona en las escenas cinemáticas. **2:** opción más agresiva. Funciona en las escenas cinemáticas, pero también elimina algunos efectos de posprocesado.
- `RE4MercsScoring` — **ON:** los valores de bonificación por combo coinciden con los del modo Mercenarios del RE4 original. Las bajas cuerpo a cuerpo no añaden 5 segundos y no se conceden puntos adicionales por cada segundo restante al eliminar 150/400 enemigos.
- `FourPlayerMercs` — **ON:** permite jugar en línea con hasta cuatro jugadores en Mercenarios. Mientras esté activada, las puntuaciones no se guardarán (ni en individual ni en dúo en línea) ni se subirán a las clasificaciones (en ningún caso), independientemente del número de jugadores.
- `RandomMinigameBGM` — **ON:** reproduce aleatoriamente los temas musicales de Mercenarios y Versus. Cambia la música con cada reinicio rápido y requiere el contenido descargable:
  - Assault Fire (The Mercenaries)
  - Killers (Survivors)
  - Rust in Summer 2008 (Slayers)
  - The Mercenaries Reunion

### Compatibilidad con mods

- `IgnoreMissingFiles` — **ON:** impide que el juego se cierre automáticamente al detectar archivos esperados que faltan, aunque todavía podría cerrarse sin previo aviso si falta un archivo esencial o está dañado.
- `SnWM29Fix` — **ON:** utiliza un conjunto de animaciones personalizado que permite a los personajes femeninos diestros recargar correctamente el revólver S&W M29.
- `JailBreakerFix` — **ON:** utiliza un conjunto de animaciones personalizado que permite a **todos** los personajes femeninos diestros recargar correctamente la escopeta Jail Breaker.
- `MissingVoiceLinesFix` — **ON:** utiliza archivos `stq` personalizados para garantizar que los atuendos de Chris, Sheva y Jill que no pertenecen a los DLC tengan acceso a las líneas de voz adicionales de estos contenidos.
- `DamageAnimationsDLCFix` — **ON:** obliga a todos los personajes a utilizar el conjunto actualizado de animaciones de Lost in Nightmares para que reaccionen correctamente a los nuevos ataques de Wesker y al ácido de los Blobs.
- `TextFixes` — **ON:** utiliza archivos de texto personalizados del juego para garantizar que todos los textos nuevos y corregidos se muestren correctamente, independientemente de los mods instalados.
- `HudIconFixes` — **ON:** desactiva las correcciones de la interfaz que dependen de un archivo `cp_life_360.lsp` modificado, como las relacionadas con las texturas de nombres de personajes que faltan en los modos ajenos a los DLC.
