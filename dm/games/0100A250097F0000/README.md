<!-- PEANUTS begin: Android bring-up profile. -->
# DRAGON BALL FIGHTERZ

## Build and content

- Title `0100A250097F0000`, base version `1.0.0` (`v0`) only; later title updates are not yet profiled.
- Main `af996c8a822d1e8b902d91ed4019852d`, `subsdk0` (`NintendoSDK_movie`) `303578054faefc2198114b62e408c498`, `sdk` `e01ad5381c948c4ec3b0bb210b08d5c8`, Nintendo SDK 4, Unreal Engine 4.18 (Arc System Works RED) on NVN.
- `sys_resource = 0x0` and `mem_used = 0x8000000` accommodate the ~78 MB rewritten module and `.bss` footprint on a `0xCD500000` app pool. `tex_flush_upload` and `tex_dirty_upload` are enabled for UE4 CPU-written textures.
- `shader_split.py` extracts 10,679 shaders (7,858 pixel, 2,546 vertex, 272 compute, 3 geometry) and 2,546 vertex/pixel variation pairs from `RED/Content/Paks/pakchunk0-Switch.pak`.

## Drivers tested

- **Mr. Purple Turnip T30 (Vulkan):** Boots cleanly through menus and gameplay with no missing shaders or graphical issues.
- **System driver:** Not tested.

## Network and offline behaviour

- Offline mode does not work; the title fails to advance past its initial network/lobby sign-in step without connectivity.

## Frame rate behaviour

- Runs locked at **60 FPS** in menus and gameplay on Mr. Purple Turnip T30.

<!-- PEANUTS end -->
