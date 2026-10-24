# PS4 update channel v1.1.0 — permissions-r2

This candidate fixes module execution permissions after an accepted update.
Both the replacement and rollback copy are explicitly set to mode 0755 before
syncing and committing. Failure to set permissions aborts the update.

The modules and corresponding source are public for console validation. The
GitHub release and builder ZIPs remain drafts. No game assets or player data
are included. Existing PS4 settings and identities are preserved.
