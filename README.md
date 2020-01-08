# micropython-unm3-pybd-example
Example project using the micropython-unm3-pybd module with OTA updater running on a PYBD.

Copy the contents of main/ to the PYBD flash drive. Create a wifi_cfg.json file based on the template. On Power On Reset the device will use the OTA updater from https://github.com/rdehuyss/micropython-ota-updater to check for new releases of the micropython-unm3-pybd module and automatically download to the PYBD flash memory before rebooting. 

See https://github.com/bensherlock/micropython-unm3-pybd for information about the module and how to structure your own OTA updateable application modules. Add these to the ota_modules list in main.py to automatically update them OTA on power on reset. 
