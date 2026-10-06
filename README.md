# Digimon World 2003 — Quality of Life Patch
<img width="400" height="117" alt="image" src="https://github.com/user-attachments/assets/49527f33-42cb-4329-b4cb-51d1512a8e5e" />

A community mod compilation for **Digimon World 2003 (Europe / PAL, SLES-03936)**, assembled and extended by **rsigrist**. Includes Flawe's Mod 2.0, guiomatos' Initial Pack Customizer enhancements, markisha64's patches, and additional interface and progression improvements.

**Patch only. Each player must provide their own original, legally obtained copy of the game and dump it themselves. No game image, BIOS, or standalone game assets are provided.** This patch does not work with the North American *Digimon World 3* release.

[Download the release](https://github.com/rsigristc/dw2003-qol-patch/releases/latest) · [Support Rodrigo on Ko-fi](https://ko-fi.com/rodrigosigrist)

## How to patch

1. Back up your original disc dump and memory cards.
2. Download `dw2003-flawe-quest-walkthrough-gpu-depth-fix-20261006.bps` from Releases or the `patches/` folder.
3. Verify your **unmodified European BIN** matches the source below. Apply this complete patch directly to the original BIN, with no earlier mods applied. Do not patch the CUE file, a compressed image, or an already patched BIN.
4. Open [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/), select your original BIN as the ROM file, and the BPS as the patch file. Apply the patch with checksum verification enabled and save the output to a new file. Large disc images may require a desktop BPS-compatible patcher if your browser runs out of memory.
5. Keep your original CUE and update its `FILE` entry to reference the new BIN filename, preserving its track definitions. Load that CUE in your emulator.
6. Boot the game normally. Load a memory-card save instead of a save state made with an earlier build. Start a new game to use the starter team selection and Fast Start features.

If the patcher reports a source mismatch, stop and check the edition, dump format, size, and hash. Do not bypass verification.

### Required original BIN

- Edition: Digimon World 2003 (Europe), SLES-03936.
- Size: **692,146,560 bytes**.
- CRC32: `007df18e`.
- SHA-256: `fb70dc9a995aed628cf515cabc87c7b14e5142559076ec394dfe793ec3e26a04`.

On Windows PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath 'Digimon World 2003 (Europe).bin'
```

### Expected patched BIN

- Size: **693,562,464 bytes**.
- CRC32: `673c4293`.
- SHA-256: `b3aa0b474abbfaea7713d35e69de019a5d16b945c94e651e8d70285a60bda4c4`.
- BPS SHA-256: `d1e844a9eecd02f4e607d1d59bb6ad972e3ac9f44aa1015e5549af71b9735fd6`.

The JSON manifest records build metadata and hashes. The draft JSON records the build recipe; neither JSON file is a patcher input.

## Quality of life changes

### Battle and progression

- Restore partner Digimon HP and MP when leveling up.
- Faster battle text and reduced redundant messages from **Flawe's Mod**.
- Display enemy HP during battle.
- Always display partner MP without opening the Techniques menu.
- Display technique attributes, power, and MP cost. Effective attributes appear blue, ineffective attributes red, and neutral attributes without a color highlight. Insufficient MP appears red.
- Display partner stats and attributes in the battle DV menu, with the strongest resistance in blue and the weakest in red.
- Show EXP required for the next level after each battle, and DV EXP beside Digivolutions.
- Show the active Digivolution's DV EXP beside partner EXP in the status window, and beside Digivolution names.
- Increase global EXP gain to **×1.3** and DV EXP gain to **×1.2**.
- Unlock **Share EXP** after defeating Leader Seiryu. Partners who do not participate receive an additional one-third of the battle's total EXP. EXP Adapter also increases shared EXP. Shared EXP does not grant DV EXP; participation is required for DV EXP.
- **Fixed Field Moves:** correct the element applied by battle field moves.
- **Uncapped Digivolution EXP:** remove the 10/50 DV EXP caps before applying the ×1.2 multiplier, while preserving the level 99 ceiling and accumulated EXP limit.
- **Improved HP Proxy:** reduce damage by 10%/20% instead of a fixed 10/20 points.

### Exploration, guidance, and menus

- **Flawe's Fast Travel** and **In-Game Walkthrough**, accessible through the game menus.
- Extend the walkthrough to all five PAL languages: English, French, Italian, German, and Spanish.
- Show a mission log in the upper-right corner during exploration, summarizing Flawe's walkthrough. Press **Circle** to show or hide it.
- Press **Square** during exploration to open the map for quick access to fast travel. On the map, use **X** to select a destination and exit the menu to travel; **Square** switches server maps.
- NPC bubbles identify available quests, Digimon battles, and card battles.
- Press **L1/R1** during exploration to change the leader Digimon.
- Show notifications when an auction or DRI event becomes available.
- Show Digivolution requirements for each Digimon in the DigiLab.
- Add item bonuses and stats to descriptions in shops and the equipment menu.
- Add a **Save** option to the Start menu using the native memory-card interface. Saving remains subject to gameplay restrictions, such as active events or battles.
- Speed up map transitions and save-menu animations.
- Increase the player name limit from 8 to **10 characters**.

### New game and story flow

- Extend **guiomatos' Initial Pack Customizer** with **Pack D**, allowing a custom starter team while keeping Packs A/B/C. Add a Veemon description and support for the first summon scene reflecting the selected team.
- **Fast Start:** retain player naming and starter pack selection, then begin directly in Asuka, skipping the introduction and initial summon event. Consequently, the custom summon scene is skipped in this combined build.
- Allow postgame content to trigger without epic weapons.
- Make Baronmon/TNT accessible without first visiting Phoenix Bay.
- Make the Admin Center accessible after A.o.A. Ambusher.
- Skip the Folder Bag scene while preserving its progression callback.

### Video timing

- Apply the **NTSC 60 Hz patch** for native video mode and timing. This does **not** mean every scene renders at 60 frames per second.

## Release notes and limitations

This release packages the **October 6, 2026 GPU depth fix** build identified by the supplied manifest. The feature list above documents the intended mod behavior; it is not a claim of exhaustive hardware or emulator playtesting.

- Flawe's walkthrough covers the main story, not side quests or postgame guidance.
- Flawe's upstream notes warn that traveling outside the normal postgame area can leave NPCs absent; entering underground or underwater areas there can crash the game. These routes are not declared fixed by this release.
- Back up memory cards when changing builds. For the first test of Start-menu saving, use a free slot and verify that the save loads after restarting.
- Faster transitions and animations do not eliminate actual disc or memory-card I/O time.
- See [CHANGELOG.md](CHANGELOG.md) and [CREDITS.md](CREDITS.md) for release provenance and attribution.

## Credits and rights

**Flawe**, **guiomatos**, **rsigrist**, and **markisha64 / Marko Grizelj** receive credit for their respective contributions. EmeraldPhoenix is credited for the walkthrough on which Flawe's guide is based. Full attribution and third-party notices are in [CREDITS.md](CREDITS.md) and [LICENSE-NOTICE.md](LICENSE-NOTICE.md).

Digimon and Digimon World 2003 belong to their respective rights holders, including Bandai / Bandai Namco, Akiyoshi Hongo, and Toei Animation. Original game development credits include BEC and Boom Corp. PlayStation belongs to Sony Interactive Entertainment. This is an unofficial fan project with no affiliation, endorsement, or grant of rights to the original game.

## Support

If you enjoy my improvements and integration work, you can [support me on Ko-fi](https://ko-fi.com/rodrigosigrist). Donations are optional to support my work; you won't purchase the game, grant game rights, or imply that upstream authors receive a share.

Report issues through [GitHub Issues](https://github.com/rsigristc/dw2003-qol-patch/issues), including your emulator/version, selected language, reproduction steps, and the patch version. Do not upload disc images, BIOS files, or copyrighted game assets.
