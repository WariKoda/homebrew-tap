# WariKoda Homebrew tap

Homebrew casks for [drift](https://github.com/WariKoda/drift), a terminal tool that diffs a local
project against a server and syncs only the changes you approve, over SFTP, FTP or FTPS.

## Install

```bash
brew install warikoda/tap/drift
```

Update with `brew upgrade drift`, remove with `brew uninstall drift`.

drift needs Git at runtime.

## How the cask is maintained

The release workflow of [WariKoda/drift](https://github.com/WariKoda/drift) updates
`Casks/drift.rb` with GoReleaser for every release. Do not edit the file by hand; the next
release overwrites it. Prereleases such as `-alpha` or `-rc` tags do not update the cask.

The macOS binaries are not signed. The cask removes the quarantine attribute after installing,
so Gatekeeper does not block drift.

Report problems with the cask in the [drift issue tracker](https://github.com/WariKoda/drift/issues).
