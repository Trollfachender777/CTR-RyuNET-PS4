# CTR Nitro-Fueled Online - RyuNET

## Latest PS4 update: v1.2.1

**[Open v1.2.1 — PS4 updates, English and Spanish](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/tag/v1.2.1)**

**The builders/converters have not been updated. Update your existing PS4 installation without rebuilding or converting the game again.**

- **Option 1:** use **L3+R3 → Online and extras → PS4 updates** on an installation with the compatible updater, then close and reopen CTR normally.
- **Option 2:** [English manual PKG](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/download/v1.2.1/CTR_Nitro-Fueled_Online_RyuNET_v1.2.1_Update_EN.pkg) · [PKG manual en español](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/download/v1.2.1/CTR_Nitro-Fueled_Online_RyuNET_v1.2.1_Update_ES.pkg).

**Manual PKG requirement:** the r4 packages are paired to the tested reference base. Independently rebuilt bases may have different fingerprints even with the same CUSA/title ID. Read the compatibility section in the release before installing. The working L3+R3 update route remains available.

En español: **el convertidor sigue igual; la actualización de PS4 se instala aparte, sin volver a convertir el juego**. Los PKG manuales requieren una base cuya huella coincida.

An unofficial adaptation for playing **Crash Team Racing: Nitro-Fueled on PS4 with RyuNET**, the community service used by OCTR on PC. The game runs on the console; a Windows computer is used to build the installer.

The aim is to make it easier to prepare an installation using each player's own files and provide PS4-specific settings through **L3+R3**.

## Download the builder

For an initial installation, open the [unchanged builder release](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/tag/constructores) and choose one ZIP under **Assets**:

| Language | File | Folder after extraction |
| --- | --- | --- |
| English | `CTR_RyuNET_Builder_EN.zip` | `CTR_RyuNET_Builder_EN` |
| Spanish | `CTR_RyuNET_Constructor_ES.zip` | `CTR_RyuNET_Constructor` |

Each ZIP includes the builder, its source code, and portable tools. Download your language's ZIP from Assets; **Code → Download ZIP** downloads the repository files and does not replace the portable builder.

Both editions provide equivalent in-game features and use the same validated packaging engine, memory controls, and progress display. The builder runs at reduced Windows priority, sets the processor count exposed to .NET to at most four, and monitors only its own child processes. Its 768 MiB working-set threshold per process is a soft threshold, not a hard limit on total RAM usage.

## Features

- Local builder for 64-bit Windows, with portable tools.
- First-run setup and a separate RyuNET identity for each local PS4 user.
- A RyuNET nickname independent of the PSN name.
- 30 and 60 FPS caps, with **Unlimited** as a separate option.
- Native, 720p, or 480p internal resolution; motion blur and dynamic shadow options; and graphics reset.
- Contact management and joining games through CTR's original Friends menu, using compatible clients.

The 60 FPS setting is a cap: actual performance depends on the track and console. The public builder release does not include invitations; the v1.2.1 module adds RyuNET-menu invitations, with wider network testing still in progress.

## PS4 module v1.2.1

The [PS4 v1.2.1 update](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/tag/v1.2.1) adapts selected OCTR v0.6.4 network protocols: server friends and requests, RyuNET-menu invitations, regional relays, peer ping and signed background requests. The maintainer confirmed the v1.2.1 module, Online, L3+R3 and season-event activation on the reference PS4. Manual PKGs use the previously corrected base-binding format; the release describes their compatibility and validation. The update also restores automatic season-event activation from the server. The public builder ZIPs are unchanged. See the release for update instructions and the exact base-package requirement for manual PKGs.

## Before you start

This integration supports **CUSA13795 with update 1.21 and compatible executables**. Each player supplies their own game, update, and optional DLC. Portable builders and source archives contain no game data, saves, accounts or personal identity keys. Manual update PKGs are patches containing the modified launch executable and RyuNET module for the matching existing installation, not the complete game or DLC.

The public builder release is based on **OCTR 0.5.3**. Later PC releases may include features that have not yet been adapted or tested here. Compatibility with every CUSA, firmware version, or network setup is not guaranteed.

## Read the instructions in this order

1. [Prepare your files, build the PKG, and install it](GUIA_DE_USO.md).
2. [Configure FPS, graphics, your nickname, and friends](MENU_L3_R3.md).
3. [Authors, upstream projects, and tools](CREDITOS.md).

The guide gives the **action first**, followed by **what it does** under each step. It includes the folder and script names for both the English and Spanish editions.

## Main acknowledgments

This work builds on [OCTR and RyuNET by Ryu7w7 and contributors](https://github.com/Ryu7w7/OCTR-NitroFueled-PC), and [GetLostIn's Windows port](https://github.com/GetLostIn/CTR-NitroFueled-PC). The full credits also cover SacredFire, bbport, shadPS4, and the development tools.

The PS4 adaptation does not claim authorship of the original PC port or the RyuNET server. It is an independent community project with no official affiliation with the game's rights holders.

## Validation status

A complete build using the developer's own game files, executable readback from the generated PKG, and local module tests have been checked. The author has confirmed startup, Online access, and separate profiles when switching local users on the development console. Testing on one console does not establish compatibility with every system or network.
