# ESPHome playground

[ESPHome](https://esphome.io/)

## General Usage

- Install ESPHome locally following the [Installation instructions](https://esphome.io/guides/installing_esphome.html).
- Check out this repo to local disk.
  ```
  git clone https://github.com/ollliegits/esphome.git
  ```
- Copy file `common/secrets.yaml.tmpl` to `common/secrets.yaml`, make it accessible to you only and fill in your secrets.
  ```
  # copy
  cp common/secrets.yaml.tmpl common/secrets.yaml

  # make private
  chmod 0600 common/secrets.yaml

  # fill in your secrets with your favorite editor.
  ```
- Start ESPHome Web Console with
  ```
  esphome dashboard .
  ```
  and [open in browser](http://0.0.0.0:6052).

## #1 Project HOME

Measure room temperature and humidity. Measurements will be displayed on OLED display, as well as pushed to an MQTT broker.

[Home config](home.yaml)

## #2 Project FLORA

Scan for nearby Xiaomi Mi Flora soil sensors, push measurements to an MQTT broker, sleep for an appropriate amount of time.

[Flora config](flora.yaml)