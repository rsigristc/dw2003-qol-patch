# Changelog

## October 16, 2026 — Beta 1.5 (r48)

**Cumulative changes since the corrected Beta 1.0 download, r31, released on October 10.** Beta 1.5 identifies `dw2003-harmony-beta1.5.bps`.

This update expands all eight Rookie evolution trees, rebalances evolution and technique progression, strengthens Special forms, and fixes inventory and shop regressions reported in Beta 1.0.

### Inventory, quests, and shops

- Fix contradictory item checks that could treat an item as both present and absent. This could select incompatible NPC/dialogue states, repeat key-item rewards, or return a DRI conversation to its initial quest branch after obtaining DDNA.
- Fix an inventory bridge that could freeze the game when selling items, including the last unit of an item.
- Fix related item-exchange, equipment-removal, and card-reward paths affected by the same inventory access issue.
- Preserve original DRI quest acceptance requirements. Already duplicated items and damaged quest states are not automatically repaired.

### Evolution trees for all eight Rookies

The current trees cover **103 distinct evolution species and 109 assignments across eight Rookies**. These are totals for the current roster, not 103 newly added Digimon.

- **Agumon:** expand and reorganize branches around WarGreymon, BK WarGreymon, Cannondramon, Machinedramon, and KingEtemon.
- **Renamon:** retain Sakuyamon and add alternatives ending in Pharaohmon, Rosemon, Gryphonmon, SlashAngemon/GuardiAngemon, Puppetmon, and Phoenixmon.
- **Patamon:** angelic, demonic, and ghost branches ending in Seraphimon, Valkyrimon, BK Seraphimon → Creepymon, MaloMyotismon, VenomMyotismon, Beelzemon, and Piedmon. Beelzemon is exclusive to the SkullSatamon branch.
- **Guilmon:** retain Gallantmon and add Boltmon, Ghoulmon, and Diaboromon → Armageddemon branches.
- **Kotemon:** swordsman/knight routes toward Zanbamon and Fujinmon, a mechanical route toward HiAndromon, and Kabuterimon → Okuwamon → H-Kabuterimon.
- **Monmon:** routes toward Suijinmon, MetalEtemon, and MetalMamemon → MegaGargomon → BK MegaGargomon.
- **Bearmon:** retain Grizzmon → GrapLeomon → Marsmon; add Thundermon → Datamon → Raijinmon, Frigimon → Mammothmon → SkullMammothmon or MetalGarurumon, and Grizzmon → Monzaemon → Vikemon.
- **Veemon:** retain the main progression through Imperialdramon Paladin Mode and add Seadramon → MegaSeadramon → MetalSeadramon and Shellmon → Scorpiomon → Pukumon.

Routes combine franchise relationships with Harmony adaptations to available models. **Super/Special** describes advanced access within Harmony, not a new official Digimon stage.

### Shared Specials and unlock requirements

- **Omnimon:** combines WarGreymon progress on Agumon with MetalGarurumon progress on Bearmon; available to both Rookies.
- **Raidenmon:** combines Fujinmon on Kotemon, Suijinmon on Monmon, and Raijinmon on Bearmon; available to those three Rookies.
- **Apocalymon** —Apokarimon in PAL—: combines Puppetmon on Renamon, Machinedramon on Agumon, Piedmon on Patamon, and MetalSeadramon on Veemon; available to those four Rookies.
- Shared unlocks require the applicable DV mastery and additional requirements, not just learning the component forms. Components are not consumed, and all owners need not be in the active party.
- These are the only intentional shared species in the new allocation. Historical duplicates in older saves are preserved but do not replace components on the required owner.
- Rebalance requirements using Rookie level, DV mastery, base stats, charisma, and resistances as appropriate. Equipment and evolution bonuses do not satisfy base-stat requirements.
- Check revised routes for unreachable dependencies. Paladin can recognize Omnimon mastery on either Agumon or Bearmon.

### DigiLab and presentation

- Consolidate branching routes so shared ancestors appear once within each tree.
- Fix texture/palette overlap affecting portraits, including Diaboromon, Beelzemon, Myotismon, and Devimon.
- Update evolution requirements and the remaining available-Digimon catalogue.

### Form strength, techniques, and MP

- Rebalance form stat bonuses and resistances by stage so Specials improve on their precursors.
- Give Omnimon, Fighter Mode, Creepymon, Armageddemon, Raidenmon, and BK MegaGargomon **+20% ordinary physical/magic damage and −10% MP cost**.
- Give Paladin Mode and Apocalymon **+30% ordinary damage and −15% MP cost**, preserving game caps and elemental/effect differences.
- Correct 52 ally profiles that could use a paid finisher as a free basic attack.
- **Omega Blade:** power 500 → 900; base MP cost 280 → 160, or 136 MP on Paladin without accessories. Retain DV40 learning, accuracy, element, and type advantage.
- **Fighter Mode:** learn Sylph Storm instead of Counter Strike at DV20.
- **Paladin Mode:** learn Sylph Storm instead of Erase Magic at DV15, and Inferno instead of Soul Plunder at DV20. These are own-form techniques and do not occupy a loaded-skill slot.

