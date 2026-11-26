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
2. Tap **START TIMER**. The iOS Clock timer starts, set exactly to the call time.
3. Swipe back to the app.

Backup: if the Shortcut is missing, read the **Clock timer** value under the call and set it in **Clock → Timers** by hand. That value rounds down, so it rings on time or up to 1 min early.

iOS runs one Clock timer at a time: start the next call's timer, then start the following one after it rings.

## Set up the "Crew Rest Timer" Shortcut (do once, 1 action)
1. Open **Shortcuts** → tap **+** → name it exactly `Crew Rest Timer`.
2. Add the action **Start Timer**.
3. Tap the duration → choose **Shortcut Input** → set the unit to **seconds**.

Test it on the ground: enter a take-off time a few minutes ago (UTC) and a flight time of 02:00, then tap **START TIMER**. Check **Clock → Timers**. Also check what happens when a timer is already running.

## Watch-outs
- After a call time passes, the app shows **Passed** for it.
- Take-off date: if now is between take-off and 6 h after ETA, the app uses that flight. Otherwise it uses the next take-off at that time.
