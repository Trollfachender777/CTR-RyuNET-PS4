## PS4 update — no conversion required

**The English and Spanish builders/converters have not been updated. Install this update on an existing compatible CTR RyuNET PS4 installation without converting the game again.**

| Manual PS4 update | Download |
| --- | --- |
| English L3+R3 menu | [Download EN PKG](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/download/v1.2.1/CTR_Nitro-Fueled_Online_RyuNET_v1.2.1_Update_EN.pkg) |
| Menú L3+R3 en español | [Descargar PKG ES](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/download/v1.2.1/CTR_Nitro-Fueled_Online_RyuNET_v1.2.1_Update_ES.pkg) |

**Manual PKG compatibility:** these patches require the tested **RYUN00001** reference base. Matching the CUSA or title ID alone is insufficient: independently rebuilt bases can have a different fingerprint and reject the patch with **CE-36433-9**. For other compatible installations, use the working L3+R3 module updater. A manual patch for another base must be bound to that exact original package.

Reference base content digest: `8e4ef1f90576c0bd634a51a059ab05c7fe813b59cd8dd0dac82255fcb7a6dd77`.

## What changed in v1.2.1

Restores automatic activation of the season event announced by RyuNET. The event query runs in the background and the selected mode applies when the next track loads. The server selects the normal, Halloween or Golden Wumpa mode; no game assets need replacing.

The v1.2.0 network adaptation and approved settings remain: Online, friends and requests, RyuNET-menu invitations, relay selection, room ping, independent identities/nicknames, FPS caps and graphics options. The PC client and converter ZIPs are unchanged. The network reference remains selected components from [OCTR v0.6.4](https://github.com/Ryu7w7/OCTR-NitroFueled-PC/releases/tag/v0.6.4), rather than complete PC feature parity.

## Option 1 — update directly from PS4

On an installation with the compatible updater:

1. Open **L3+R3 → Online and extras → PS4 updates → Check for updates → View result**.
2. Choose **Update now** for **v1.2.1** and wait for **Update prepared**.
3. Close CTR normally from the PS menu, then reopen the game.
4. Check the **L3+R3 v1.2.1** menu and Online.

Spanish path: **L3+R3 → Online y extras → Actualizaciones PS4 → Buscar actualizaciones → Ver resultado → Actualizar ahora**. Wait for **Actualización preparada**, close CTR normally and reopen it. This update route needs no PC or converter. Legacy installations without the compatible updater still need its one-time setup; copying a PRX alone does not add a missing loader.

## Option 2 — manual PKG fallback

For the matching reference base above:

1. Close CTR normally and leave GoldHEN enabled.
2. Install **one** PKG language over the existing **CTR Nitro-Fueled Online - RyuNET** installation.
3. Open the usual CTR game, then check Online and L3+R3.

Do not uninstall the game or launch a separate recovery app. PS4 application information shows **1.23**, while the RyuNET menu shows **v1.2.1**. This cumulative patch includes the previous approved functions and keeps the module updater available. Saves, identities, nicknames, contacts and graphics preferences are preserved.

**Español:** el convertidor sigue igual. Actualiza desde L3+R3 o instala el PKG de tu idioma sobre la base compatible, con CTR cerrado. No necesitas volver a convertir ni borrar el juego. Después cierra y abre CTR normalmente.

## Validation and source

The maintainer confirmed the v1.2.1 module on the reference PS4: the season event, Online and L3+R3 all work. The console log confirms successful hook installation and server-mode selection. ES and EN passed local module/protocol tests. The existing v1.2.0 updater was executed with the real v1.2.1 module in emulation, verifying download, rollback, executable permissions and preservation of user profiles.

Both manual PKGs passed 32 container checks each, payload readback, exact original-base binding, save-metadata/keystone preservation and native loader tests at two load addresses. The new loader rejects the older v1.2.0 override so the bundled v1.2.1 module can load. The v1.2.0 manual format was confirmed on the reference console; the newly rebuilt v1.2.1 PKGs have not been separately installed there. These checks do not establish compatibility with every independently built base or network.

- `source.zip`: corresponding ES/EN module source, upstream references, build/test scripts, license and notices.
- `PKG_Update_Source_v1.2.1.zip`: corresponding manual loader and packaging source; rebuilding requires your own compatible game and exact base package.
- `SHA256SUMS.txt`: checksums of the attached binaries, sources and instructions.

Builders and source archives contain no game data, saves or identity keys. Manual update PKGs contain the modified launch executable and RyuNET module for the existing installation, rather than the complete game, tracks or DLC. The [original English and Spanish builders](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/tag/constructores) remain available for initial setup.

## Credits

[Ryu7w7 and OCTR/RyuNET contributors](https://github.com/Ryu7w7/OCTR-NitroFueled-PC), [GetLostIn](https://github.com/GetLostIn/CTR-NitroFueled-PC), SacredFire, bbport, shadPS4, OpenOrbis, GoldHEN and LibOrbisPkg contributors. PS4 adaptation and integration by **Trollfachender777** with **AI assistance**. Existing upstream licenses and notices remain applicable; see the [full credits](https://github.com/Trollfachender777/CTR-RyuNET-PS4/blob/main/CREDITOS.md).
