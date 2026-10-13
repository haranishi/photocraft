# Tool-options drag comparison (#5052)

These PNGs show PhotoCraft's own UI over a synthetic white 64 × 48 document.
Both use English, the Studio theme and a 1280 × 720 offscreen viewport.
Hardness starts at 50%, and a 20-point horizontal caption drag changes it to 70%.
Opacity is 100% in both images.

- `before.png`: main `6f85054288a564f9fbbccb99268ffdb34e581584`.
  Caption text becomes selected while Hardness changes.
- `after.png`: `06f7251e355ef209b26cfc189d6db859b8a79d9d`.
  Hardness changes without selecting the caption.

The captures use actual egui events and the offscreen wgpu renderer.
The after capture also checks that rendering preserves brush state and the
single journal entry from the drag. Native OS and tablet events are unverified.

## License and attribution

Original captures and the synthetic document are contributed under MIT OR
Apache-2.0; the adjacent `LICENSE-MIT` and `LICENSE-APACHE` contain those licenses.
The rendered PhotoCraft UI retains its project and bundled-asset notices in
[`NOTICE`](../../../NOTICE) and [`ATTRIBUTION.md`](../../../ATTRIBUTION.md).
Fonts and icons retain the licenses listed there.

## PNG SHA-256

- `before.png`: `ec1fd0bd73a861279efa2bb63acba1c875c5bf39fb8887b14c5be01b62ffc04a`
- `after.png`: `5d4c5a5af96166e25f141c061886918092bfdcd0f58ad17858b761793d2f0fd0`
