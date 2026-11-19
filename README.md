# tmb releases

Release files for tmb. This repo holds compiled files, install scripts and the licence only: no source and no issues.

## Install (dev channel)

macOS and Linux:

```sh
curl -fsSL https://github.com/trustmybot/tmb-releases/releases/download/dev/install.sh | sh
```

Windows (PowerShell):

```powershell
irm https://github.com/trustmybot/tmb-releases/releases/download/dev/install.ps1 | iex
```

Then, inside a project: `tmb setup`.

## Channels

| Channel | Release |
|---|---|
| dev | The rolling prerelease `dev`, replaced on every merge to the base branch. |
| rc | Prereleases tagged as release candidates. |
| stable | Normal releases. The newest is "latest". |

## Licence

[Functional Source License 1.1, Apache 2.0 future license](LICENSE.md).
