Built on **official SpidyVR 0.6.0**. For the full list of changes introduced in 0.6.0 and all official features, follow the [official SpidyVR page](https://github.com/IlyaMez/SpidyVR). The additions below are iplusd's contributions; original and upstream features remain credited to Ilya and their respective contributors.

# iplusd's SpidyVR — Experimental 0.6.0

Optional web and movement experiments for Marvel's Spider-Man Remastered, built and playtested locally by iplusd.

![SpidyVR gameplay](docs/images/iplusd-g1.gif)

## What's added since 0.4.3

- **Web range and flight:** 10–1000 m reach, OFF/SLOW/MEDIUM/FAST distance-based arrival, visible web extension and flutter, a gentle catch and a pulse in the controller that fired.
- **Slingshot speed:** an independent 20–300 m/s launch-speed selector.
- **Elastic Web:** adjustable stretch that softens the catch under load.
- **Smart Anchor:** an optional small aiming cone that catches nearby real surfaces after a miss.
- **Soft Release:** a short, adjustable fade of the loaded rope pull when letting go.
- **Swing Assist:** gently reduces speed into an approaching obstacle, without choosing a different route or disabling collision.
- **Two Hand Web Zip:** retract both arms quickly toward your chest at one arrived real target; stronger pulls launch harder.
- **Hand Rope Steering:** take the strand with the free hand and pull sideways to redirect existing momentum.
- **Climbing fixes:** grabbing your strand no longer fires an unintended second web; deliberate overhead pulls can start climbing from the ground; shared open-air webs can be climbed too.
- **Recording controls:** FOV OFF / 70–160 and smoothing OFF / 5–100, without changing headset FOV or locking the horizon.
- **Hand Momentum:** can now be reduced to 0%.

All custom controls are grouped in **Settings → iplusd's Experimental Settings**. The other official controls remain in **SPIDY VR**. New movement experiments default OFF; the retained small Smart Anchor assistance defaults ON. Try one new option at a time.

Web Slingshot, Better Climbing, FOV controls, FOV smoothing, Near Clip Fix and Realistic Swinging were already present in 0.4.3. This release extends them; it does not present those original additions as new. **Flips in Combat was added by Ilya**, as credited beside its menu entry.

## Download and play

1. Download the ZIP from the [experimental release](https://github.com/iplusdvr/iplusds-SpidyVR/releases/tag/v0.6.0-iplusd.1).
2. Extract the entire folder, then run **Spidy Launcher.exe** and choose **START VR**.
3. Load a save and open **iplusd's Experimental Settings** to enable the optional features.

See the [official player guide](https://github.com/IlyaMez/SpidyVR/blob/main/docs/PLAYERS.md) for supported game/headset setup. Spidy does not need to be copied into the game's installation folder.

## Recommended in-game settings

[iplusd's current in-game settings](docs/RECOMMENDED_SETTINGS.md), in menu order. This page contains in-game controls and game graphics only, with no launcher recommendations. It records the RTX 5090 profile used for the last playtest.

## Validation and current limits

- Based on official tag v0.6.0, commit `4837c064b12b051adab799945881550d2677b749`.
- 734 core checks, all three native test suites and 171 protocol checks passed. The user approved the local VR playtest before publication.
- Experimental movement can still need tuning. Swing Assist reduces collision risk; it does not guarantee collision avoidance.
- This downloadable build has controller vibration, but **no wearable bHaptics output** because it has no developer app key. The bHaptics runtime DLL is included under its original notices.
- Wall Catch and Push, added swing leg poses and sustained web-tension sound/vibration are not included. The native slingshot wind experiment did not produce confirmed visible effects and is not advertised as a working feature.

## Credits

- **Ilya Mezerowsky and upstream contributors:** SpidyVR and its official features.
- **iplusd:** the custom additions and refinements described above.
- **Blaze's Spider-Man mod for Blade & Sorcery:** inspiration for physical web movement. No assets from that mod are distributed here.

See [LICENSE](LICENSE) and [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
