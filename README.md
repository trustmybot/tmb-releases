# tmb releases

Release files for [tmb](https://github.com/trustmybot/tmb). This repo holds compiled files, install scripts and the licence only: no source and no issues. Report issues on [trustmybot/tmb](https://github.com/trustmybot/tmb/issues).

## Channels

Each channel installs as a program of its own name, so channels live side by side on one machine, and each keeps itself up to date on its own channel.

| Channel | Program | Release | For |
|---|---|---|---|
| stable | `tmb` | Normal releases, tagged `vX.Y.Z`. The newest is "latest". | Everyday use. |
| rc | `tmb-rc` | Prereleases tagged `vX.Y.Z-rc.N`. | Trying the next release before it ships. |
| dev | `tmb-dev` | The rolling prerelease `dev`, replaced on every merge to tmb's base branch. | Following development day to day; it may break. |

No stable or rc release is out yet. Until v1.0.0, only the dev channel installs.

## Install

Pick the channel with `TMB_CHANNEL`. The install needs no login. Run the same command again to upgrade.

### stable

macOS and Linux:

```sh
curl -fsSL https://github.com/trustmybot/tmb-releases/releases/download/dev/install.sh | TMB_CHANNEL=stable sh
```

Windows, in PowerShell:

```powershell
$env:TMB_CHANNEL = 'stable'; irm https://github.com/trustmybot/tmb-releases/releases/download/dev/install.ps1 | iex
```

### rc

macOS and Linux:

```sh
curl -fsSL https://github.com/trustmybot/tmb-releases/releases/download/dev/install.sh | TMB_CHANNEL=rc sh
```

Windows, in PowerShell:

```powershell
$env:TMB_CHANNEL = 'rc'; irm https://github.com/trustmybot/tmb-releases/releases/download/dev/install.ps1 | iex
```

### dev

macOS and Linux:

```sh
curl -fsSL https://github.com/trustmybot/tmb-releases/releases/download/dev/install.sh | TMB_CHANNEL=dev sh
```

Windows, in PowerShell:

```powershell
$env:TMB_CHANNEL = 'dev'; irm https://github.com/trustmybot/tmb-releases/releases/download/dev/install.ps1 | iex
```

### One exact release

`TMB_INSTALL_VERSION=1.0.0` in place of `TMB_CHANNEL` installs that one rc or stable release as `tmb-1.0.0`. It never updates itself.

## Then

Inside a project, run the program you installed: `tmb init`, `tmb-rc init` or `tmb-dev init`. Setup, updates and removal are in [tmb's reference](https://github.com/trustmybot/tmb/blob/dev/docs/reference/README.md).

## Licence

[Functional Source License 1.1, Apache 2.0 future license](LICENSE.md).
