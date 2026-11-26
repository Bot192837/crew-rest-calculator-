# Crew Rest Calculator

Offline crew rest calculator for double and augmented crew ops. Works in airplane mode after you install it once.

**App:** https://bot192837.github.io/crew-rest-calculator-/

## Rules used
- Rest starts at take-off + 30 min.
- Total rest = flight time − 90 min.
- Double = 2 rests, Augmented = 3 rests. Equal whole minutes. Leftover minutes go to the last rest.
- Calls: one per handover (end of each rest), set at the handover or 5 / 10 / 15 min before.

## Day / night colours
- **Day:** dark text on a light background, which reads better in bright light.
- **Night:** soft warm-grey text on a near-black background, with no blue light. Medium contrast reduces glare and blur around the text.
- Tap **NIGHT / DAY** at top right to switch. The app remembers your choice. First launch follows the phone's dark mode setting.
- At night, also set the phone brightness low.

## Install on iPhone / iPad (do once, with signal)
1. Open the app link in **Safari**.
2. Tap **Share → Add to Home Screen**.
3. Open it once from the Home Screen. It is now available offline.

After an update, open the app once with signal to get the new version.

## Set a call
1. Choose **At / −5 / −10 / −15** for the call.
2. Read the **Clock timer** value under the call (time from now until the call).
3. Open **Clock → Timers** and set that time. Start it.

The timer value updates every 30 s. It rounds down, so the timer rings at the call time or up to 1 min early, never late. A timer counts down in real time, so a phone time zone change does not affect it. iOS runs one Clock timer at a time: set the next call's timer, then set the following one after it rings.

## Watch-outs
- After a call time passes, the app shows **Passed** for it.
- Take-off date: if now is between take-off and 6 h after ETA, the app uses that flight. Otherwise it uses the next take-off at that time.
