# CTR Nitro-Fueled Online - RyuNET

An unofficial adaptation for playing **Crash Team Racing: Nitro-Fueled on PS4 with RyuNET**, the community service used by OCTR on PC. The game runs on the console; a Windows computer is used to build the installer.

The aim is to make it easier to prepare an installation using each player's own files and provide PS4-specific settings through **L3+R3**.

## Download the builder

Open [Releases](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases), select **Builders — English and Spanish**, and choose one of the ZIP files under **Assets**:

| Language | File | Folder after extraction |
| --- | --- | --- |
| English | `CTR_RyuNET_Builder_EN.zip` | `CTR_RyuNET_Builder_EN` |
| Spanish | `CTR_RyuNET_Constructor_ES.zip` | `CTR_RyuNET_Constructor` |

Each ZIP includes the builder, its source code, and portable tools. Download your language's ZIP from Assets; **Code → Download ZIP** downloads the repository files and does not replace the portable builder.

Both editions provide equivalent in-game features and use the same validated packaging engine, memory controls, and progress display. The builder runs at reduced Windows priority, uses at most four .NET workers, and monitors only its own child processes. Its 768 MiB working-set threshold per process is a soft threshold, not a hard limit on total RAM usage.

## Features

- Local builder for 64-bit Windows, with portable tools.
- First-run setup and a separate RyuNET identity for each local PS4 user.
- A RyuNET nickname independent of the PSN name.
- 30 and 60 FPS caps, with **Unlimited** as a separate option.
- Native, 720p, or 480p internal resolution; motion blur and dynamic shadow options; and graphics reset.
- Contact management and joining games through CTR's original Friends menu, using compatible clients.

The 60 FPS setting is a cap: actual performance depends on the track and console. Invitations are not implemented in this PS4 adaptation.

## Before you start

This integration supports **CUSA13795 with update 1.21 and compatible executables**. Each player supplies their own game, update, and optional DLC. Game files, saves, accounts, and personal keys are not distributed.

The network implementation is based on **OCTR 0.5.3**. Later PC releases may include features that have not yet been adapted or tested here. Compatibility with every CUSA, firmware version, or network setup is not guaranteed.

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
