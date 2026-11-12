# Changelog

All notable changes to the Rocscience FastWpfGrid fork are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-11-12

### Changed

- Forked [CodingConnected.FastWpfGrid](https://github.com/CodingConnected/CodingConnected.FastWpfGrid) tag `v1.1.0` (`c74d436232cf512dfacbc25147cea885f5c8e20c`). Package ids are `Rocscience.FastWpfGrid` and `Rocscience.WriteableBitmapEx.Wpf`. Namespace and assembly names stay `CodingConnected.FastWpfGrid` and `CodingConnected.WriteableBitmapEx.Wpf`.
- This fork targets `net9.0-windows`. Upstream 1.1.0 targeted `net10.0-windows`.
- `OnDpiChanged` runs the same DPI rebuild as a resize, so a monitor move that does not change the window size still recreates the bitmap and glyph cache.
- `SizeColumnsToContent` (default true) can open every column at the default width. Drags still stick, using the widths v1.1.0 already stores. A double-click auto-fit keeps that one column off the uniform width.
- Text that does not fit a cell is painted with an ellipsis. Measurement and the trimmed-cell tooltip still use the full string.
