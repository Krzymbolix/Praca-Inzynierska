🇬🇧 English | 🇵🇱 [Polski](README.pl.md)

# Access Control Device — Engineering Thesis

Hardware (PCB) design of an access control device, developed as an engineering
(BEng) thesis in **Internet of Things Engineering** at the **Warsaw University of
Technology**, Faculty of Electronics and Information Technology.

The device authorizes access using a **fingerprint** reader together with **NFC**
and **BLE** communication, built around the **BL54L15u (Nordic nRF54L15)** radio module.

> 📷 *[Add a photo of the assembled board or a 3D render of the PCB from Altium here — this is the single most important part of the README.]*

---

## Features

- Fingerprint reading as part of the access authorization
- **BLE** (Bluetooth Low Energy) wireless communication
- **NFC** communication
- Access control logic running on the nRF54L15 module
- Fully custom PCB design — from schematic to layout

## Hardware Architecture

The block diagram of the device is in `Schemat_blokowy.SchDoc`.

Main blocks:
- **MCU / radio** — BL54L15u module (Nordic nRF54L15: BLE + NFC) — `MCU.SchDoc`
- **Fingerprint reader** — [model / interface, e.g. UART/SPI — fill in]
- **Power supply** — `Zasilanie.SchDoc` — [e.g. USB / battery powered, voltage regulation — fill in]

## Key Components

| Component | Description |
| --- | --- |
| **BL54L15u** | Radio module based on Nordic **nRF54L15** (BLE + NFC), chip antenna |
| **Fingerprint reader** | [model — fill in] |
| **Power supply** | [description — fill in] |

## Repository Contents

| File | Description |
| --- | --- |
| `KD_Praca_Inzynierska.PrjPcb` | Main Altium Designer PCB project |
| `Schemat_blokowy.SchDoc` | Device block diagram |
| `MCU.SchDoc` | MCU / radio module schematic |
| `Zasilanie.SchDoc` | Power supply schematic |
| `PCB1.PcbDoc` | PCB layout |
| `WlasneElementy.SchLib` | Custom-made component symbols |
| `453-00223_BL54L15u_Chip ANT_SCH_Symbol_Altium.SchLib` | BL54L15u module symbol |
| `basic_lib_v10.SchLib` | Basic component library |

## How to Open

The project requires **Altium Designer**:

1. Clone the repository:
   ```bash
   git clone https://github.com/Krzymbolix/Praca-In-ynierska.git
   ```
2. Open `KD_Praca_Inzynierska.PrjPcb` in Altium Designer.
3. Open schematics from the *Projects* panel; the layout is in `PCB1.PcbDoc`.

## Stack / Tools

`Altium Designer` · `nRF54L15 (BL54L15u)` · `BLE` · `NFC` · `PCB design` ·
`firmware: nRF Connect SDK`

## Status

[e.g. "PCB design complete, firmware in progress" — update with the current state.]
Firmware: [link to a separate firmware repo if any — or "same repo / in progress".]

## Author

**Krzysztof Dobosz** — [github.com/Krzymbolix](https://github.com/Krzymbolix)
Engineering thesis, Warsaw University of Technology (FEIT), Internet of Things Engineering.
