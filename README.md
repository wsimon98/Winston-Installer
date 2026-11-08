# Winston

Winston is an account-free, self-hosted Android security camera. Install the same app on two or more phones — one runs as a camera, another as a viewer. No cloud backend, no sign-in, no tracking. Video stays on your own phones and your own network (local Wi-Fi or Tailscale/VPN for remote access).

This repository only hosts the installable app. The source code is kept in a private repository.

## Install

Open **[Releases](../../releases/latest)** and download the APK under Assets. Install it on each Android phone (8.0 / API 26 or newer). Android may ask you to allow installing from your browser or files app — that's expected for an app distributed outside the Play Store.

## Getting started

1. Install the same APK on two phones.
2. Open Winston on the phone you want to use as a camera, switch to **Camera mode**, and start it.
3. Open Winston on the other phone (**Viewer mode** by default), tap **+ Add Camera**, and scan the QR code shown on the camera phone — or enter its address/ID/PIN manually.
4. Watch the live feed, set up motion detection, and manage everything from the viewer.

## What it does

- Live video between paired phones (LAN or Tailscale)
- Motion detection with recording, adjustable sensitivity and schedule
- Clip playback, download, and sharing from the viewer
- Remote snapshot and alarm
- Multi-camera grid view
- Push-style alerts for motion, low battery, and offline cameras

## A note on security

This is an independent, experimental project — not security-audited. Video and pairing traffic are unencrypted on ordinary Wi-Fi, so use Tailscale or another VPN for anything beyond a trusted home network. Don't expose a camera's port directly to the public internet.

## Questions or issues

This repo doesn't track issues for the app itself. If you installed this from a link someone sent you, reach out to them directly.
