# ESPHome based accessories for home automation

Install ESPHome from https://esphome.io/guides/getting_started_command_line.html
On Mac, you can't use the docker method indicated there, as there is no USB device access for docker.

Install pip on the mac in some other way. Some notes https://ahmadawais.com/install-pip-macos-os-x-python

## Usage
Use ESPHome normally. I find that running the integrated dashboard works really well for uploading.
Edit in a regular editor and click upload on the dashboard or just use the dashboard

```bash
esphome . dashboard
```

## Accessories

### Bathroom (removed)
This is an RGB light, got the LEDs from amazon and they seem lower quality.
Use the 400KBPS method and 0s transition time in the light configuration to make it work.

Without the speed setting, it will light up random colors and behave strangely.
Without the 0s transition, it will not turn off completely and flicker while transitioning between colors

### Candle
After losing our baby boy Herón Nicolás during labor, I wanted to have a small creative project to keep my hands
busy. I made a small light that lights up as a candle in the evenings and helps me think about him, and to take
things slow, relax and live life to the fullest.

I used the 400KB speed variant of the neopixel library here, reusing the circuit from the bathroom light above.
I think the circuits are bad, it may be a brownout or just a blown out or defective chip in one of the LEDs.
 #TO-DO replace the LED strip

### Infinity Eclipse
A small experiment for an infinity  mirror. Functionally it's just a regular neopixel on a ESP8266 nodemcu light the
same as all above.