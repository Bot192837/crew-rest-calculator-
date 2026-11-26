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

## Set up the "Crew Rest Alarms" Shortcut (do once)
The app sends each call as `seconds-from-now|label`, one per line. The Shortcut turns each line into a Clock alarm. Because the app sends time from now, not a clock time, the phone's time zone setting does not matter when you set the alarms.

1. Open **Shortcuts** → **+** → name it exactly `Crew Rest Alarms`.
2. Tap **ⓘ**. If it shows a **Receive** input setting, set it to **Text**.
3. Add **Split Text**: input `Shortcut Input`, separator **New Lines**.
4. Add **Repeat with Each** item in `Split Text`.
5. Inside the repeat, add **Split Text**: input `Repeat Item`, separator **Custom** → `|`.
6. Add **Get Item from List**: **First Item** from `Split Text` (this is the seconds).
7. Add **Get Item from List**: **Last Item** from the same `Split Text` (this is the label).
8. Add **Adjust Date**: **Add** `First Item` **seconds** to `Current Date`.
9. Add **Create Alarm**: time `Adjusted Date`, label `Last Item`.
10. Leave **End Repeat** at the end.

### Test it on the ground
1. Enter a take-off time a few minutes ago and a flight time, e.g. 02:00 (gives a call ~15 min later).
2. Tap **SET ALARMS**. Shortcuts opens and creates the alarms.
3. Open **Clock → Alarms** and check the times (shown in phone local time).

## Watch-outs
- Clock alarms keep their local clock time. If the phone time zone changes after you set them (e.g. inflight Wi-Fi with automatic time zone), tap **SET ALARMS** again.
- Calls that have already passed are skipped.
- Old alarms stay in the Clock app. Delete them after the flight.
- Take-off date: if now is between take-off and ETA, the app uses that flight. Otherwise it uses the next take-off at that time.
