# Birthday Plugin for Pwnagotchi

A plugin for your Pwnagotchi that automatically finds its birthday and displays its age!

Age is based on the born_at value in the brain.json file.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


<img width="1436" alt="Screenshot 2023-06-17 at 8 22 44 PM" src="https://github.com/nullm0ose/pwnagotchi-plugins/assets/77137650/4323bea3-5488-42bf-b55c-98ac39cdf155">



## Requirements

- RTC (Real-Time Clock) synced to correct time.
- I2C interface configured.

## Notes
- Tested on Pwnagotchi version 1.5.3 and 1.5.5.
- Tested on Raspberry Pi Zero W with WaveShare 2.13inch V3 (Black and White) display.
- Works in WebUI.

## Installation

1. Ensure you have the custom plugins directory set up:
   ```
   Custom plugins directory set up: /etc/pwnagotchi/custom-plugins
   ```

2. Copy the `birthday.py` file to the custom plugins directory:
   ```
   cp birthday.py /etc/pwnagotchi/custom-plugins
   ```

3. Add the plugin configuration to the `config.toml` file:
   ```
   main.plugins.birthday.enabled = true
   main.plugins.birthday.age_x_coord = 0
   main.plugins.birthday.age_y_coord = 32
   ```

4. Fully reboot Pwnagotchi:
   ```
   sudo reboot
   ```

## Customization

You can customize the position of the displayed age on the Pwnagotchi UI by modifying the following options in the `config.toml` file:

- `main.plugins.age.age_x_coord`: X-coordinate of the age display.
- `main.plugins.age.age_y_coord`: Y-coordinate of the age display.

Feel free to adjust these values according to your preference.

## Author

- Author: nullm0ose

## Version

- Version: 1.0.

## License

This plugin is licensed under the MIT License.

---
