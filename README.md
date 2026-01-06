# EM Field Detector – My First Arduino Project

This is my very first Arduino project! I wrote this while learning the basics of reading analog inputs and controlling LEDs. It's simple and messy but it taught me about:

- Reading sensor values with `analogRead()`
- Smoothing readings using a moving average
- Mapping sensor values to LED thresholds
- Using `digitalWrite()` to control multiple LEDs
- Serial debugging with `Serial.println()`

## How it Works

1. Connect a sensor (like a copper wire strip) to pin A5.
2. LEDs are connected to pins 2–11.
3. The program reads the analog value, smooths it over 25 readings, and lights up LEDs progressively based on the average.

## Lessons Learned

- Averaging sensor readings reduces noise and gives more stable LED output.
- Mapping values helps in scaling sensor input to a usable range.
- Always keep a history of your readings for smoother output.

## Improvement Areas

- Refactor to use arrays and loops instead of 10 separate `if` statements.
- Replace hard-coded pin numbers with arrays for scalability.

This project is intentionally left as-is to document my learning journey.
