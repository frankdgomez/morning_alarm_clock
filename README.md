# morning_alarm_clock
This script turns your Home Assistant setup into a smart alarm clock. It wakes you up gently with music, light, and motion-based stop logic.

This script turns your Home Assistant setup into a smart alarm clock.
It wakes you up gently with music, light, and motion-based stop logic.

Features
	•	Plays a local MP3 (from My Media) on your HomePod Mini or any media player.
	•	Turns on your bedroom light at a soft brightness.
	•	Keeps replaying and slowly increases volume until motion is detected in the bathroom.
	•	Stops automatically once you get up and move.
	•	Works standalone or can be scheduled by an automation at any time you choose.

Inputs
	•	media_path: MP3 or stream to play (media-source://media_source/local/YourSong.mp3)
	•	start_vol: starting volume (0 – 1)
	•	step_vol: how much to raise each retry
	•	max_vol: maximum volume cap
	•	interval_min: minutes between retries
	•	window_min: maximum alarm duration before giving up

  Example use
Create an automation triggered at 06 : 30 that calls:

service: script.morning_alarm_run
