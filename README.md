# {{crate_name}}
#### TAGLINE-REPLACE
[![crates.io](https://img.shields.io/crates/v/{{crate_name}}.svg)](https://crates.io/crates/{{crate_name}})
[![docs.rs](https://docs.rs/{{crate_name}}/badge.svg)](https://docs.rs/{{crate_name}})
[![tests](https://github.com/libcala/{{crate_name}}/workflows/tests/badge.svg)](https://github.com/libcala/{{crate_name}}/actions?query=workflow%3Atests)
[![changelog](https://img.shields.io/badge/changelog-green.svg)](https://github.com/libcala/{{crate_name}}/blob/master/CHANGELOG.md)

## Targets
Targets that are marked are currently *supported*, the rest are *planned*.
Targets in **bold** are preferred for that platform.  Targets not listed are
(mostly) similar to the ones listed, so bug reports and PRs can still be opened
for them.  This list is based on how
[cargo-cala](https://github.com/libcala/cargo-cala) builds distribution
packages, so it may seem a little weird.

### Android
- [ ] APK / AAB (Android App Bundle)
  - [ ] **aarch64-linux-android** (APK: `/lib/arm64-v8a/`)
  - [ ] armv7-linux-androideabi, **thumbv7neon-linux-androideabi** (APK:
    `/lib/armeabi-v7a/`)
  - [ ] **i686-linux-android** (APK: `/lib/x86/`)
  - [ ] **x86\_64-linux-android** (APK: `/lib/x86_64/`)

### BSD Variants
- [ ] **i686-unknown-freebsd** (32-bit FreeBSD App)
- [ ] **x86\_64-unknown-freebsd** (64-bit FreeBSD App)
- [ ] **x86\_64-unknown-netbsd** (64-bit NetBSD App)

### Fuchsia
- [ ] **aarch64-fuchsia** (Fuchsia for ARM App)
- [ ] **x86\_64-fuchsia** (Fuchsia for X86 App)

### iOS
- [ ] iOS App
  - [ ] **aarch64-apple-ios**
  - [ ] **x86\_64-apple-ios**

### Linux Variants
- [ ] Flatpak
  - [ ] **x86\_64-unknown-linux-gnu** (arch: /x86_64/)
  - [ ] **i586-unknown-linux-gnu** (arch: /i386/)
  - [ ] **aarch64-unknown-linux-gnu** (arch: /aarch64/, Raspberry Pi 4)
  - [ ] armv7-unknown-linux-gnueabihf, **thumbv7neon-unknown-linux-gnueabihf**
    (arch: /arm/, Raspberry Pi 2-3)
- [ ] **arm-unknown-linux-gnueabihf** (Raspberry Pi Zero W Program)
- [ ] **riscv64gc-unknown-linux-gnu** (Risc-V Linux Program)

### MacOS
- [ ] **x86\_64-apple-darwin** (MacOS App)

### Redox
- [ ] **x86\_64-unknown-redox** (Redox App)

### Web
- [ ] Static Web App
  - [ ] wasm32-unknown-emscripten, **wasm32-unknown-unknown**
  - [ ] **asmjs-unknown-emscripten** (fallback)
- [ ] **wasm32-wasi** (WASI App)

### Windows
- [ ] i586-pc-windows-msvc, i686-pc-windows-msvc, **i686-pc-windows-gnu**
  (32-bit Windows App),
- [ ] **x86\_64-pc-windows-gnu**, x86\_64-pc-windows-msvc (64-bit Windows App)

Template to use for libcala libraries: cargo generate --git https://github.com/libcala/lib_template
