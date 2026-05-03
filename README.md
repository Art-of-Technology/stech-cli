# stech-cli

Public release distribution for [**stech**](https://www2.stech.com) — the
control plane for AI agents.

This repo hosts the **binaries**. The CLI source code lives in the (currently
private) [Art-of-Technology/stech.com](https://github.com/Art-of-Technology/stech.com)
monorepo and is published here on each `v*` tag via cross-repo release.

## Install

```bash
# macOS / Linux
curl -fsSL https://www2.stech.com/install.sh | sh

# Windows (PowerShell)
irm https://www2.stech.com/install.ps1 | iex

# Homebrew (mac + linux) — coming v0.1.x
brew install Art-of-Technology/stech/stech
```

The install scripts detect your OS/arch, fetch the matching archive from the
[Releases](https://github.com/Art-of-Technology/stech-cli/releases) page,
verify SHA-256 against the published `checksums.txt`, and drop the binary on
your PATH (`~/.local/bin` on Unix, `%LOCALAPPDATA%\stech\bin` on Windows).

Override the install dir with `STECH_PREFIX`; pin a version with `STECH_VERSION`.

## Manual install

If you'd rather not pipe a script into your shell, grab the right archive from
the latest [release](https://github.com/Art-of-Technology/stech-cli/releases/latest)
and extract `stech` (or `stech.exe`) onto your PATH yourself. Verify the
SHA-256 against `checksums.txt` from the same release.

## License

Apache-2.0 — see [`LICENSE`](./LICENSE).
