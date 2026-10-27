# Behringer IGNITE (BE 0716-AAF)

> There is a Creator in every human being. Our mission is to empower those who have not and cannot.

Source code for the Behringer IGNITE 64-channel multi-track sequencer.

<p align="center">
  <img src="docs/images/ignite-front.jpg" alt="Behringer IGNITE" width="720">
</p>

## Key features

- 64-channel multi-track sequencer with a song, scene, track and pattern structure
- Patterns of up to 16 bars with 16 steps per bar, scenes of up to 200 bars, 96 PPQN timing
- Real-time recording, undo, fill, solo/skip, gang and sculpt functions
- Transpose control and up to 10 user-defined scales
- Internal General MIDI sound engine
- 5 MIDI DIN in/out pairs, USB MIDI, and USB host MIDI for up to 5 devices
- MIDI clock sync, MIDI Machine Control and remote control
- 8 CV and 8 Gate jacks with calibration, plus sync in/out
- Wi-Fi connectivity

## Release status

This repository contains the IGNITE application, its audio engine and hardware protocol, and the
Buildroot tree for the Linux image. Material that could not be redistributed was removed, so some
parts need your own replacements before they build (see the README in each folder). There is no
official firmware release here yet.

## Front panel

- Touchscreen
- 16 RGB step pads, each with its own encoder
- 8 assignable knobs (A–H) and a jog wheel
- ROW and BAR encoders
- Transport, song/scene/track/pattern, and edit buttons
- USB-A port (5 V, 1 A) with a USB STOP button

## Connections

<p align="center">
  <img src="docs/images/ignite-rear.jpg" alt="Behringer IGNITE rear panel" width="100%">
</p>

| Rear panel |
|---|
| Power switch, 12 V DC input (2000 mA) |
| USB-C |
| 5 × MIDI IN / OUT (5-pin DIN) |
| 8 × CV, 8 × Gate |
| Sync in and out |
| Line / headphone output |

## Repository

| Folder | Contents | License |
|---|---|---|
| [`Source/Application/`](Source/Application) | IGNITE application (UI, model and hardware integration, built on JUCE) | AGPL-3.0-or-later |
| [`AudIO/`](AudIO) | Audio engine library | AGPL-3.0-or-later |
| [`ComProtocol/`](ComProtocol) | Hardware communication protocol | AGPL-3.0-or-later |
| [`Linux/`](Linux) | Buildroot Linux image for the i.MX8M Mini SOM | GPL-2.0 (Buildroot) |

## Licensing

Original software in this repository is licensed under **AGPL-3.0-or-later**; see [LICENSE](LICENSE).
The Buildroot tree in `Linux/` is GPL-2.0 (see `Linux/buildroot/COPYING`), and the packages it builds keep
their own licenses.

Third-party components retain their original licenses and notices. Each folder's README lists the
bundled third-party code and its license. The LICENSE does not relicense third-party code, images or
trademarks.

## Contribute and get help

You do not need organization membership or a company account to participate. Use your own GitHub
account to open an issue or send a pull request. Sign off commits with `git commit -s`.

- [Contribution guide](https://github.com/MusicTribeOpenSource/.github/blob/main/CONTRIBUTING.md)
- [Code of conduct](https://github.com/MusicTribeOpenSource/.github/blob/main/CODE_OF_CONDUCT.md)
- [Community governance](https://github.com/MusicTribeOpenSource/.github/blob/main/GOVERNANCE.md)
- [Discord community](https://discord.gg/gS6qtuShvw)

## Security

Do not disclose vulnerabilities, personal information or credentials in public issues.
Use [private vulnerability reporting](https://github.com/MusicTribeOpenSource/0716-AAF/security/advisories/new).
See [SECURITY.md](SECURITY.md) for scope and response expectations.

## Maintainers

Reviews are routed to the organization's **Owners** team. Default-branch protection,
code-owner review and the organization's sign-off workflow apply here.

## Names and logos

Behringer is a brand of MUSIC Tribe. The Behringer and IGNITE names and logos are not granted under
the software license. The product photos in `docs/images/` are not covered by the software license
either. See the organization's
[trademark policy](https://github.com/MusicTribeOpenSource/.github/blob/main/TRADEMARKS.md).

Copyright (c) MUSIC Tribe.
