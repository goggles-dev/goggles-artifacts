# Goggles Artifacts

Prebuilt binary artifacts and project documents consumed by or produced alongside the Goggles build workflow.

## Repository Scope

- Versioned release assets for Goggles build dependencies
- Checksums and release notes for each published artifact
- Stable download URLs for Pixi/rattler package recipes
- OpenSpec design documents and change proposals

## Release Tags

| Artifact | Tag Pattern | Typical Asset |
| --- | --- | --- |
| wlroots | `wlroots-<version>` | `wlroots-<version>.tar.xz` |
| i686 sysroot | `sysroot-i686-<version>` | `sysroot-i686-<version>.tar.xz` |

## Published Releases

- <https://github.com/goggles-dev/goggles-artifacts/releases>

Current tags:

- `wlroots-0.19.2`
- `wlroots-0.18.3`
- `sysroot-i686-2.31.0`

## OpenSpec

`openspec/` contains design specs and change proposals for Goggles. Moved from the main repository to keep the source tree focused on code.

- `openspec/specs/` — module-level specifications
- `openspec/changes/` — feature proposals and archived changes

## Consumer Repository

Main project: <https://github.com/goggles-dev/Goggles>

Current in-tree consumer references include:

- `packages/wlroots_0_19/recipe.yaml`
