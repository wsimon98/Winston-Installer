# Winston

Winston is an account-free, self-hosted Android security camera. Install the same app on two or more phones — one runs as a camera, another as a viewer. No cloud backend, no sign-in, no tracking. Video stays on your own phones and your own network (local Wi-Fi or Tailscale/VPN for remote access).

This repository only hosts the installable app. The source code is kept in a private repository.

## Install

Open **[Releases](../../releases/latest)** and download the APK under Assets. Install it on each Android phone (6.0 / API 23 or newer). Android may ask you to allow installing from your browser or files app — that's expected for an app distributed outside the Play Store.

## Getting started

1. Install the same APK on two phones.
2. Open Winston on the phone you want to use as a camera, switch to **Camera mode**, and start it. The screen goes dark while streaming (tap to reveal controls) and stays awake the whole time.
3. Open Winston on the other phone (**Viewer mode** by default), tap **+ Add Camera**, and scan the QR code shown on the camera phone — or enter its address/ID/PIN manually.
4. Watch the live feed, set up motion detection, and manage everything from the viewer using the icon buttons: flip, flashlight, rotate, snapshot, alarm, motion zone, clips. Long-press a camera's tile in grid/list view for Rename / Change address / Sound alarm / Forget camera.

## What it does

- Live video between paired phones (LAN or Tailscale)
- Motion detection with recording, adjustable sensitivity, a draggable watch zone, and schedule
- Clip playback, download, and sharing from the viewer, with auto-cleanup after a configurable retention period
- Remote snapshot and an alarm with a choice of 4 sounds (tap for default, long-press to pick), optionally auto-played on motion
- Flashlight toggle and one-tap rotation cycling (0/90/180/270), usable locally or from any paired viewer
- Multi-camera grid and list view, with a charging badge so you know which cameras have reliable power
- Push-style alerts for motion, low battery, and offline cameras

## Release notes

### v0.2.0
Icon-first viewer UI (flip/flash/rotate/snapshot/alarm/motion-zone/clips as icon buttons), a single cycling rotate icon instead of four rotation buttons, a long-press camera tile menu (Rename/Change address/Sound alarm/Forget), a 4-sound alarm library with optional auto-play on motion, a charging badge on grid tiles, and keep-screen-on while in Camera mode.

### v0.1.0
Initial test build: pairing, live streaming, motion detection, clip recording, snapshot, basic alarm, and multi-camera grid view.

## A note on security

This is an independent, experimental project — not security-audited. Video and pairing traffic are unencrypted on ordinary Wi-Fi, so use Tailscale or another VPN for anything beyond a trusted home network. Don't expose a camera's port directly to the public internet.

## Questions or issues

This repo doesn't track issues for the app itself. If you installed this from a link someone sent you, reach out to them directly.
