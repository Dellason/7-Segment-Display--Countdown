**7‑Segment Display — Countdown**

Minimal Arduino sketch to run a numeric countdown on a single 7‑segment display.

![Countdown Demo](assets/7SegmentDisplayCountdown.gif)

Quick start
- Open `countdown.ino` in the Arduino IDE (or use `arduino-cli`).
- Verify/compile and upload to your Arduino (select correct board and port).

Wiring (single digit)
- Connect segments a–g (and optional DP) to the digital pins declared in `countdown.ino`.
- Use a 220–330Ω resistor per segment.
- Common‑cathode -> GND. Common‑anode -> VCC (invert logic if needed).

Customize
- Edit the top constants in `countdown.ino` to change the countdown length, pin mapping, or timing.

Notes
- If the display shows all segments or none, verify common‑anode vs common‑cathode wiring.
- Example `arduino-cli` commands:

```
arduino-cli compile --fqbn arduino:avr:uno .
arduino-cli upload -p /dev/ttyACM0 --fqbn arduino:avr:uno .
```

License
- MIT — feel free to reuse or improve.

Enjoy! Contributions welcome.
