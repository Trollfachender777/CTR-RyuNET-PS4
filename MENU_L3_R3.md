# L3+R3 settings guide

**Version scope:** sections 1–9 describe the original settings supplied by the unchanged public builders. The separate [v1.2.1 PS4 update](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/tag/v1.2.1) keeps those approved settings and adds the server-friends, invitations and network screens described in section 10. Update an existing installation without converting the game again; see the release for compatibility and installation instructions.

Press **L3 and R3 together** to open **RyuNET - PS4 Settings** in English or **RyuNET - Ajustes PS4** in Spanish. Press **Circle** to return to the game.

The paths below use the English labels. If you installed the Spanish edition, use these equivalents as they appear in its module:

| English | Spanish module label |
| --- | --- |
| FPS and graphics | FPS y graficos |
| FPS limit / Unlimited | Limite de FPS / Sin limite |
| Graphics / Internal resolution | Graficos / Resolucion interna |
| Native / Next / Apply | Nativa / Siguiente / Aplicar |
| Selected / Saved | Elegida / Guardada |
| More options / Effects and shadows | Mas opciones / Efectos y sombras |
| Motion blur / Enable / Disable | Desenfoque / Activar / Desactivar |
| Dynamic shadows | Sombras dinamicas |
| Remove shadows / Restore shadows | Quitar sombras / Restaurar sombras |
| Restore graphics / Restore | Restaurar graficos / Restaurar |
| Friends / My nickname | Amigos / Mi apodo |
| Change nickname / Add friend | Cambiar apodo / Anadir amigo |
| View / remove / View list | Ver / eliminar / Ver lista |
| Remove friend | Eliminar amigo |

## 1. Choose an FPS cap

Open **FPS and graphics → FPS limit → 30 / 60 FPS** and select **30 FPS** or **60 FPS**. Confirm and return to the game.

**What it does:** sets an actual frame-rate cap. The change takes effect when you return to the game, without restarting it. Choosing 60 does not guarantee that the console can reach exactly 60 FPS on every track or in every situation.

To remove this cap, return to **FPS limit** and choose **Unlimited**.

**What it does:** removes this module's frame-rate limit. It may increase load and power use; it does not ensure that the console or display can show more frames.

## 2. Change the internal resolution

Open **FPS and graphics → Graphics → Internal resolution**. Press **Next** until **Selected** shows **Native**, **720p**, or **480p**. Press **Apply**, close the application normally, and relaunch it.

**What it does:** changes the resolution used to draw the 3D scene. Native keeps the native profile's resolution; 720p and 480p reduce detail and may reduce GPU load. The 720p profile also keeps motion blur disabled.

Your TV may still report **1080p** because that is the HDMI output signal. It does not mean the 3D scene is still rendered at 1080p. Menus and loading screens may not lose sharpness in the same way.

**Saved** shows the stored setting; **Selected** shows the option you are browsing. Pressing Circle before applying keeps the previous setting. This option preserves your FPS cap and shadow preference.

## 3. Adjust motion blur

Open **FPS and graphics → Graphics → More options → Effects and shadows → Motion blur**. Choose **Enable** or **Disable**, save, close the game, and relaunch it.

**What it does:** lets you keep or remove the blur associated with movement. Native and 480p use your preference; the 720p profile keeps it disabled.

## 4. Adjust dynamic shadows

Open **FPS and graphics → Graphics → More options → Effects and shadows → Dynamic shadows**. Choose **Remove shadows** to disable them or **Restore shadows** to bring them back. Close and relaunch the game after saving.

**What it does:** reduces the work required for supported dynamic shadows, including racers' shadows. Lighting remains enabled. Shadows painted into textures may remain visible; not every dark area on a track is a dynamic shadow.

## 5. Restore graphics

Open **FPS and graphics → Graphics → More options → Restore graphics**, choose **Restore**, and restart the application.

**What it does:** returns to Native with motion blur and dynamic shadows enabled. It preserves your FPS cap, save data, nickname, and contacts.

## 6. Change your nickname

Open **Online → My nickname → Change nickname**. Enter your new nickname, confirm, close the game, and relaunch it.

**What it does:** changes the name used for RyuNET. It does not change your PSN account name. A different nickname may correspond to another server profile, so your friends will need to add the new name. Your local save is preserved.

## 7. Add a friend

Open **Online → Friends → Add friend**, enter their exact RyuNET nickname, and confirm. Use the name that person configured in RyuNET, rather than their Discord or PSN name. After saving, exit the settings and re-enter **Online** to refresh the list.

**What it does:** saves the contact in your list. Adding a contact does not create a lobby or send an invitation. To make it easier to find each other, both players should save each other's nicknames.

## 8. View your list or remove a contact

Open **Online → Friends → View / remove**. Choose **View list** to see your saved nicknames or **Remove friend** to remove a contact from your list.

**What it does:** lets you review and manage your own contacts. Removing someone from your list does not guarantee that you disappear from the list stored by their client.

## 9. Join a game

Exit L3+R3 settings, open **Online → Friends** in CTR's original menu (**Amigos** if the game is in Spanish), and select the contact. The other player must be online and in a compatible lobby with free slots, before the race starts.

**What it does:** uses CTR's own joining interface. The duplicate **Join friend** option was removed from L3+R3; managing contacts and joining a lobby are separate actions.

Joining compatible PC clients' private and public lobbies has been tested. The same result has not been demonstrated on every network. The original public-builder module does not implement invitations. With the separate v1.2.1 update, use the RyuNET invitations screen described below; the original PSN invitation dialog is not replaced.


## 10. Server friends and invitations in v1.2.1

Install the [separate PS4 update](https://github.com/Trollfachender777/CTR-RyuNET-PS4/releases/tag/v1.2.1) on a compatible installation, close CTR normally and reopen it. The English and Spanish converter ZIPs remain unchanged.

Enter Online, then open **L3+R3 → Online → Friends → View / remove → View list → Server friends**. Use **List / invite** to review accepted friends, or **Requests and extras → Incoming requests** to accept or decline requests. Use the other player's exact RyuNET nickname and a compatible current client. New friendships require that player's acceptance; a saved local contact alone is not an accepted server friendship.

**What it does:** reads and manages the shared RyuNET friends service. Previous local contacts stay on disk and are submitted as requests when needed. The server screens can inspect up to 200 accepted friends; CTR's original Friends list keeps its existing 32-contact compatibility limit. Wait for the server response before reopening the original CTR list.

Use **Invitations / network** in the server-friends menu to review incoming invitations and explicitly accept one, or to view room ping. Send invitations through the RyuNET **List / invite** screen while the relevant player and lobby are available. The game's original PSN invitation dialog is not replaced.

**What it does:** uses the selected friends, invitation, relay and ping protocols adapted from OCTR v0.6.4. It does not add the PC mod manager, desktop launcher or every PC-specific feature. Successful download/restart and Online on the reference console do not establish every cross-network combination.

For later PS4 updates, open **L3+R3 → Online and extras → PS4 updates → Check for updates → View result**. Confirm an available update, wait for **Update prepared**, close CTR normally and reopen it. Spanish labels are **Online y extras → Actualizaciones PS4 → Buscar actualizaciones → Ver resultado → Actualizar ahora**.

## 11. Automatic season events in v1.2.1

The module reads the active event from RyuNET in the background and applies it when the next track loads. No extra menu switch or replacement game assets are needed.
