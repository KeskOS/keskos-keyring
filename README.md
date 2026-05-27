# keskos-keyring

`keskos-keyring` is currently a placeholder package reserved for the future KeskOS pacman signing keyring.

## What this is

This repository keeps the package name and install target in place so signed-repo support can be introduced later without renaming packages or changing installer logic again.

## Role in KeskOS

Pacman keyring package.

## Package name

```txt
Package: keskos-keyring
Repo: [keskos]
Architecture: any
```

## What it installs or provides

- Installs package documentation under `/usr/share/doc/keskos-keyring/README.md`.
- Installs a placeholder marker under `/usr/share/pacman/keyrings/keskos-placeholder`.
- Does not yet ship real public keys or trust database files.

## Commands and launchers

- This package does not install commands or GUI launchers.

## Config, logs, and state

- This placeholder package does not generate logs or systemd units.
- Real pacman key material is intentionally not present yet.

## Dependencies

- No runtime dependencies are declared.
- Build with `makepkg -s --noconfirm`.

## Build

```bash
makepkg -s --noconfirm
```

## Packaging notes

- Keep the package name reserved so the future signed keyring can replace this placeholder cleanly.
- Do not document this as a complete signing solution until real key material is added.

## Troubleshooting

- If you are debugging package signing, remember this package is still only a placeholder and will not fix signature-verification problems on its own.

## Docs website export notes

- Docs site usage: placeholder notice and future signing-roadmap pointer.
