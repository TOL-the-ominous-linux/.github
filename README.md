# The Ominous Linux (TOL)

> Linux, without the cheerful marketing.

**The Ominous Linux** — **TOL** — is the group behind
[camareLOL](https://github.com/TOL-the-ominous-linux/camareLOL) and the projects
that grow out of it. It is not a distribution and it has no company behind it.
It is a name for a way of building Linux tooling: state the risk, show the
evidence, and never claim a result that was not verified.

## Projects

### camareLOL

A safety-first TUI installer for Arch Linux, written in Rust. Discovery → plan →
review → confirm → execute → verify, with a safety gate in front of every
destructive operation. Vietnamese, English and Simplified Chinese.

- Repository: <https://github.com/TOL-the-ominous-linux/camareLOL>
- Releases: <https://github.com/TOL-the-ominous-linux/camareLOL/releases>
- npm: `@wenker-ai/camarelo` — the `beta` tag carries 1.x; `latest` is still
  0.1.22.
- It installs Arch Linux. It is not a distribution and does not ship a kernel.

### iLOL kernel

The kernel line that camareLOL may install when the stock Arch kernel is not
enough for a machine. Arch-based, delivered as normal Arch packages
(`linux-ilol`, `linux-ilol-headers`), opt-in and reversible.

**Status: planned. Nothing is built, packaged or shipped.** Home repository:
[TOL-the-ominous-linux/kernel](https://github.com/TOL-the-ominous-linux/ilol-kernel)
— the policy and the patch set live there; the definition is in
[camareLOL/tol/LOL-KERNEL.md](https://github.com/TOL-the-ominous-linux/camareLOL/blob/main/tol/LOL-KERNEL.md).

## Principles

1. **Say the dangerous thing first.** "This erases the disk" belongs before the
   write, not in a footer.
2. **Evidence or it did not happen.** A package name that passed unit tests but
   died in a VM is a bug, not a win.
3. **Re-identify before writing.** Hardware topology changes; a plan is a
   promise about a specific disk, not about "the disk".
4. **No updater in the binary.** The thing that installs the system is not the
   thing that replaces itself.
5. **A skipped gate is disclosed.** If a test was not run, the release notes say
   so.

## Naming

| Written | Means |
|---|---|
| `TOL`, `The Ominous Linux` | the group |
| `camareLOL` | the installer (one `m`, then `are`) |
| `iLOL kernel`, `linux-ilol` | the kernel line; package names use `linux-ilol` |
| `LOL` alone | avoid it outside this context; it reads as "laughing out loud" |

`camareLOL` is the spelling used by the binary, the npm package, tag names and
documentation. A local folder named `carameLOL` is a typo, not a second product.

## Brand

The mark is an eye split into black and red, with the letters `TOL`.

The eye follows the graphic language of the band **TOOL**. That is inspiration,
not a partnership, and the difference is written down:

> The TOL mark is inspired by the visual language of the band TOOL. TOL is not
> affiliated with, endorsed by, or connected to TOOL, its members or its
> management.

Keep that line wherever the mark is published. Before any commercial use —
hardware, paid support, a paid build — replace the mark. Full rules:
[camareLOL/tol/BRAND.md](https://github.com/TOL-the-ominous-linux/camareLOL/blob/main/tol/BRAND.md).

## Status

| Piece | State |
|---|---|
| Name, documents, brand rules | done, October 2026 |
| camareLOL 1.0.1 beta | published: GitHub pre-release, npm `beta` |
| GitHub organisation | pending; this repository moves into it and becomes the `.github` profile |
| iLOL kernel | not started; checklist empty on purpose |

## Contributing

There is no contributor programme yet. Issues and discussions for the installer
live in the camareLOL repository. If you want to work on the kernel line, read
the definition first: the constraints there are the project.

## License

GPL-3.0-or-later. See [LICENSE](LICENSE). The name "The Ominous Linux" and the
`TOL` wordmark are not licensed for endorsement of third-party products.
