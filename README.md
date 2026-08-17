[update-readmes]   Mode: rewrite — migrating to template structure...
# incus-box

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/incus-linux-toolkit) [![KDE Eco](https://img.shields.io/badge/KDE%20Eco-certified-brightgreen?logo=kde&logoColor=white&style=flat-square)](https://eco.kde.org/) [![Blue Angel](https://img.shields.io/badge/Blue%20Angel-DE--UZ%20215-0055a4?style=flat-square)](https://www.blauer-engel.de/en/certification/criteria) [![Energy](https://api.green-coding.io/v1/ci/badge/get?repo=Interested-Deving-1896%2Fincus-linux-toolkit&branch=main&workflow=eco-audit.yml)](https://metrics.green-coding.io/ci-index.html)


<!-- AI:start:what-it-does -->
`incus-box` is a distrobox-inspired tool that uses [Incus](https://github.com/lxc/incus) instead of
Docker or Podman as the container runtime. It lets you use any Linux distribution inside your
terminal with tight host integration: shared HOME, X11/Wayland, audio, GPU, and USB passthrough.

Unlike distrobox, `incus-box` supports the full Incus workload spectrum:

| Workload | Backend | Use case |
|---|---|---|
| **System containers** | LXC (default) | Distro environments, dev boxes, services |
| **Virtual machines** | KVM / QEMU | Full kernel isolation, Windows, Talos, winesapOS |
| **OCI containers** | OCI runtime | Docker-compatible images via `docker:` prefix |

This means you can run an Ubuntu dev container, a Fedora VM, and a Docker image side by side
under the same `incus-box` interface.
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
_Architecture documentation pending._
<!-- AI:end:architecture -->

## Install

```bash
git clone https://github.com/Interested-Deving-1896/incus-linux-toolkit.git
cd incus-linux-toolkit
sudo ./incusbox/install          # system-wide
# or
./incusbox/install --user        # ~/.local (no root)
```

The installer creates `incus-box` and all `incus-box-*` subcommand symlinks in your `$PATH`.
It also installs a `incusbox` → `incus-box` compatibility symlink so existing scripts and
muscle memory continue to work.

### Rename note

This repository was previously named `incusbox` and the command was `incusbox`.
Both have been renamed to `incus-box` for consistency with the `incus-*` ecosystem naming
convention. The old name redirects automatically on GitHub. The installer provides the
`incusbox` compatibility symlink for a smooth transition.

## Usage

<!-- Add usage examples here. This section is yours — the AI will not modify it. -->

## Configuration

<!-- Document configuration options here. This section is yours — the AI will not modify it. -->

## CI

<!-- AI:start:ci -->
_CI documentation pending._
<!-- AI:end:ci -->

## Mirror chain

<!-- AI:start:mirror-chain -->
This repo is maintained in [`Interested-Deving-1896/incus-linux-toolkit`](https://github.com/Interested-Deving-1896/incus-linux-toolkit) and mirrored through:

```
Interested-Deving-1896/incus-linux-toolkit  ──►  OpenOS-Project-OSP/incus-linux-toolkit  ──►  OpenOS-Project-Ecosystem-OOC/incus-linux-toolkit
```

Changes flow downstream automatically via the hourly mirror chain in
[`fork-sync-all`](https://github.com/Interested-Deving-1896/fork-sync-all).
Direct commits to OSP or OOC are detected and opened as PRs back to `Interested-Deving-1896`.
<!-- AI:end:mirror-chain -->

## Contributors

<!-- AI:start:contributors -->
_Contributors pending._
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->

Original project — Incus-backed distrobox replacement using any Linux distro in the terminal via Incus containers.

| Origin | Host | Fork in I-D-1896 |
|--------|------|-----------------|
| [lxc/incus](https://github.com/lxc/incus) | GitHub | ✅ |
| [89luca89/distrobox](https://github.com/89luca89/distrobox) | GitHub | ✅ |
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
| File | Description |
|---|---|
| [dep-graph/origins.md](https://github.com/Interested-Deving-1896/incus-linux-toolkit/blob/main/dep-graph/origins.md) | Dependency graph (Markdown table) |
| [config/gitlab-subgroups.yml](https://github.com/Interested-Deving-1896/incus-linux-toolkit/blob/main/config/gitlab-subgroups.yml) | GitLab subgroup map |
<!-- AI:end:resources -->

<!-- AI:start:accessibility -->
This repo uses automated accessibility auditing via `check-accessibility.yml`.

Checks include: CODEOWNERS ownership coverage, README screen-reader compatibility,
WCAG 2.1 AA HTML compliance, audio overview (espeak-ng), and Braille output (liblouis).




Run the [Check Accessibility](https://github.com/Interested-Deving-1896/incus-linux-toolkit/actions/workflows/check-accessibility.yml)
workflow to generate the first report and accessibility artifacts.
See [DOCS/accessibility.md](https://github.com/Interested-Deving-1896/incus-linux-toolkit/blob/main/DOCS/accessibility.md) for the full reference.
<!-- AI:end:accessibility -->

## License

<!-- AI:start:license -->
[GPL-3.0](https://github.com/Interested-Deving-1896/incus-linux-toolkit/blob/main/LICENSE) © 2026 [Interested-Deving-1896](https://github.com/Interested-Deving-1896)
<!-- AI:end:license -->
