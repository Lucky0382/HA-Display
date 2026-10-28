# DisplayIQ wall panel

ESPHome firmware for a Waveshare ESP32-S3-Touch-LCD-3.5-C, built by GitHub Actions.

## One-time setup
1. Settings > Secrets and variables > Actions > New repository secret:
   - `WIFI_SSID` - your home Wi-Fi name
   - `WIFI_PASSWORD` - your home Wi-Fi password
2. Actions tab > **Build firmware** > **Run workflow**.

## Install
1. Open the finished run and download **displayiq-firmware** (a zip). Unzip it.
2. In Chrome or Edge, go to https://web.esphome.io and plug the display in by USB-C.
3. Click **Connect**, pick the port, then **Install** and choose the `.factory.bin` file.

After the first USB install, later builds can be installed over Wi-Fi from
Home Assistant's ESPHome page (Install > Manual) using the `.ota.bin` file.

## Changing the panel
Edit `wall-panel.yaml` on GitHub and commit - a new build starts automatically.
