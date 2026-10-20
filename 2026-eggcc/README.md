# build instructions

- Install Rhombus from a nightly snapshot:
  https://users.cs.utah.edu/plt/rhombus-snapshots/ (the deck was last run on
  the 2026-10-12 snapshot, Racket v9.3.0.10 / Rhombus v1.1.0.2). Put the
  install's `bin` (on Windows, the install folder itself) on `PATH`.
- `raco pkg install --auto slideshow-exe`, for `raco slideshow` (the Rhombus
  distribution ships `slideshow-lib` but not the command).
- Fonts: the deck is set in PT Mono, Helvetica Neue (or Nimbus Sans where that
  is not installed) and Times New Roman. The free faces are in `fonts/`; on the
  Mac and Linux they load from there, on Windows install them (right-click,
  Install) first. It refuses to run on substitutes rather than draw with them.
- `make` builds `talk.pdf`; `make show` (or `rhombus talk.rhm`) runs the talk.

The deck needs nothing else: the drawing runtime it was written against,
formerly the `glide-pptx` package, is vendored in `glide/`.
