# Third-party notices

The Joy-Con 2 Dongle firmware is GPL-3.0 (see `LICENSE`). Parts of it come
from, or follow, the projects below under their own licences. Each licence is
kept verbatim in `LICENSES/`, and a copy of this file and of `LICENSES/`
travels with the firmware images in `dist/` (and on the tool page).

## HIDMaestro (MIT)

<https://github.com/hifihedgehog/HIDMaestro>

Used in `main/out_steam.c` (Steam Controller mode): the steam-controller-2
profile's HID report descriptor, USB layout and the command-channel answers
Steam checks. Shipped in every firmware image.

Licence: [`LICENSES/HIDMaestro_LICENSE.txt`](LICENSES/HIDMaestro_LICENSE.txt)
(`Copyright (c) 2026 HIDMaestro Contributors`, MIT).

## GP2040-CE (MIT)

<https://github.com/OpenStickCommunity/GP2040-CE>

Used in `main/out_xinput.c`, `main/out_ds4.c` and `main/out_switchpro.c`:
the XInput, DS4 and Switch Pro Controller USB descriptors, report layouts and
protocol handling (Switch Pro: the 0x80 handshake, subcommand replies and SPI
flash answers). The web configurator approach follows GP2040-CE too. Shipped
in every firmware image.

Licence: [`LICENSES/GP2040-CE_LICENSE.txt`](LICENSES/GP2040-CE_LICENSE.txt)
(`Copyright (c) 2024 OpenStickCommunity (gp2040-ce.info)`,
`Copyright (c) 2021 Jason Skuby (mytechtoybox.com)`, MIT).

## sc2-research (MIT)

<https://github.com/CouchTurtle/sc2-research>

Used in `main/out_steam.c`: the Steam Controller haptic output reports
0x81..0x85 (sides, gain in dB), from its HAPTICS.md.

Licence: [`LICENSES/sc2-research_LICENSE.txt`](LICENSES/sc2-research_LICENSE.txt)
(`Copyright (c) 2026 sc2-research contributors`, MIT).

## SDL (zlib)

<https://github.com/libsdl-org/SDL>

Used as a reference for `main/out_steam.c`: the Steam Controller input report
0x42 layout, button bits, IMU scale and rumble, from
`src/joystick/hidapi/SDL_hidapi_steam_triton.c` and
`src/joystick/controller_structs.h`. No SDL source file is included.

Licence: [`LICENSES/SDL_LICENSE.txt`](LICENSES/SDL_LICENSE.txt)
(`Copyright (C) 1997-2026 Sam Lantinga`, zlib).

## Protocol research (credited, no code taken)

Switch2Connect (TommyWabg, GPL-3.0: this project is based on it, hence its
GPL-3.0 licence), Nadeflore/switch2-controllers,
ndeadly/switch2_controller_research, german77/JoyconDriver,
TheFrano/joycon2py, darthcloud/BlueRetro and iczero/steam-controller-stuff.
