# MAPP Snare firmware releases

Signed firmware images for the MAPP Snare drum trigger. This repository only
holds releases; the firmware source is private.

The MAPP Snare iPhone app reads the latest release from here and installs it
on the drum over Bluetooth. You don't need to download anything by hand.

## What's in a release

Each release is tagged with the firmware version (e.g. `v0.3.0`) and has two
files:

- `mapp-snare-firmware-<version>.bin`: the firmware image, signed with the
  project's key. The drum refuses images that aren't signed with it.
- `manifest.json`: the version, file name, size, SHA-256 and protocol
  version, which the app checks before sending the image.

The drum accepts any signed version, including older ones, so an earlier
release can be installed again from its release page.
