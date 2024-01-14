Flashing Firmware

- Flash the RPI2040 Zero by pressing and holding the boot button while plugging in the USB until it's detected on the computer as a new drive.

- Drag and drop or copy and paste the file with the .uf2 extension onto the drive. Wait until the keyboard is detected.

Unfortunately, the VIA support hasn't been merged into the branch yet. However, to use it, follow these additional steps:

- Visit https://usevia.app/ and navigate to the gear icon, then enable the "Show Design Tab" option.
- Once active, open the brush icon next to the gear. Click "Load" on the "Load Draft Definition" menu and input the via.json file located in the firmware folder.
- Return to the configuration menu, click on "Device Authorization," and your keyboard will appear, ready to use.

Choose "Mist65_via" for VIA support or "Mist65_default" for the default keymap without VIA support.

Create a new keymap tutorial soon!
