# Digimon World 2003: Harmony — Beta 1.5

**16 de octubre de 2026 · Build r48**

Changelog acumulativo desde la última actualización de **Beta 1.0: r31**, publicada como descarga corregida el 10 de octubre. Beta 1.5 corresponde al parche `dw2003-harmony-beta1.5.bps`.

Esta actualización amplía los árboles de los ocho rookies, revisa la progresión de evoluciones y técnicas, refuerza la identidad de los Special y corrige fallos de inventario y venta detectados en Beta 1.0.

## Correcciones de inventario, misiones y tiendas

- Corregida la comprobación contradictoria que podía considerar un objeto presente y ausente al mismo tiempo. Este fallo podía seleccionar diálogos y apariciones de NPC incompatibles, repetir entregas de objetos clave o volver a la rama inicial de una misión DRI después de obtener el DDNA.
- Corregida una ruta de venta que podía bloquear el juego, incluida la venta de la última unidad de un objeto.
- Corregidas rutas relacionadas de intercambio de objetos, retirada de equipo y recompensas de cartas afectadas por el mismo problema de acceso al inventario.
- Se mantienen los requisitos originales para aceptar las misiones DRI. El parche no borra objetos duplicados ni repara automáticamente estados de misión ya dañados.

## Árboles evolutivos para los ocho rookies

El reparto actual contiene **103 especies evolutivas distintas y 109 asignaciones entre los ocho árboles**. Estas cifras describen el conjunto actual; no son 103 Digimon nuevos añadidos en esta actualización.

- **Agumon:** árbol ampliado y reorganizado alrededor de WarGreymon, BK WarGreymon, Cannondramon, Machinedramon y KingEtemon.
- **Renamon:** conserva Sakuyamon e incorpora alternativas hacia Pharaohmon, Rosemon, Gryphonmon, SlashAngemon/GuardiAngemon, Puppetmon y Phoenixmon.
- **Patamon:** ramas angelicales, demoníacas y fantasmales hacia Seraphimon, Valkyrimon, BK Seraphimon → Creepymon, MaloMyotismon, VenomMyotismon, Beelzemon y Piedmon. Beelzemon queda exclusivamente en la rama de SkullSatamon.
- **Guilmon:** conserva Gallantmon y añade las ramas de Boltmon, Ghoulmon y Diaboromon → Armageddemon.
- **Kotemon:** ramas de espadachines y caballeros hacia Zanbamon/Fujinmon, una rama mecánica hacia HiAndromon y Kabuterimon → Okuwamon → H-Kabuterimon.
- **Monmon:** ramas hacia Suijinmon, MetalEtemon y MetalMamemon → MegaGargomon → BK MegaGargomon.
- **Bearmon:** conserva Grizzmon → GrapLeomon → Marsmon; añade Thundermon → Datamon → Raijinmon, Frigimon → Mammothmon → SkullMammothmon o MetalGarurumon, y Grizzmon → Monzaemon → Vikemon.
- **Veemon:** conserva su progresión hasta Imperialdramon Paladin Mode y añade Seadramon → MegaSeadramon → MetalSeadramon y Shellmon → Scorpiomon → Pukumon.

Las rutas combinan relaciones de la franquicia y adaptaciones de Harmony a los modelos disponibles. **Super/Special** identifica un acceso avanzado dentro del mod, no una nueva etapa oficial de Digimon.

## Special compartidos y requisitos

- **Omnimon:** combina el progreso de WarGreymon en Agumon y MetalGarurumon en Bearmon; disponible para ambos rookies.
- **Raidenmon:** combina Fujinmon en Kotemon, Suijinmon en Monmon y Raijinmon en Bearmon; disponible para esos tres rookies.
- **Apocalymon** —Apokarimon en PAL—: combina Puppetmon en Renamon, Machinedramon en Agumon, Piedmon en Patamon y MetalSeadramon en Veemon; disponible para esos cuatro rookies.
- Estos desbloqueos exigen los niveles DV y requisitos adicionales correspondientes; no basta únicamente con haber aprendido los componentes. No consumen las formas y no requieren llevar a todos los compañeros en el equipo activo.
- Son las únicas excepciones intencionales al reparto de especies entre rookies. Se conservan duplicados históricos en partidas antiguas, pero no sustituyen componentes del propietario requerido.
- Requisitos revisados con nivel del rookie, dominio DV, estadísticas base, carisma y resistencias según la forma. El equipo y los bonos de digievolución no sustituyen los requisitos de estadísticas base.
- Eliminadas dependencias imposibles en las rutas revisadas; Paladin puede reconocer el dominio de Omnimon en Agumon o Bearmon.

