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
