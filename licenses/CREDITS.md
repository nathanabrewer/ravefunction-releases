# Credits

## Music

The songs bundled with the game, with their licences. In the game the same
credits are on Settings → Credits, and each song's source link and licence are
in its detail pane on the Songs tab. Every package (`songs/<id>.zip`) is pinned
by SHA-256 in `catalog/approved.json`; its rights record is
`catalog/rights/<id>.md`. For each song: level-matched (one fixed gain),
re-encoded to Ogg Vorbis, and mapped (Normal to Expert+) for the game, then
called Decision Rhythm, by the project's map generator; the covers are original artwork generated from
the audio. Store builds carry only the music the project owns (Astra / First
Light, last below); the other songs are in personal builds only.

- **“December”** by **Valya Kan** (Yarn Audio, YARN020, 2018).
  https://archive.org/details/yarn020 · Licensed under CC BY 4.0
  (https://creativecommons.org/licenses/by/4.0/).
- **“eat space with forced headroom”** by **Jukka-Pekka Kervinen**
  (unfoundsound, unfound91, 2017). https://archive.org/details/unfound91 ·
  Licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/).
- **“Express Shock”** by **Demonside** (Genetic Trance, GT290, 2011).
  https://archive.org/details/gt290Demonside-WelcomeToYourDestiny · Public
  domain (CC0 1.0, https://creativecommons.org/publicdomain/zero/1.0/),
  credited with thanks.
- **“Ruination”** by **Sciurid** (Illusory, Dwindle, 2018).
  https://archive.org/details/dwindle · Licensed under CC BY 4.0
  (https://creativecommons.org/licenses/by/4.0/).
- **“Laser Cut”** by **Sciurid** (Illusory, Secret Centre, 2020).
  https://archive.org/details/secretcentre · Licensed under CC BY 4.0
  (https://creativecommons.org/licenses/by/4.0/).
- **“AFAIK”** by **Sum-1** (Tobias Peterson; Togeo Music, Mechanical Monkeys,
  2008). https://archive.org/details/MechanicalMonkeys · Licensed under CC BY
  3.0 (https://creativecommons.org/licenses/by/3.0/).
- **“(Do Not Provoke) That Which Is Steel + Eyes + Mind”** by **Adhesion**
  (Evil Residence Records, Idiosyncratic Dance Music, 2007).
  https://archive.org/details/ER48idiosyncratic · Licensed under CC BY 3.0
  (https://creativecommons.org/licenses/by/3.0/).
- **“Astra / First Light”**: the project's original synthesized demo song and
  charts (no third-party material; described under Moon Rider below).

None of these artists endorse this game; their licences let anyone use the
music with credit.

## Software notices

`licenses/THIRD-PARTY-NOTICES.txt` lists all the third-party software in the
apps: which app carries what, each component's licence and source, and the
file with its full licence text. Every export carries the `licenses/` folder.
The same files are linked from the download page,
https://ravefunction.com/download/. In the game, Settings → Credits names each
component under the music.

## Godot Engine

Godot Engine 4.8 beta3, copyright (c) 2014-present Godot Engine contributors
and (c) 2007-2014 Juan Linietsky and Ariel Manzur, is used under the MIT
License (`licenses/godot-LICENSE.txt`). The libraries Godot includes
(FreeType, HarfBuzz, ICU, mbed TLS, ENet and others) are listed with their
licences in `licenses/godot-COPYRIGHT.txt`, Godot's own notices file for the
pinned engine commit.

## Other Rust crates

The native core also compiles in RustFFT, serde_json, glam and the crates they
use, each used under the MIT License (most offer MIT or Apache 2.0).
`licenses/rust-crates.txt` lists every crate with its version, source and MIT
text. `scripts/third-party-notices.py` writes that file from
`rust/Cargo.lock`, and `tests/notices_test.py` fails until it covers every
locked crate.

## Quest and Android components

On Quest, Godot OpenXR Vendors 5.2.0 (MIT, Godot XR contributors, built with
godot-cpp, MIT), the Khronos OpenXR loader (Apache 2.0) and Meta's OpenXR
headers (Oculus SDK License Agreement). In every Android app, AndroidX and
Kotlin (Apache 2.0) and libc++ from the Android NDK (Apache 2.0 with LLVM
Exceptions). The texts are in `licenses/THIRD-PARTY-NOTICES.txt` and
`licenses/apache-2.0.txt`.

## godot-rust native bindings

godot-rust 0.5.5, copyright godot-rust; Bromeon and contributors, is used under
MPL-2.0. Upstream source: https://github.com/godot-rust/gdext/tree/v0.5.5.
The local `godot-ffi` dependency adds visionOS constructor registration in
`src/shard_registry.rs`. Its complete modified source is provided in
`licenses/godot-ffi-0.5.5-source.zip` (also included in each app's resource pack),
and directly in `rust/vendor/godot-ffi/`. The license is provided in
`licenses/godot-rust-MPL-2.0.txt`. This dependency retains its MPL-2.0 license.

## Symphonia audio decoders (live radio)

Live radio decodes MP3, AAC-LC, Vorbis and FLAC with Symphonia 0.6.1
(crates `symphonia`, `symphonia-core`, `symphonia-common`,
`symphonia-metadata`, `symphonia-bundle-mp3`, `symphonia-codec-aac`,
`symphonia-codec-vorbis` and `symphonia-bundle-flac`), copyright the
Project Symphonia developers (Philip Deljanov and contributors), used
unmodified under MPL-2.0. Upstream source:
https://github.com/pdeljanov/Symphonia/tree/v0.6.1 (and crates.io). The
license is provided in `licenses/symphonia-MPL-2.0.txt`. Symphonia brings in
bitflags, bytemuck, lazy_static, log, regex-lite and smallvec, each under
MIT or Apache-2.0 (bytemuck also Zlib), unmodified. AAC is a patent-licensed
format; see apps/rhythm/docs/RADIO_PICKUP.md section 7 before shipping a
build that decodes it with its own decoder.

## qrcode (Operator links as QR codes)

The Operator app draws its party links as QR codes with the `qrcode` crate
0.14.1, copyright 2016 kennytm, used unmodified under the MIT License (it is
dual-licensed MIT OR Apache-2.0), without its optional image features.
Upstream source: https://github.com/kennytm/qrcode-rust (and crates.io). The
license is provided in `licenses/qrcode-MIT.txt`.

## Fonts: Archivo and IBM Plex Mono, SIL Open Font License 1.1

The menus use Archivo (copyright 2020 The Archivo Project Authors,
https://github.com/Omnibus-Type/Archivo) and IBM Plex Mono (copyright 2017
IBM Corp., https://github.com/IBM/plex), both under the SIL Open Font License
1.1, taken unmodified from https://github.com/google/fonts. The licences are in
`assets/fonts/Archivo-OFL.txt` and `assets/fonts/IBMPlexMono-OFL.txt`.

## Moon Rider (Supermedium), MIT License

Moon Rider (https://github.com/supermedium/moonrider) was used as a visual
reference. The items below come from it or are based on it:

| File in this project | Source in Moon Rider | Use |
|---|---|---|
| `models/beat.obj` | `assets/models/beat.obj` (unchanged) | Optional Neon note block mesh |
| `shaders/aurora.gdshader` | idea from `src/components/shaders/aurora.frag.glsl` / `aurora.vert.glsl` | Layered-sine aurora curtains, rewritten in Godot shader language |
| `scripts/space.gd`, `shaders/journey.gdshaderinc`, `shaders/track.gdshader` | techniques studied in `supercurve.js`, `supercurve-shader.js`, `curve-follow-rig-reset.js` | Original analytic path, rebased to its tangent with a stable play zone; ribbon geometry and song-clock travel |
| `shaders/ring.gdshader`, `shaders/tunnel.gdshader`, procedural meshes in `scripts/space.gd` | techniques studied in `ring.js` and `tunnels.js` | Repeated distance-aligned structures, fades and pooling principles; new native geometry and shaders |
| stars and laser instancing, phrase palette in `scripts/space.gd` | techniques studied in `stars.js`, `stage-lasers.js`, `stage-colors.js` | Original MultiMesh star/beam effects and beat/phrase colour response |

No Moon Rider textures, sounds, fonts or press-kit files are included. Apart from
the Godot sky-depth workaround credited below, every other shader, mesh and texture here (sky, planet, stars, dust, rings,
sabers, trail, cut effect, scoreboard, neon pylons, stage lasers, bombs,
walls, score pop-ups, menus, live-entity boxes) is original to this project
and generated in code.

All sounds (cut, bad cut, bomb, saber clash, miss, wall warning, UI click,
question chime) are synthesised at start-up by the Rust core
(`rust/src/sfx.rs`); no sample files are used.
The 0.4.1 solid note mesh (`scripts/note_mesh.gd`) is an original 44-triangle
cube with flat bevels. Its 85 ms unpitched cut transient is synthesized from
filtered noise; no commercial game recordings or geometry were used.

No proprietary game assets, code or designs are used. No APK, OBB or decompiled
files were read or included. Community-map compatibility is an original reader
of publicly documented data formats; source references are in
`docs/COMMUNITY_MAPS.md`. Imported maps and music remain their creators' work.

`songs/astra-first-light.zip` contains an original synthesised demonstration song
and two original charts, generated by `tests/make_community_fixtures.py`.
`icon.svg` is original vector artwork for Astra. Neither uses external assets.

```
The MIT License

Copyright © 2018 Supermedium.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```

## Foreman owner branding

The telephone receiver in `scripts/telephone.gd`, song placeholder in
`assets/song-placeholder.svg`, song-list layout and native speech adapter are
original work for this copy. They contain no Beat Saber or Beat Punch assets.
The start-up splash and the app icons in `assets/brand/` are the Rave Function
identity's ψ mark (the Mac app, Rave Function Operator, wears its Beat cut mark),
original work made by `scripts/make-brand-art.py` from `docs/brand/rave-function/`.
Foreman artwork remains connector branding.
Test cover images are generated fixture artwork. Live BeatSaver thumbnails are
fetched at runtime and are not redistributed as bundled app artwork.

`assets/foreman/brand-mark.svg` and `brand-app-icon.svg` are the owner's supplied
DFTZ Foreman marks, copied from `../docs/foreman-vr/brand/` for the requested Foreman
VR product direction. The current draft-3 brief replaces the earlier pixel hat
with this amber F hard hat and cyan signal arc. These owner-provided brand assets
are not part of Moonrider's MIT assets. The native job-site geometry and HUD layout
in this copy are original work.

## Godot visionOS depth workaround

The project also builds Godot 4.8 beta3 source with local visionOS viewport,
texture-lifetime, compositor-resume and hand-provider fixes in
`scripts/patches/godot-visionos-*.patch`. Godot remains
MIT licensed under the notice below. These modifications are original project
work; the pinned source and reproduction steps are recorded in `docs/BUILDING.md`.

`shaders/visionos_depth.gdshader` adapts the small sky-depth workaround from
[Godot's visionOS XR documentation](https://docs.godotengine.org/en/latest/tutorials/xr/visionos_intro.html).
Godot documentation code samples are MIT licensed. This writes distant depth
for Apple's compositor while leaving the existing sky color intact.

```
MIT License

Copyright (c) 2014-present Godot Engine contributors.
Copyright (c) 2007-2014 Juan Linietsky, Ariel Manzur.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```


The 0.5.5 native dashboard graph geometry, pace panel, environment preset JSON and
system-selection adapter are original project work. The existing Moonrider MIT
technique credit above continues to apply to the procedural journey. No commercial
game assets or designs were imported for these controls or themes.

## Default avatar: "Yarncrafted Ginger" (Meshy AI)

`assets/avatars/ginger/` is the project owner's own avatar, a knit-style
character with glasses, made by the owner with Meshy AI (https://www.meshy.ai)
on 2026-10-20 and rigged there with a Mixamo skeleton; downloaded rigged on
2026-11-18 and reduced to 1024 px JPEG textures for Quest (9,967 triangles,
42 bones). Used under the owner's Meshy plan terms (free-tier Meshy generations
are CC BY 4.0: credit Meshy).
