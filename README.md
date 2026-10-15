[README.txt](https://github.com/user-attachments/files/33473541/README.txt)
# Silver the Hedgehog + Telekinesis for Vampire Survivors

Silver the Hedgehog joins the survivors! Dominate your enemies with his unique
psychic abilities! Grab enemies and swing them around, and stand still to release them!
This version includes a powerful Evolution when leveled up to 8 with Spinach or Tome!
Psychic Control allows you to directly control the sphere with your mouse!
Fling it around anywhere, and the right mouse button to release it into crowds
of enemies!

**Fan work, not affiliated.** Silver the Hedgehog is SEGA's character (Sonic
the Hedgehog 2006). All sprites and sounds here are original fan-made
placeholders. Vampire Survivors belongs to poncle. Built with AI assistance;
every release was play-tested in-game before publishing.

## What it does

- **Silver kit** (applies to the character you pick): +15% Duration to start,
  +5% more at levels 5/10/15/20/25, +20% Growth, +20% Luck, 0.9x move speed,
  +10% Might. Fan sprite set with hover-bob visuals.
- **Silver select slot**: Silver also appears as his own card on the
  character selection screen (always available, Antonio-based stats plus
  the kit above, Silver portrait).
- **Telekinesis** (innate, active from run start, levels 1-8 through its own
  level-up cards): grabs nearby enemies and carries them as a burning orb
  that hurts what it touches. Click to hurl captives toward your cursor;
  standing still releases early; at higher levels it holds up to 4 (+Amount).
  Captives take no damage while held, can't hurt Silver, and pass straight
  through him on sharp turns. Scales with Might, Area, Amount, Duration
  and Cooldown like a real weapon.
- **Psychic Control** (evolution: Telekinesis 8 + Spinach, Empty Tome or
  Candelabrador): the orb follows your mouse on its own and devours what
  it touches (8 holds + Amount + Magnet rank, up to 100). Right-click hurls
  everything toward the cursor; flung bodies detonate at the screen edge in
  an Area-scaled blast.
- **Psychic pickup**: anything on screen Silver is allowed to take is
  collected automatically — gems, coins, hearts, food, magnets, chests,
  relics. Deliberately walk-over only (and magnet-proof): rosaries, stage
  weapons, NPCs/merchants, coffins, reroll/skip/banish tokens.
- Grip ring, green captive bubble, evolved ring skin, edge-blast flash,
  grab/throw/impact sounds (built-in synth, or drop WAVs in `sfx/`).
  Everything tunable in the config file.

## Install (Steam, Windows)

1. Install BepInEx 6 bleeding-edge IL2CPP (`Unity.IL2CPP-win-x64`,
   build 6.0.0-be.788 or newer from builds.bepinex.dev) into your Vampire
   Survivors folder (the one with `VampireSurvivors.exe`). Run the game once
   (first start is slow: it builds compatibility files), then quit.
2. Copy `SilverTelekinesis.dll`, `frames/`, `evo/`, `tk_glow.png`, `tk_hands.png`,
   `tk_orb.png` and `sfx/` into `<game>/BepInEx/plugins/SilverTelekinesis/`.
3. Launch and start any offline/single-player run. Do NOT use in online co-op.

## Tune it

Open `<game>/BepInEx/config/you.silverdtelekinesis.cfg` after the first run:
`[Silver]` for the stat kit, `[Telekinesis]` for ranges/damage/timings
(including evolved capacity), `[TelekinesisFX]` for visuals and volume,
`[SilverVacuum]` for psychic pickup. Edits apply live mid-run.

## Uninstall

Delete `<game>/BepInEx/plugins/SilverTelekinesis/`. Saves are untouched
(the mod never writes to them).

## Credits

- BepInEx, HarmonyX, Il2CppInterop, Cpp2IL, ILSpy teams
- OffTheClockMods/vampiresurvivors-mods and kulmin/VSEvolutionHelperEx for
  the proven BepInEx-6-on-Unity-6 patterns this mod builds on
- poncle for Vampire Survivors; SEGA/Sonic Team for Silver's inspiration
