# libghost_rtsp

First-class **RTSP** receive library for [GhostVidStream](https://github.com/iHadAThought/GhostVidStream).

Same product bar as `libghost_ndihx`: native `ghost_rtsp.h` API, `media_core` plugin id `rtsp`, BGRX `capture_newest`, embed docs.

See `docs/embed.md`.

## Build

```bash
make
sudo make install
```

Requires FFmpeg shared libs.

## Hardening (2026-09-25)

ASan soak+reconnect on AIDA H.264 1080p30: **PASS** (Mac lab). Valgrind not available on macOS host.

Encode matrix: see `docs/srt-rtmp-rtsp-encode-compatibility.md`.

## License

Released under the [MIT License](LICENSE) — free to use, modify, and redistribute.
Copyright © 2026 Brendan Mahoney / iHadAThought.

## Related

- GhostVidStream: https://github.com/iHadAThought/GhostVidStream
- Companion: libghost_ndihx / libghost_srt / libghost_rtmp / libghost_rtsp
