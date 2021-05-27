# nswitch

Nintendo Switch Homebrew Repo
How to set up emuNAND with Atmosphere

Download the apps to a folder:
[Hekate](https://github.com/CTCaer/hekate/releases/latest/)
[Atmosphere 0.18.1](https://github.com/Atmosphere-NX/Atmosphere/releases/tag/0.18.1)
[SigPatches](https://github.com/ITotalJustice/patches/releases)

Download the payload injector
[TegraRcmGUI](https://github.com/eliboa/TegraRcmGUI)

## 2. Step

Extract these files into the root of your SD card:
`hekate_ctcaer_x.x.x_Nyx_x.x.x.zip`
`atmosphere-x.x.x-master.zip`
`fusee.zip`

## 3. Step 3

Place the file named `fusee-primary.bin` in your `/bootloader/payloads/` folder.
Create a file named `hekate_ipl.ini` inside of your `/bootloader/` folder and paste this within the file:

```bash
[config]
autoboot=0
autoboot_list=0
bootwait=3
backlight=100
autohosoff=0
autonogc=1
updater2p=0
bootprotect=0

[Atmosphere CFW]
payload=bootloader/payloads/fusee-primary.bin
icon=bootloader/res/icon_payload.bmp

[Stock SysNAND]
fss0=atmosphere/fusee-secondary.bin
stock=1
emummc_force_disable=1
icon=bootloader/res/icon_switch.bmp
```

Create the file `exosphere.ini` in the root of your SD card and paste this inside (this step is needed in order to blank your prodinfo so that you can avoid getting your switch banned):

```bash
[exosphere]
debugmode=1
debugmode_user=0
disable_user_exception_handlers=0
enable_user_pmu_access=0
blank_prodinfo_sysmmc=0
blank_prodinfo_emummc=1
allow_writing_to_cal_sysmmc=0
log_port=0
log_baud_rate=115200
log_inverted=0
```

Afterwards create a file named `default.txt` in `/atmosphere/hosts/` (the hosts folder won't exist, so make sure to create it) and paste this in your `default.txt` file (this step is prevents you from connecting to Nintendo's servers):

```bash
# Block Nintendo Servers
127.0.0.1 *nintendo.*
127.0.0.1 *nintendo-europe.com
127.0.0.1 *nintendoswitch.*
95.216.149.205 *conntest.nintendowifi.net
95.216.149.205 *ctest.cdn.nintendo.net
```

<https://nsw2u.org/page/4>
