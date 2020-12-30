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

### Bathroom
This is an RGB light, got the LEDs from amazon and they seem lower quality.
Use the 400KBPS method and 0s transition time in the light configuration to make it work.

Without the speed setting, it will light up random colors and behave strangely.
Without the 0s transition, it will not turn off completely and flicker while transitioning between colors