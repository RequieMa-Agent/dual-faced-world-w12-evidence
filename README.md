# dual-faced-world W12 before/after screenshots

Automated evidence for [RequieMa/dual-faced-world PR #39](https://github.com/RequieMa/dual-faced-world/pull/39)
(Issue #19). Captured from a real Godot 4.7.2 run, 1152x648, same entry scene and capture method:

- `before.png` — `scenes/main.tscn` at `develop` `9812b2d` (empty Node2D placeholder).
- `after.png` — `scenes/main.tscn` on the PR branch (`feature/integration-smoke-w12-149dbab59087`, head `ffc8160`),
  instantiating `scenes/game_root.tscn`.

Capture: load `res://scenes/main.tscn`, wait 15 rendered frames, save the root viewport via
`get_texture().get_image().save_png()`.

These images are referenced from the PR description so reviewers can see the visual delta.