### Technique learning and DV EXP

- Make full repertoires available by DV40 for Champion, DV45 for Ultimate, DV50 for Mega, DV35 for Super/Special, and DV40 for final Special forms.
- Remove the DV99 wait for Special finishers: the six Super/Special finishers are learned at DV35; Paladin and Apocalymon finishers at DV40.
- Rebalance mastery levels for loading regular techniques. Exclusive finishers remain exclusive.
- Use consistent DV EXP curves within each stage for original and added forms, with gradual increases every ten DV levels instead of the previous abrupt jump.
- Preserve existing global EXP multipliers, Share EXP, and experience items. Share EXP remains Rookie EXP; it does not award DV EXP to passive party members' forms.

### Late-game bosses

- Increase only HP in **17 selected encounters**: +15% for selected Black bosses, +20% for their higher-level variants and challenge teams, and +25% for the late Datamon/Bulbmon/Armageddemon team.
- Preserve weaknesses, resistances, damage, speed, AI, and rewards.
- Leave early encounters, tutorials, DRI fights, and excluded story-mechanic encounters unchanged. Bosses do not automatically scale to the player's form.

### Updating and beta status

- Apply the BPS to the **original unmodified PAL image**, not to a Beta 1.0 image. Restart from boot and load a memory-card save; do not reuse older save states.
- Back up memory cards. Previously learned forms are retained. DV EXP migration preserves level and fractional progress while converting accumulated EXP to the new scale. Returning a converted save to an older build is not recommended.
- Replaced Fighter/Paladin skills migrate when loading a memory card, preserving level, EXP, and mastery/loaded flags.
- The reported Agumon level-up freeze **has not been reproduced and is not claimed fixed**. DRI hand-ins and Etemon progression in previously affected saves still need confirmation with those saves.
- Automated execution, learning, save, packaging, and controlled combat checks have been performed. A complete DuckStation campaign and visual checks for every form remain pending.

RNG-free training, the 15 additional items, loading/saving improvements, battle-menu memory, the analyzer, translucent shadows, and the Harmony logo were **already included in corrected Beta 1.0**. They are retained, not newly introduced in Beta 1.5.

- Technical build: **r48**.
- BPS file: `dw2003-harmony-beta1.5.bps`.
- BPS SHA-256: `80e32238105442ebc80795553cee150a53084e835eb1d7d7654eb5c93cb33f5c`.

## October 10, 2026 — Beta v1.0 download corrected to r31

The initial Harmony Beta v1.0 download accidentally contained the older r15 build. It has been replaced with **dw2003-harmony-r31-20261009**, keeping the download name **dw2003-harmony-betav1.bps**. If you downloaded the initial release, download the patch again and apply it to your original unmodified PAL BIN, not to the previously patched image.

This cumulative r31 build includes the r29 training improvements and the clean title logo. It also moves the language-selection logo panel up 20 pixels so Harmony fits inside the 224-line gameplay display area. Visual testing in DuckStation remains pending according to the supplied build notes.

Restart from boot and load a memory-card save; do not use save states from earlier builds. Back up memory cards before changing builds.

- BPS SHA-256: `b71731332a72ed2a9da1b3c00aeb267d9cdeef76d6040b76981fbd5a3d141343`.
- BPS size: **3,438,321 bytes**.
- Patched BIN SHA-256: `ffa0feaf7de575afc8295760f54af4846c767cfcabf196feae919c1609e3135d`.

The patch is renamed without changing its bytes. The matching r31 manifest replaces the r15 manifest; the obsolete r15 draft recipe is removed.

## Second Beta v1.0 — Digimon World 2003: Harmony

The project is now **Digimon World 2003: Harmony**. Work continues to make the game more enjoyable and approachable for everyone, with training without RNG, faster loading and saving, new items, improved systems, and fixes from the previous beta.

### Training rebuilt

- Remove RNG from training results. Base stat gains are guaranteed even if you fail the minigame.
- Stop the cursor in the green zone in the new timing minigame for extra stat bonuses.
- Fast Training skips the minigame and grants base gains without the additional bonus.
- Training descriptions explain how each stat helps your Digimon.

### Menus, loading, and saving

