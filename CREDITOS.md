# Credits and acknowledgments

This PS4 adaptation exists thanks to the earlier work of several people and communities. The credits below recognize their contributions; they do not imply that these authors developed, reviewed, or endorsed this PS4 edition.

## Online and RyuNET

**[Ryu7w7 and contributors — OCTR-NitroFueled-PC](https://github.com/Ryu7w7/OCTR-NitroFueled-PC):** development of the online fork and the RyuNET community server. Their work provides the reference for this adaptation's network compatibility, profiles, sessions, and friends.

Authorship of the RyuNET service and original Online implementation belongs to that project. This edition adapts the integration to PS4; it does not claim to have created the server.

## PC port and underlying projects

- **[GetLostIn — CTR-NitroFueled-PC](https://github.com/GetLostIn/CTR-NitroFueled-PC):** the Windows port on which the online fork was developed.
- **T3CHNOLOG1C — SacredFire:** the native CTR Linux port from which those foundations originated. Reference: [OCTR credits](https://github.com/Ryu7w7/OCTR-NitroFueled-PC#credits).
- **deadinside28 and contributors — bbport:** loader, runtime, and rendering foundations acknowledged by SacredFire and the PC projects.
- **Supermedo:** the Windows adaptation of bbport used by the PC port.
- **The shadPS4 team and contributors:** video-core and shader-recompilation work used in the PC projects' lineage.
- **illusion and TroyWarez — [PS-Game-Patch](https://github.com/illusionyy/PS-Game-Patch):** community game patches acknowledged by the upstream projects.

The attributions for bbport, Supermedo, shadPS4, and the patches can be found in [GetLostIn's credits](https://github.com/GetLostIn/CTR-NitroFueled-PC#credits) and [OCTR's credits](https://github.com/Ryu7w7/OCTR-NitroFueled-PC#credits). Those pages also maintain their acknowledgments of other contributors, libraries, and PC tools.

GetLostIn and Ryu7w7 state in their respective credits that their contributions were developed with assistance from Claude by Anthropic. That attribution is retained when describing the original work.

Acknowledging components in the history of the PC port does not mean this PS4 adaptation includes all of its graphics features, Windows libraries, or options from newer releases.

## Tools used for PS4 and the builder

- **[OpenOrbis PS4 Toolchain](https://github.com/OpenOrbis/OpenOrbis-PS4-Toolchain)** and **[create-fself](https://github.com/OpenOrbis/create-fself):** tools for compilation and module preparation.
- **[GoldHEN](https://github.com/GoldHEN) and [GoldHEN Plugins SDK](https://github.com/GoldHEN/GoldHEN_Plugins_SDK):** the environment and references for module startup.
- **[maxton — LibOrbisPkg](https://github.com/maxton/LibOrbisPkg):** foundations for the package-reading and package-building tools used by the builder.
- **[LLVM/Clang](https://llvm.org/):** compilation and analysis tools.
- **[Unicorn](https://www.unicorn-engine.org/):** instruction and native-integration tests in a simulated environment.
- **[Python](https://www.python.org/)** and **[PowerShell](https://github.com/PowerShell/PowerShell):** automation and portable builder tools.

## PS4 adaptation and testing

**Trollfachender777**, with assistance from **AI**, for integrating this edition, the local builder, the L3+R3 menu and its settings, per-local-user identities, and tests performed on the development console.

Thanks to everyone who tested the project and shared feedback. The documented tests and features reflect the scope checked for this adaptation; they are not attributed to the authors of the upstream projects.

## Licenses and game rights

Third-party components retain their original notices and licenses. The builder ZIPs include their source code, license notices, and the attributions supplied with their components and tools. These credits do not replace those texts.

**Crash Team Racing: Nitro-Fueled**, its data, and its trademarks belong to their respective rights holders. Beenox, Activision, and Sony are not presented as authors or sponsors of this community adaptation.

No game files, updates, DLC, saves, or personal identities are included in this documentation.
