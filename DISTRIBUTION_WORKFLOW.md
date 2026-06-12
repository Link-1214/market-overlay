# Distribution Workflow

## Repository split

- `market-overlay-private`: source code, tests, build scripts, internal docs, and mirrored release artifacts.
- `market-overlay`: public distribution only. Keep installers, public user guides, patch notes, release notes, and checksums here.

## Release archive policy

1. Build and verify the installer from the private source repo.
2. Copy the final installer and public docs into `releases/vX.Y/` in both repos.
3. Generate `SHA256SUMS.txt` for each archived folder.
4. Confirm the public repo does not contain `.py`, tests, build scripts, owner-only notes, or personal data.
5. Create or update the GitHub release asset from the public repo.

## Older versions

The v1.8 and older folders are reconstructed from local release archives. They are kept for download/history convenience and should not be treated as full source history.