- Improve loading and transitions when entering and leaving menus.
- Saving/loading reductions from around 15–20 seconds to under 5 seconds have been reported. Results vary by setup; timing measurement in DuckStation remains pending for this r15 build.
- Remove redundant location screens after battles, after leaving the save menu, and when returning from the full Start menu to the same map. Preserve labels when changing maps.
- Start-menu saves display the correct location instead of Asuka Inn.
- Battle menus remember previous selections, including Techniques instead of resetting to Attack.
- Fix the map glitch when pressing Square during exploration.

### Digivolutions and battles

- Add the first experimental custom Digivolution line for Agumon, with battle camera scenes and 3D battle portraits. Development continues; stats and abilities may contain inconsistencies.
- Add a DigiLab Digivolution routes interface showing requirements.
- Display the active Digivolution name in battle instead of the Rookie name.
- Customize technique order per Digimon/Digivolution: open Techniques in battle, press Select, move with Up/Down or L1/R1, and confirm with X or Select.
- Fix Picking Claw and Snapping Claw when an enemy is KO'd and improve their descriptions.
- Display actual technique power values.
- Show a Share EXP activation notification after defeating Leader Seiryu.

### New items

All 15 test items cost **1 BIT** at the initial Gargomon shop and the first item shop. English names below are descriptive translations.

- **Lure Disk:** encounters ×1.25 for 300 steps.
- **Frenzy Disk:** encounters ×3 for 300 steps.
- **Repellent Disk:** encounters ×0.5 for 300 steps.
- **Stealth Disk:** no random encounters for 300 steps.
- **Lure Ring:** encounters ×1.25 while equipped.
- **Repellent Ring:** encounters ×0.5 while equipped.
- **DV Adapter:** +20% DV EXP for the form used in battle.
- **Apprentice Ring:** +15% Share EXP for the wearer; does not stack with EXP Adapter.
- **Analysis Disk:** reveal enemy resistances and stealable-item availability for 5 battles. Analysis becomes permanent after defeating Byakko. L1/R1 changes pages; Select shows/hides analysis from main battle commands.
- **Reserve Ring:** restore 10% of maximum MP after winning a battle.
- **Risk Ring:** +15% damage dealt and received.
- **Tenacity Ring:** survive a lethal hit with 1 HP once per battle, provided HP was above 50% before the hit.
- **Three MP recovery consumables:** restore 25%, 50%, or 100% of maximum MP in exploration or battle.
- Notify when encounter effects expire and when battle item bonuses apply.

### Visuals and fixes

- Restore light-blue borders for Flawe's walkthrough and the exploration Quest Log.
- Make shadows transparent instead of solid black circles.
- Correct battle reward text from “1IT”/“1EXP” to “BIT”/“EXP”.

### Languages and compatibility

All changes cover English, Spanish, French, German, and Italian. Gameplay testing has only been carried out in English and Spanish. Added text in other languages uses a text translation tool and may contain wording, spelling, or grammatical errors.

Apply `dw2003-harmony-betav1.bps` directly to the original unmodified PAL BIN. This is the supplied October 9 r31 cumulative build, renamed without changing the patch bytes. Its matching manifest records provenance and hashes.

Back up memory cards. Restart from boot; use memory-card saves instead of older save states. KIT2 saves migrate to KIT3 on loading and saving. KIT3 saves require r15 or later; physical memory-card file size is unchanged. Full emulator playthrough and visual validation remain pending. Automated checks do not establish bug-free gameplay.

### Next Steps

Rework Intelligence/Wisdom-focused Digimon and techniques, supported by the newly implemented MP recovery disks and MP recovery ring. Develop custom Digivolution lines for the remaining Rookies and further rebalance Digivolution stats and techniques to make more team compositions and playstyles rewarding.

### Related projects

Harmony complements the [DS Companion for Android](https://github.com/rsigristc/DW3-DS-Android). See the [first beta announcement](https://www.reddit.com/r/DigimonWorld/comments/1wzc6e0/digimon_world_2003_qol_new_systems_mod_for_psx/) for the original feature overview.

Bug reports, balance feedback, and translation corrections are welcome through [GitHub Issues](https://github.com/rsigristc/dw2003-qol-patch/issues). Include patch version, language, emulator/hardware, reproduction steps, and whether you started a new game or loaded a save.

## 2026-10-06 — GPU depth fix build

- Publish the supplied `dw2003-flawe-quest-walkthrough-gpu-depth-fix-20261006.bps` without rebuilding or altering it.
- Preserve its manifest and draft recipe alongside the patch.
- Document the combined quality of life features, controls, original-image requirements, and expected output hashes.
- Add contributor attribution, upstream MIT notices, original-game rights acknowledgments, patch-only instructions, known upstream limitations, and optional Ko-fi support.

The build name identifies the quest/walkthrough GPU depth fix revision. This distribution step does not claim new gameplay fixes or a complete playthrough validation.
