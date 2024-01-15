
## Materials

Part list
| Name          | Quantity     | Description                |
| :-------------| :----------- | :------------------------- |
| `1N4148`      | `66`         | DO-35 (1N4148 or similar).  |
| `RP2040 Zero` | `1`          | RP2040 Zero (You can use all models, but first pay attention to the pinout). |
| `Kailh hotswap socket (optional)` | `66` | if you want hotswap features and south facing switches. |
| `Mist65 PCB`  | `1`          | Mist65 PCB is available for purchase [here](https://tokopedia.link/6WUgB6gHmGb).|

Case part list

| Name            | Quantity    | Details|
| :---------------| :-----------| :------|
| `Layer 1`       | `1`         | 3mm thicknes.   |
| `Layer 2`       | `3`         | 3mm thickness.   |
| `Layer 3`       | `2`         | 3mm thickness.   |
| `Layer 4`       | `1`         | 1.5mm thickness. |
| `Layer 5`       | `2`         | 3mm thickness.   |
| `bolts and nuts`| `8`         | M2 size with 30mm length.|

*layer 1 is the bottom layer (in order of top).

Tools needed

| Name            | Details      |
| :---------------| :------------|
| `Solder`        |  Any kind of solder is suitable, but I recommend using a pointed or sharp-tipped one.   |
| `Tin`           | You'll need approximately 4-5 meters of tin wire.   |
| `Flux`          | Any type of flux is acceptable, but avoid overusing it.  |
| `Tweezers`      | Opt for tweezers with a hooked shape. |
| `Nail clippers` | Any type with flat surfaces will work.   |

## Let's start building

Firstly, prepare the necessary tools and materials. I will provide you with some tips and tricks. I recommend a soldering temperature of 300 to 350 degrees Celsius; please note that high temperatures can damage the PCB traces. Additionally, the soldering tip may quickly turn black. Each time you solder, ensure to clean the soldering tip thoroughly to prevent residue from sticking to the soldered joints later.

The use of nail clippers instead of cutting pliers is for precision, allowing you to trim component legs more neatly. Before soldering, apply an adequate amount of flux to the PCB. Applying too much flux can complicate cleaning later. Once everything is ready, test-fit the components in place, ensuring they match the silk screen markings on the PCB. Trim any excess component legs promptly; although it may take time, patience is crucial for satisfactory results.

Afterward, solder the components one by one, using tweezers to position them accurately. If a component is tilted, you can correct it with tweezers, but be cautious as this process involves melting the tin and adjusting the component's position. For the microcontroller, there is a ">" sign indicating pin 0 on the rp2040 zero; refer to the picture [below](https://github.com/naaeell/Mist65/blob/main/mist65/pictures/20240113_094051.jpg) for the microcontroller's position. Before soldering, verify that the component placement is correct to achieve neat soldering results.

Begin soldering slowly, ensuring not to melt too much tin; excessive tin can result in poor solder joints. Once all components are soldered, clean the PCB with isopropyl alcohol or contact cleaner.

## Flashing Firmware

- Flash the RPI2040 Zero by pressing and holding the boot button while plugging in the USB until it's detected on the computer as a new drive.

- Drag and drop or copy and paste the file with the .uf2 extension onto the drive. Wait until the keyboard is detected.

#### Unfortunately, the VIA support hasn't been merged into the branch yet. However, to use it, follow these additional steps:

- Visit [https://usevia.app/](https://usevia.app/) and navigate to the gear icon, then enable the "Show Design Tab" option.
- Once active, open the brush icon next to the gear. Click "Load" on the "Load Draft Definition" menu and input the via.json file located in the firmware folder.
- Return to the configuration menu, click on "Device Authorization," and your keyboard will appear, ready to use.

Choose "Mist65_via.uf2" for VIA support or "Mist65_default.uf2" for the default keymap without VIA support.

Create a new keymap tutorial soon!
