# Pit Wall Duel

An offline motorsport quiz where recognising a circuit is only half the challenge. Name the track, find it on the world map, and outscore your rival.

Built for iPhone and iPad, with local two-player duels, an offline bot, and English and Croatian interfaces.

## Features

### Circuit recognition and map challenges

- Recognise 40 circuit layouts across modern and retro collections.
- Choose the correct circuit name from four answers before time runs out.
- Watch the outline gradually take shape or display the entire circuit immediately.
- Place a pin on the world map using touch controls, panning, and pinch-to-zoom.
- Earn points for correct answers, speed, and accurate locations.
- Review the real circuit location and your distance from it after each round.

### Local duels and offline opponents

- Play against a friend on the same device.
- Sit opposite each other in portrait or play side by side in landscape.
- Each player has their own controls, answers, and score.
- Play solo against a local bot with three difficulty levels: Rookie, Driver, and Champion.
- No account, matchmaking, or internet connection is required.

### Custom races and results

- Choose 8, 12, or 16 rounds.
- Select modern circuits, retro circuits, or the complete collection.
- Enable random circuit rotation for an additional challenge.
- Circuits do not repeat within the same race.
- Pause and resume a race, review its results, or start a rematch.
- See correct-answer totals, fastest-answer bonuses, average map distance, and a round-by-round recap for the current race.

### Interactive walkthrough

- A step-by-step guide opens on first launch.
- Text and interactive elements appear progressively to introduce each action.
- Practise recognising a circuit and placing a map pin before playing a timed race.
- Replay the guide from the main menu at any time.
- Respect the device's Reduce Motion preference.

### Music, sound effects, and haptics

- Looping background music continues through the tutorial, menus, and gameplay while the app is active.
- Buttons, screen transitions, and race events have distinct sound cues.
- Supported devices provide different haptic patterns for actions such as selections, confirmations, and screen changes.
- Music, sound effects, and haptics have separate on/off controls.
- Music is enabled by default; turning it off stops playback completely.

### Localisation and touch controls

- English and Croatian interfaces, including the walkthrough and results.
- Change language and feedback preferences in the app or its standard iOS Settings entry.
- Preferences are remembered between launches.
- Touch-first controls and layouts for iPhone and iPad in portrait and landscape.

## Technology

- Swift and SwiftUI for the native application shell.
- UIKit feedback generators for haptics.
- `UserDefaults`, a Settings bundle, and WebKit local storage for preferences.
- A local, rule-based bot with configurable answer accuracy, timing, and map precision; no remote AI service or language model.
- Bundled circuit data, map data, translations, and music; no game server or external runtime assets.
- Automated checks for game logic, touch interactions, localisation, audio cues, and preference handling.

## Storage and Privacy

The app stores optional player names, race configuration, language and feedback preferences, and walkthrough completion on the device. Names are local display labels, not accounts, and can be left blank.

Current-race answers, map guesses, scores, and results are held in memory. They are not uploaded or saved as a permanent match history.

The map uses bundled geographic data and the pins you place yourself. It does not request or read your device's GPS location.

The current app has no advertising, third-party analytics or tracking SDKs, account system, Game Center integration, or app-managed cloud synchronisation. Gameplay and bot decisions are processed on the device.

Device backups and Apple-provided diagnostics are separate operating-system services and depend on your Apple settings. The app does not operate its own backup or analytics service.


## Limitations

- Multiplayer is limited to two people sharing one device. There is no online multiplayer, cross-device play, matchmaking, or Game Center leaderboard.
- Completed races are not saved as a permanent history. An unfinished race cannot be restored after the app's game session is terminated or reloaded.
- Settings and player names are not synchronised between devices by the app, and there is no in-app data export or reset-all feature.
- Circuit layouts and map positions are simplified game content, not navigation tools or a live source of motorsport information.
- The bot is a simulated opponent with preset difficulty rules, not an online player or conversational AI.
- Haptic feedback depends on device hardware and system settings; it cannot be experienced in the simulator.
- Audible playback depends on the device's volume, silent mode, and selected audio output. Music pauses when the app becomes inactive or an audio interruption occurs.
