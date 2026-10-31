# Resident Evil 5 — Quality of Life Fixes

Complete list of fixes, restorations, improvements, and optional modifications.

## Contents

- [General Fixes](#general-fixes)
- [Splitscreen Fixes](#splitscreen-fixes)
- [Mouse & Keyboard Fixes](#mouse--keyboard-fixes)
- [Language Fixes](#language-fixes)
- [Modded Game Fixes](#modded-game-fixes)
- [Optional Modification](#optional-modification)


## General Fixes

*A set of fixes that improve the vanilla experience*

- Enemy pathfinding restored. This does **not** have to do with collision issues caused by high framerates.
- Added new inventory management options from the Nintendo Switch version:
  - Give all and Request all will ignore the item's assigned maximum quantity that can be handed over at a time (for example, 30 handgun rounds, 1 egg). The latter is only available while playing with a CPU controlled partner, as it is up to a real player how much they want to give you. If you press the Give button while the inventory is closed, behavior will default to the last picked option, which resets on level load and defaults to the original "Give".
  - Exchange is now permanently available in your partner's inventory, even if you're not full.
  - Combine option now only appears if the item can be combined with something in the first place.
- Inventory icons removed in update 1.2.0 restored:
  - Equipped item highlight.
  - 'E' letter for "Equipped" item indicator.
  - Infinite ammo indicator.
- Added new Shadow Quality settings. LOW, MEDIUM and HIGH have now become OFF, LOWEST and LOW respectively. In order, the shadow map resolutions are: Disabled, 512, 1024, 2048, 3072, 4096.
- Aim quickturns now display correctly online at framerates other than 30fps.
- Fixed session list softlock caused by attempting to join a lobby and getting an error message.
- Spamming character switching in Mercenaries and Versus lobbies by holding down both triggers is no longer possible, which now matches the original console patch behavior and should help prevent excessive online updates and potential desync in lobbies.
- New 1.2.0 Mercenaries and Versus "The other player is not ready" displays "Back" button and text regardless of host or client. This visual bug no longer displays if you are not the host.
- Incorrect in-game inventory name position fixed. See InventoryNameType under Optional Modifications for more information.
- No Mercy added to Mercenaries Reunion based on Mercenaries United including its scoring system. Saving high scores is not possible in this version and it is unknown whether this will change in the future.
- No Mercy character selection screen now correctly displays No Mercy ranks, instead of solo ranks.
- Joining a Duo Mercenaries lobby through invites while in the No Mercy menus will no longer cause No Mercy to remain active, which would cause a desync.
- Misplaced controller prompt position in Versus result screen fixed (bug introduced in 1.2.0 update).
- Reworked Options menu:
  - Fixed menu transition animations.
  - Fixed vertical coordinates to match transition animations.
  - Replaced "Default" option with "Reset to default" shortcut.
- "Overall quality" setting partially fixed. Some parameters like LOD are now properly set based on Games for Windows Live version, but a lot of code is still missing.
- Fixed missing DLC voicelines for Chris, Sheva and Jill. While this mainly affects modded gameplay, you will now for instance hear Chris or Sheva shout "Josh!" when he dies in the main campaign. Refer to Optional Modifications section to disable it.
- Jill (and any other right handed female character) now has a more appropriate reload animation for the S&W M29. Refer to Optional Modifications section to disable it.
- Expanded special character support for Steam usernames. Unsupported characters should now display a white square ('□') instead of garbled text.
- Fixed softlocks caused by attempting to discard an empty item slot. Two ways of triggering it were:
  - Fire a non-infinite rocket launcher and buffer a discard command before it disappears.
  - Reload a weapon and buffer a discard command on its ammo before it disappears.
- Title screen prompt can now freely switch between "Press any key" and "Press start" like in pre-1.2.0 versions.
- Transition animation (jumbled letters) from Difficulty Select into Network Settings now waits for action assist prompt when Amateur is selected.
- Buggy region lock behavior fixed.
- The game no longer shows your own Steam profile when you attempt to bring up your partner's in a Mercenaries lobby as the client (2P).
- Removed LAN option as it originally relied on Games for Windows Live code and doesn't work on Steam (will be reinstated if fixed).
- Removed Match Type concept from Versus, as it was more of an Xbox/Games for Windows Live version leftover.
- Fixed multiple issues regarding Lost in Nightmares and Desperate Escape menus.
- Fixed character scale (size) for Josh, Barry and Rebecca (originally fixed by maluc).
- Removed Black Outlines around objects and characters when Shadows and Anti-Aliasing were engaged at the same time.
- Ported a corrected version of the vertically expanded Title Screen from the Games for Windows Live version (visible at narrower aspect ratios, like 4:3), and restored blood cell animations missing from every later re-release.
- Semi-transparent black background while reading documents now scales properly at narrower aspect ratios in Lost in Nightmares.
- Fixed player profile manager behavior, which fixes issues such as not being able to trade weapons with a CPU controlled partner.
- First time DLC availability notifications now account for DLC unlock criteria being already met or not, and also added missing Extra Figures notification.
- All characters are now able to perform most melee attacks when controlled by the CPU. While this mainly affects modded gameplay, Chris would originally refuse to perform the follow up Haymaker on enemies such as Gatling Gun Majini and Giant Majini.
- Privacy Policy Yes/No prompt style now matches those seen throughout the rest of the game.
- M93R handgun no longer gives off the impression of piercing through enemies when in reality it does not (effect originally visible on walls and floor).
- The reaper will no longer dramatically overshoot some of its vertical jumps.
- Splitscreen button prompts no longer appear in Item Management screen after attempting to start a Lost in Nightmares or Desperate Escape splitscreen session and backing out into the main menu.
- BSAA Jill's holstered handgun now properly appears and disappears as you equip a handgun in Mercenaries as well (partially thanks to Henry).
- Low poly Rocket Launcher model no longer appears partially invisible.
- Breakable score star hitboxes fixed (originally fixed by Syndeh).
- Changed minimum resolution from 800x600 to 640x360. **WARNING**: Specific cutscenes may crash at specific points with an "Unsupported function" error message. 1024x576 should be the lowest, crash-free widescreen (16:9) option. The game is still fully playable if said cutscenes are skipped before the troublesome shots happen. The known examples are: "Medicine" and "A Message from Jill", as well as the Desperate Escape equivalent of the latter.

## Splitscreen Fixes


*A set of fixes aimed at improving the splitscreen play experience*

- Item prioritization setting and input method are now properly respected when giving items in the Item Management screen.
- Controller vibration intensity now works correctly regardless of input method combination in splitscreen mode.
- In-game prompt sizes no longer reduced for Chinese in splitscreen mode.
- Player 2's username will now always display as "Guest" in Mercenaries lobby, instead of appearing blank under certain input method combinations.
- Player 2 now correctly rejoins as Heavy Metal Chris in Mercenaries Reunion, rather than Excella.
- Added temporary bandaid fix for "Save successful." screen softlock (keyboard should always allow you to proceed to the main menu now).
- Motion blur now works in splitscreen mode (and other unused camera modes) if enabled under System Settings, making this the only version of the game to support it.
- 1-1 controls tutorial file now displays correctly for each player while using mixed input methods.

## Mouse & Keyboard Fixes


*A set of tweaks and additional settings to further customize the Mouse & Keyboard controls*

- Added new Keyboard/Mouse Settings.
  - Movement Type:
    - Type A = Turn character with mouse, strafe with A & D keys.
    - Type B = Turn character with A & D keys (tank controls). Camera controls subject to change.
  - Aiming Type:
    - Default = Aim with the camera, character follows with a delay.
    - Classic = Aim by controlling the character's arms directly. Camera follows with a delay, with deadzone in the middle (forces laser sight).
    - Cursor aiming = Reticle moves freely across the screen, visible at all times (forces tank controls and crosshair).
  - Aiming Reticle:
    - Default = Crosshairs.
    - Classic = Laser sight (includes laser angle fix).
  - Separate camera and aiming mouse sensitivity values.
  - Alternate QTE binding preset (Aim + Fire).
- Menus can now be navigated using WASD keys.
- Contextual action key binding now acts as move item shortcut in inventory.
- Mousewheel to switch characters now also works in Versus lobbies.
- Binding to toggle between High Score/Highest Rank and Enemies Routed/Max Combo in Stage Select menu changed from Z back to Left Shift to match vanilla Leaderboards equivalent, as well as our previous patch.
- Added and fixed mouse support in numerous menus.
- Mouse camera movement enabled in Versus and Mercenaries Intro and Outro for strafing controls.
- Restored and added numerical inventory layout support for multiple game modes. Must manually set Item Prioritization to Numerical under Keyboard/Mouse Settings for it to work. Disabled while playing with non-patch users outside of Survivors and Team Survivors modes, due to compatibility reasons.
- Menu navigation controls no longer become partially unresponsive in an online Mercenaries lobby after playing a full match as the client (2P).
- Fixed some instances of menu navigation controls legend showing keyboard preset while using a controller ("(B)Back", instead of "(LS)Select (A)OK (B)Back").
- Versus lobby key bindings rearranged to more closely match original menus.
- Home key is now a valid key binding, as it's no longer used to bring up the Games for Windows Live interface.
- Lost in Nightmares fixed camera easter egg is now fully playable with mouse and keyboard.

## Language Fixes


*A set of fixes aimed at improving localization support*

- Minor typos fixed in English and Spanish.
- Implemented Russian DLC translation by INSERTHERE and general improvements made by Infernal.
- Some in-game text is no longer hardcoded, which allows for certain language-specific fixes:
  - "Chris Redfield" and "Sheva Alomar" in Costume Select.
  - "Chris Redfield", "Josh Stone" and "Jill Valentine" in Lost in Nightmares and Desperate Escape session lists and Leaderboards.
  - Character names in the inventory.
- Russian no longer uses the cyrillic alphabet for ranking systems, as requested by multiple members of the community.
- Chapter select divider texture no longer missing for slavic languages.
- Slavic character select menu text restored in original Mercenaries and Versus.
- Chapter 2-1 tutorial no longer displays Russian character names over English ones.
- Spanish "Your partner died" screen is no longer missing the letter that determines gender.
- The 'X' key icon to bring up your partner's inventory is no longer missing in Spanish.
- Certain Russian HUD names no longer display in English (textures provided by Syndeh).

## Modded Game Fixes

*A set of fixes that improve the experience while using mods*

- Stun rod nerf from Mercenaries Reunion now also applies to the original Mercenaries as well as Versus.
- Blobs/Guardians of Insanity will now blow up upon death if inserted into Versus, Desperate Escape or either Mercenaries mode (via modding).
- Timings for breaking time bonuses as originally unintended characters fixed (Wesker in Mercenaries Reunion/United being a notable example).
- Certain weapons should now be usable (but not always flawless) by any character: Longbow, Gatling gun, Lantern and Flamethrower.
- Partially removed a restriction that prevented CPU controlled characters to finish off bosses and sub-bosses (Mercenaries and Versus only).
- Removed restrictions that prevented trading Px4 and knives in-game.
- Fixed weapon request voice lines for Barry's Samurai Edge as well as all knives.
- Some items' icons have been fixed in the Item Management screen, with some of them being rearranged, such as the Px4, Samurai Edge pistols and unused Emerald Beetle.
- Emerald Beetle now sells for ₦2500, instead of 9.
- While using certain cranks in Lost in Nightmares, characters will now correctly call out their actual partner's name.
- Some animations are now correctly oriented regardless of gender and dominant hand, such as using cranks and levers.
- Weapon animation fixes:
  - All right handed women now have access to Rebecca's reload animation for the Jail Breaker.
  - Knives (excluding Jill's), Px4 and Samurai Edge handguns all use the correct animation sets for the opposite genders.
- Replacing Chris with a different character in Lost in Nightmares no longer softlocks the piano sequence when controlled by the CPU.
- Casual walk animation in chapter 1-1 now works regardless of character and outfit chosen.
- Changing characters in the main campaign no longer breaks infinite ammo functionality.
- Fixed missing damage animations against Blobs/Guardians of Insanity and Wesker in Lost in Nightmares. Refer to optional tweaks section to disable it.
- The DLC knife and Barry's Samurai Edge will now grant the player points for damage dealt to players in Survivors and Team Survivors.
- UI and stage props will now display when the camera is forced to follow a CPU controlled character.
- Shots fired by Barry's Samurai Edge no longer automatically count as missed shots.
- Fixed Barry's Headbutt and Excella's Humiliate melee attacks outside of Mercenaries Reunion, and First Aid no longer crashes the game.
- S75 rifle hand position offset fixed for right handed female characters. Still requires a proper animation set to look correct.
- Fixed numerous instances of partner action events where the game relied on gender to determine who does what (now checks player number). Some examples are: Jump assists, door kicking position, large gate opening position, container pushing, turret section, hovercraft cutscenes, etc.

## Optional Modification


*A set of modifiers that may provide additional challenge and / or enjoyment*


> **OFF** and **0** = Original / Intended behavior, unless stated otherwise.

Use of numbers generally signifies the existence of two or more options.

### Gameplay

- `DisableInventoryReloads` — **ON** = Cannot reload weapons by combining them with ammo in the inventory.
- `SkipDyingState` — **ON** = When your health bar drains completely, you'll die instantly, similarly to most single player entries in the series (does not work in Versus).
- `ProDyingBarOverride` — **1** = 3 seconds to resuscitate or heal your partner in Lost in Nightmares and Desperate Escape on Professional difficulty. **2** = 8 seconds to resuscitate or heal your partner in the Main Campaign on Professional difficulty.
- `ExtraVoiceCommands` — **ON** = Certain voice commands will no longer remain exclusive to CPU controlled players (originally implemented by maluc, but slightly differently).
  - Healing or resuscitating your partner.
  - Giving items to your partner.
  - Reloading (10% chance).
- `ExtraGestureCommands` — **ON** = Command for partner to pick up ammo will no longer remain exclusive to CPU controlled players.
- `ExtraAICommands` — **ON** = Enables "Thanks" and "Halt" commands while playing with a CPU controlled character.
- `HideReticles` — **ON** = Hides crosshairs and laser sights completely.
- `LaserDotType` — **ON** = Laser dot visible on all solid surfaces, similar to RE6.
- `AimDisablesMelee` — **ON** = Hides melee prompts while aiming. Only applies to controller types A and C.
- `ReloadAiming` — **ON** = Allows you to aim while reloading, similar to aiming in-between shots with the S75 sniper rifle. Directly inspired by E3 trailers and demos, seemingly removed late into development. Only works with controller and M&K classic aiming type.

### UI

- `InvertConfirmCancel` — **ON** = Inverts the controller bindings for menu navigation to match Japanese PS3s, as well as the Nintendo Switch.
- `InvertBumperTrigger` — **ON** = Inverts LB/LT and RB/RT under certain circumstances, based largely on PS3 release. For this release, QTEs remain unchanged and controller types A and C won't display the correct partner locate button when they're waiting or dying off-screen.
- `DisableInputNotification` — **ON** = No longer displays a message every time the player switches between controller and mouse and keyboard (originally implemented by maluc).
- `DisableHUDNames` — **1** = Only disables the characters' names, but leaves the container texture meant for contrast. **2** = Disables the characters' names entirely, similar to The Mercenaries 3D (useful if constantly applying different character mods).
- `DisableGameVerText` — **ON** = Removes the game version text from the title screen (originally "1.2.0", now "QOL YY/MM/DD").
- `InventoryNameType` — **0** = Name slightly offset to the left like on most console releases. **1** = Your own name will be centered, as there's no need to make room for the partner inventory button. **2** = Disables inventory names completely (useful if constantly applying different character mods).
- `InventoryNumberFontSize` — **ON** = Increases the size of the numbers in the inventory to improve legibility on a smaller screen, especially in splitscreen mode (based directly on Nintendo Switch version).
- `TitleLogoOverride` — **1** = Force "Biohazard 5". **2** = Force "Resident Evil 5".
- `GoldLogoOverride` — **1** = Force "Alternative Edition". **2** = Force "Gold Edition". **3** = Disable altogether.
- `SkipTitleVoiceDelay` — **ON** = After selecting Start Game, the game will immediately proceed to creating or loading a save file while the announcer is still talking. **Similar** to the Nintendo Switch version.
- `CustomFrameRate` — Must be a value between 10 and 10000. It replaces the 120fps cap setting (originally called "Unlocked" or "Variable" depending on the language).
- `ControllerIcons` — **0** = Xbox 360 **1** = PS4 The feature may be reworked in the future, along with PS3 and Nintendo Switch icon support.
- `UnitedTitleScreen` — **ON** = *VISUAL ONLY,* replaces Mercenaries Reunion title screen with the one from United as seen on later console re-releases.
- `RemoveLetterboxing` — **ON** = Forces the standard camera mode when the game attempts to switch to the cinematic one, which features black boxes at the top and bottom of the screen. Note that if you're playing at 16:9 (widescreen), the field of view will be narrower, as the originals rendered in some sort of ultrawide aspect ratio.
- `ExtraHudTweaks` — **ON** = Enables enemy kill counter in Mercenaries.

### Miscellaneous

- `CheapVsCharacters` — **ON** = All versus characters will cost 2000 points in the bonus features menu. Based directly on later console re-releases of the game.
- `UnlockMercs` — **ON** = Allows the player to access both Mercenaries game modes without having to finish the game first. Based directly on later console re-releases of the game.
- `UnlockPro` — **ON** = Allows the player to access Professional difficulty settings without having to beat the different modes on Veteran difficulty first, or joining a player who's hosting on Professional to permanently unlock it locally.
- `UnlockStoryCharacters` — **ON** = Allows the player to play as Sheva, Jill and Josh in the Main Campaign, Lost in Nightmares and Desperate Escape respectively, without having to beat the different modes first.
- `RemoveFilter` — **1** = Less aggressive. Keeps certain effects such as when you're dying, but doesn't work in cutscenes. **2** = More aggressive. Works in cutscenes, but also gets rid of a few post-processing effects in the process.
- `RE4MercsScoring` — **ON** = Combo bonus values will match those of the original RE4's Mercenaries. Melee kills will not grant +5 seconds, and no bonus points will be awarded upon killing 150/400 enemies per second remaining.
- `FourPlayerMercs` — **ON** = Allows for up to four players in Mercenaries in online mode. Scores will not be saved (solo or online duo) or uploaded (any) to the Leaderboards while this setting is enabled, regardless of player count.
- `RandomMinigameBGM` — **ON** = Randomizes the Mercenaries and Versus tracks. Updates on every quick restart and requires DLC content.
  - Assault Fire (The Mercenaries)
  - Killers (Survivors)
  - Rust in Summer 2008 (Slayers)
  - The Mercenaries Reunion

### Mod Compatibility

- `IgnoreMissingFiles` — **ON** = The game will not forcibly shut down due to missing expected files, but may still crash with no warning if a critical file is missing or corrupted.
- `SnWM29Fix` — **ON** = Uses a custom animation set which allows right handed female characters to reload the S&W M29 magnum properly.
- `JailBreakerFix` — **ON** = Uses a custom animation set which allows **all** right handed female characters to reload the Jail Breaker shotgun properly.
- `MissingVoiceLinesFix` — **ON** = Uses custom stq files to ensure non-DLC Chris, Sheva and Jill outfits have access to additional DLC voice lines.
- `DamageAnimationsDLCFix` — **ON** = Forces everyone to use the updated animation set from Lost in Nightmares so that they react properly to Wesker's new attacks, as well as the Blobs' acid.
- `TextFixes` — **ON** = Uses a custom set of in-game text files to ensure all new and fixed text is displayed correctly, regardless of mods.
- `HudIconFixes` — **ON** = Disables HUD fixes that rely on a modified cp_life_360.lsp file, such as missing character name textures in non-DLC modes.
