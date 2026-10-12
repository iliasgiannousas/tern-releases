# Tern releases

This repository holds **Tern's release binaries only**. It is the public feed
that an installed Tern reads to update itself; the source code lives in a
private repository and is not published here.

Every release carries four assets:

| Asset | Platform |
| --- | --- |
| `tern-linux-amd64` | Linux, x86-64 |
| `tern-linux-arm64` | Linux, arm64 |
| `tern-windows-amd64.exe` | Windows 10/11, x86-64 (GUI subsystem: no console window) |
| `SHA256SUMS` | SHA-256 of the three binaries above |

Download the file for your platform, `chmod +x` it on Linux, and run it. Tern
checks this repository for a newer release at most once a day and installs it
only after you confirm; it verifies the download against `SHA256SUMS` before
replacing itself.

Check a download yourself:

```sh
sha256sum -c SHA256SUMS --ignore-missing
```

No source code, issues or pull requests are accepted here — the binaries are
build outputs of the private repository.

The in-app release history is under the **Changelog** button in Tern.
