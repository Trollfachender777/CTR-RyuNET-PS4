# PS4 update channel v1.1.0

These files provide v1.1.0 to compatible PS4 updaters. The GitHub release and builder ZIPs remain drafts during console validation. The channel files themselves are public.

`ctr_online_es.prx` and `ctr_online_en.prx` contain only the RyuNET port modules. Their exact corresponding source, build instructions, licenses, and upstream notices are included in `source.zip`. No game assets, saves, player identities, or account credentials are included.

The parent `stable.json` is the console update feed. A compatible updater detects the version and downloads its language module only after the player chooses **Update now**. The verified module takes effect after a normal game restart. Older installations need the one-time updater setup first.
