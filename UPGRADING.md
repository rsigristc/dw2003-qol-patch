# Updating from Harmony Beta 1.0 to Beta 1.5

Beta 1.5 is build **r48**. The comparison baseline is the corrected Beta 1.0 download (**r31**, October 10), not the initial download that accidentally contained r15. Both older downloads must be replaced using the same procedure below.

## English

1. **Save in-game to a memory card**, then close the emulator. Back up the entire memory-card file and keep the backup separate. A save state is not a substitute for a memory-card save.
2. Download **`dw2003-harmony-beta1.5.bps`** from the [Beta 1.5 release](https://github.com/rsigristc/dw2003-qol-patch/releases/tag/harmony-beta1.5).
3. Apply this cumulative BPS to your **original, unmodified European/PAL BIN (SLES-03936)**. Do not apply it over Beta 1.0, another mod, a CUE file, or a compressed disc image. The North American Digimon World 3 release is not supported.
4. Keep checksum verification enabled in your BPS patcher. Save the result as a new BIN. See [README.md](README.md#how-to-patch) for patching details and source/output hashes.
5. Copy your original CUE and change only its `FILE` entry to the new BIN filename, preserving all track definitions. Open the new CUE in your emulator.
6. **Boot from the beginning**, with automatic save-state resume disabled. Load your existing in-game memory-card save. Do not load a Beta 1.0 save state: it can restore old code and bypass the update.
7. If no saves appear, check that your emulator is using the same memory-card file as before. A different game filename or per-game card setting may select a different card. Do not format or overwrite your old card.
8. Check your party and save to a separate slot, then restart and verify that the new save loads. Keep your original backup.

### What happens to an existing save?

- Previously learned forms remain available, including historical duplicates. New evolution requirements do not remove learned forms.
- DV EXP is converted per form when it next receives DV EXP. The conversion preserves its DV level and fractional progress; the displayed accumulated EXP may change because the scale changed.
- Fighter and Paladin's replaced own-form techniques migrate when loading the memory card, preserving DV level, EXP, and mastery/loaded flags. Empty slots still follow normal learning.
- Forms already above an updated technique-learning threshold receive pending techniques through the normal results sequence on their next DV level-up.
- No new game is required solely to install this update. Existing duplicate key items or damaged quest states are **not automatically repaired**.
- Keep converted saves with Beta 1.5 or a compatible later build. To return to Beta 1.0, use the untouched backup rather than a save already converted by Beta 1.5.

### Beta limitations and feedback

The previously reported Agumon level-up freeze has not been reproduced and is not claimed fixed. A complete campaign and visual testing of every form remain pending. Report issues with the build (**Beta 1.5 / r48**), emulator/version, language, party/starter pack, and reproduction steps through [GitHub Issues](https://github.com/rsigristc/dw2003-qol-patch/issues).

## Español

1. **Guarda dentro del juego en la tarjeta de memoria** y cierra el emulador. Respalda el archivo completo de la tarjeta y conserva esa copia por separado. Un savestate no sustituye una partida guardada en tarjeta.
2. Descarga **`dw2003-harmony-beta1.5.bps`** de la [release de Beta 1.5](https://github.com/rsigristc/dw2003-qol-patch/releases/tag/harmony-beta1.5).
3. Aplica el BPS acumulativo a tu **BIN europeo/PAL original sin modificar (SLES-03936)**. No lo apliques encima de Beta 1.0, otro mod, un CUE o una imagen comprimida. No funciona con Digimon World 3 norteamericano.
4. Mantén activada la verificación de checksums y guarda el resultado en un BIN nuevo. Consulta [README.md](README.md#how-to-patch) para ver los hashes y las instrucciones de parcheo.
5. Copia el CUE original y modifica únicamente su entrada `FILE` para apuntar al BIN nuevo, conservando las definiciones de pistas. Abre ese CUE en el emulador.
6. **Arranca desde el inicio**, desactivando la reanudación automática por savestate. Carga tu partida desde la tarjeta. No uses estados rápidos de Beta 1.0: pueden restaurar código antiguo y anular la actualización.
7. Si no aparecen tus partidas, comprueba que el emulador use el mismo archivo de tarjeta que antes. Cambiar el nombre de la imagen o usar tarjetas por juego puede seleccionar otra tarjeta. No formatees ni sobrescribas la anterior.
8. Revisa el equipo, guarda en otro espacio y reinicia para verificar la carga. Conserva el respaldo original.

Las formas aprendidas se conservan. La EXP DV se convierte cuando cada forma recibe EXP DV, manteniendo nivel y fracción de progreso; su total numérico puede cambiar. Las técnicas sustituidas de Fighter/Paladin se adaptan al cargar la tarjeta. Las técnicas pendientes por los nuevos umbrales se aprenden mediante la secuencia normal al siguiente nivel DV.

No hace falta empezar una partida nueva sólo para actualizar. El parche no repara automáticamente misiones dañadas ni elimina objetos clave duplicados. Para volver a Beta 1.0 utiliza el respaldo anterior, no una partida ya convertida.

El bloqueo reportado al subir de nivel de Agumon sigue sin reproducirse y no se declara corregido. Las pruebas de campaña completa y de todas las formas siguen pendientes. Incluye **Beta 1.5 / r48**, versión del emulador, idioma, equipo/paquete inicial y pasos de reproducción al reportar un problema.