## DigiLab y presentación

- Reorganizadas las bifurcaciones para compartir nodos sin repetir la misma forma dentro del árbol.
- Corregida la superposición de texturas y paletas que dañaba retratos, incluidos Diaboromon, Beelzemon, Myotismon y Devimon.
- Actualizados los árboles, requisitos y catálogo de Digimon disponibles para futuras ramas.

## Balance de formas, técnicas y PM

- Revisados los bonos de estadísticas y resistencias por etapa para que los Special mejoren respecto a sus precursores.
- Omnimon, Fighter Mode, Creepymon, Armageddemon, Raidenmon y BK MegaGargomon reciben **+20% de daño físico/mágico ordinario y −10% de coste de PM**.
- Paladin Mode y Apocalymon reciben **+30% de daño ordinario y −15% de coste de PM**. Se mantienen los límites del juego y las diferencias por elemento y efecto.
- Corregidos 52 perfiles aliados que podían usar un remate de pago como ataque básico gratuito.
- **Omega Blade:** potencia 500 → 900; coste base 280 → 160 PM, equivalente a 136 PM en Paladin sin accesorios. Conserva aprendizaje DV40, precisión, elemento y ventaja de tipo.
- **Fighter Mode:** Sylph Storm sustituye Counter Strike en DV20.
- **Paladin Mode:** Sylph Storm sustituye Erase Magic en DV15; Inferno sustituye Soul Plunder en DV20. Son técnicas propias, sin ocupar una ranura cargada.

## Aprendizaje y EXP DV

- Repertorios completos disponibles como máximo en DV40 para Champion, DV45 para Ultimate, DV50 para Mega, DV35 para Super/Special y DV40 para Special final.
- Los remates Special dejan de exigir DV99: los seis Super/Special los aprenden en DV35; Paladin y Apocalymon, en DV40.
- Revisado el dominio de técnicas regulares para cargarlas en otras formas. Los remates exclusivos siguen siendo exclusivos.
- Curvas de EXP DV unificadas por etapa entre formas originales y añadidas, con incrementos graduales cada diez niveles en lugar del salto brusco de la curva anterior.
- Conservados los multiplicadores globales de EXP, Share EXP y los objetos de experiencia. Share EXP sigue siendo EXP del rookie; no reparte EXP DV a las formas de compañeros pasivos.

## Jefes tardíos

- Ajustados únicamente los PV de **17 encuentros seleccionados**: +15% para determinados jefes Black, +20% para sus versiones superiores y equipos de desafío, y +25% para el equipo tardío Datamon/Bulbmon/Armageddemon.
- Conservadas debilidades, resistencias, daño, velocidad, IA y recompensas.
- Sin cambios en combates iniciales, tutoriales, DRI y encuentros con mecánicas de historia excluidos del ajuste. No hay escalado automático según la forma del jugador.

## Actualización de partidas y estado de la beta

- Aplicar el BPS a la **imagen PAL original sin modificar**, no encima de Beta 1.0. Reiniciar desde el arranque y cargar desde tarjeta de memoria, sin reutilizar savestates anteriores.
- Respaldar la tarjeta antes de actualizar. Se conservan las formas aprendidas; la migración de EXP DV mantiene el nivel y la fracción de progreso, aunque cambia el total numérico de EXP a la nueva escala. No se recomienda volver a versiones anteriores con una partida ya convertida.
- Las técnicas sustituidas de Fighter/Paladin se adaptan al cargar la tarjeta, conservando nivel, EXP y banderas de dominio/carga.
- El bloqueo reportado al subir de nivel de Agumon **no se ha reproducido ni se declara resuelto**. La entrega DRI y la progresión de Etemon en partidas previamente afectadas necesitan confirmación con esas partidas.
- Se han realizado pruebas automáticas de ejecución, aprendizaje, guardado, empaquetado y balance controlado. Sigue pendiente una campaña completa y la comprobación visual de todas las formas en DuckStation.

El entrenamiento sin RNG, los 15 objetos adicionales, las mejoras de carga/guardado, la memoria de menús, el analizador, las sombras semitransparentes y el logo Harmony **ya estaban en Beta 1.0 corregida**; se conservan, pero no se presentan como novedades de Beta 1.5.

**SHA-256 del BPS r48:** `80e32238105442ebc80795553cee150a53084e835eb1d7d7654eb5c93cb33f5c`.
