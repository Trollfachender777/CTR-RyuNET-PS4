# PS4 v1.2.0 — OCTR 0.6.4 network candidate

This is the PS4 module candidate published for console validation. The existing builder release is separate. A successful build and emulation do not establish real-console interoperability: the new download, restart, Online and cross-network friend/invitation flow still need to be tested on PS4.

## Changes adapted to native PS4

- OCTR v0.6.4 regional relay discovery, registration, nearest responsive relay selection, and server fallback for older peers.
- Peer ping capability and RYUPN1 request/reply packets, with a room ping screen. Control packets are consumed before CTR receives gameplay traffic.
- The current RyuNET server friends protocol: request, accept, decline, remove and invite; incoming invitations can be explicitly accepted through the existing native session bridge.
- X-RyuNET-Proof HMAC-SHA256 requests with independent local-user installation identities, unique nonces, server Date clock correction and bounded background HTTP. No network request waits on the controller/render thread.
- Existing Online, original CTR joining, nickname, 30/60/unlimited FPS, Nativa/720p/480p, blur, dynamic shadows, graphics reset and confirmed updater permission fix are retained.

## Test on an installation with the working updater

1. Open **L3+R3 → Online and extras → PS4 updates → Check for updates → View result** (Spanish: **Online y extras → Actualizaciones PS4 → Buscar actualizaciones → Ver resultado**).
2. Confirm **Update now / Actualizar ahora** for **v1.2.0**. Wait for **Update prepared / Actualizacion preparada**.
3. Close CTR normally from the PS menu and reopen it. Verify Online and the v1.2.0 L3+R3 menu.
4. Enter Online before testing server friends. **Friends → View / remove → View list → Server friends** opens the new service. Use **List / invite**, or **Requests and extras → Incoming requests**. Invitations and room ping are under **Invitations / network**.
5. New friendships require acceptance by the other player using a compatible current client. Previous local contacts stay on disk and are submitted as requests when needed. Wait for the server response, then reopen CTR's Friends list. The original CTR list retains its existing 32-contact compatibility limit; the server screens can inspect up to 200 accepted friends.

This candidate adds individual invitations in L3+R3. It does not replace the original PSN invitation dialog; use the RyuNET menu to send an invitation. PC moderation/report, search, privacy and desktop/mod-loader interfaces are not exposed by this PS4 candidate. Windows/Linux launcher and renderer-specific fixes do not apply to the native PS4 executable. This is an adaptation of the named network components, not a claim of complete PC UI/feature parity.

## Preservation and scope

The updater downloads only the selected language module, verifies size, SHA-256 and SELF compatibility, writes replacement and rollback files with executable 0755 permissions, and applies it on the next normal startup. It does not change the official PC client, the builder packaging engine, game/DLC assets, saves, installation keys or profile settings. CPU experiments, lightweight scenery and the Dark model are not included.

`source.zip` contains the corresponding native module sources and build/test scripts in ES and EN, upstream reference/provenance, GPL license and notices. It contains no game, update, DLC, private profile, save or installation key. Building the module requires the same OpenOrbis/LLVM toolchains as the source builder: set `CTR_LLVM_BIN` and `OO_PS4_TOOLCHAIN`, place the GoldHEN SDK CRT at the path used by `build_native_module.py`, and run that script in the chosen language directory. The generated native profile headers are included; native executable fixture tests require the user's own compatible game images and are not included as assets.

## Credits

Ryu7w7 and OCTR/RyuNET contributors for the upstream PC runtime and network protocols; GetLostIn, SacredFire, bbport, shadPS4, OpenOrbis and GoldHEN authors for the work acknowledged in the project. PS4 adaptation and integration by Trollfachender777 with AI assistance. Existing upstream notices and licenses remain applicable.

Upstream reference: https://github.com/Ryu7w7/OCTR-NitroFueled-PC/tree/v0.6.4 (commit ac73258dfee67263657b0722faf2262d40bea826).
