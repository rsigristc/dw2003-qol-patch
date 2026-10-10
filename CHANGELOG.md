# Changelog

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

Apply `dw2003-harmony-betav1.bps` directly to the original unmodified PAL BIN. This is the supplied October 7 r15 build, renamed without changing the patch bytes. Manifest and draft retain the original internal name for provenance.

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
