# Goggles Artifacts

Prebuilt binary artifacts consumed by the Goggles build workflow are published from this repository.

## Repository Scope

- Versioned release assets for Goggles build dependencies
- Checksums and release notes for each published artifact
- Stable download URLs for Pixi/rattler package recipes

## Release Tags

| Artifact | Tag Pattern | Typical Asset |
| --- | --- | --- |
| wlroots | `wlroots-<version>` | `wlroots-<version>.tar.xz` |
| i686 sysroot | `sysroot-i686-<version>` | `sysroot-i686-<version>.tar.xz` |

## Consumer Repository

Main project: <https://github.com/goggles-dev/Goggles>

Current in-tree consumer references include:

- `packages/wlroots_0_19/recipe.yaml`
