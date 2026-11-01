# CTR Nitro-Fueled Online - RyuNET



## PS4 v1.5.2 cumulative update



The **builders/converters are unchanged**. Update an existing compatible RyuNET installation separately, without rebuilding the complete game. [Open the v1.5.2 release](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/tag/v1.5.2).



- **In-game:** L3+R3 → Online and extras → PS4 updates → Check → View result → Update now. Wait for Update prepared, close CTR normally and reopen it.

- **Manual fallback:** download the **ES or EN .pkg update installer** from the release, copy it to USB and install it with GoldHEN Package Installer while CTR is fully closed. No Python, scripts or full-game conversion is required. These PKGs target the tested RyuNET base; independently rebuilt bases may reject the patch. Use the in-game update route if the manual package is incompatible.



This cumulative PS4 revision is based on **OCTR PC v0.7.5** and adds native in-game Graphics and private mode/cup menus while retaining the approved Online, identity, FPS and graphics options. An older installation missing the UI resource archive keeps its previous code active while the verified resource download completes; follow the ready notification and close/reopen CTR normally.



No player identity, online key, contacts, settings or save is included. New users create their own identities, and existing local profiles are preserved. Read the release's validation status and known limitations before installing. The official PC client is unchanged.



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



The 60 FPS setting is a cap: actual performance depends on the track and console. The public builder release does not include invitations; the v1.5.2 module adds RyuNET-menu invitations, with wider network testing still in progress.



## PS4 module v1.5.2



The cumulative update is pinned to OCTR PC v0.7.5. It retains the existing community friends/requests, RyuNET-menu invitations, regional relay, peer ping, signed requests and season support, and adds native in-game Graphics, private Normal/Itemless/Battle, Single/Cup, eleven cups, scoring/podiums and guest/host selector corrections. Missing remote custom racers fall back to Crash; normal SystemService Quit is retained. Experimental CPU/scenery options, Dark Mambo and the general mod manager are not included. Windows launcher/Discord changes are not presented as PS4 features.



The maintainer confirmed the v1.5.2 download/restart, Online, L3+R3 and native Graphics. 338 local regression groups passed per language. Both languages passed independent PKG and matching checks with installed and different base fingerprints. Legacy missing-resource migration has local failure-path coverage and still needs wider console confirmation. The reported official PC-host Itemless crate behavior is not claimed fixed. Public builders remain unchanged.



## Before you start



This integration supports **CUSA13795 with update 1.21 and compatible executables**. Each player supplies their own game, update, and optional DLC. Portable builders and source archives contain no game data, saves, accounts or personal identity keys. Manual update PKGs are patches containing the modified launch executable, RyuNET module and native-menu resources for the matching existing installation, not the complete game or DLC.



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

