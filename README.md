# Advanced Speaker Timer — Downloads

A presentation timer for macOS that drives a second display, with a
[Bitfocus Companion](https://bitfocus.io/companion) module for Stream Deck control.

**[⬇ Download the latest release](../../releases/latest)**

---

## What's in a release

Each release has three downloads. Pick one:

- **`…-bundle.zip`** — everything in one file: the app, the Companion module,
  and a readme. **Start here if you're not sure.**
- **`AdvancedSpeakerTimer-….zip`** — just the macOS app.
- **`AdvancedSpeakerTimer-CompanionModule-….tgz`** — just the Companion module, if you already
  have the app and only need to update Companion.

Filenames end in a version number. The app and the module are versioned
separately, so their numbers differ.

---

## Installing the app

1. Download **Advanced Speaker Timer** from the latest release. Most browsers
   unzip it for you; if not, double-click the downloaded file.
2. Drag the app into your **Applications** folder.
3. **The first launch needs an extra step** — see below.

### First launch: "Apple could not verify this app"

macOS blocks apps that aren't notarized by Apple, and this one isn't. The app is
safe, but you have to tell macOS to allow it once:

1. Double-click the app. You'll get a warning that it can't be opened — click
   **Done** (do *not* click "Move to Trash").
2. Open **System Settings → Privacy & Security**.
3. Scroll down. You'll see a message about *Advanced Speaker Timer* being
   blocked — click **Open Anyway**.
4. Confirm with **Open**.

You only do this once. The app opens normally from then on.

> On older macOS versions you can instead right-click the app and choose **Open**.

---

## Installing the Companion module

Requires Companion 3.x or newer.

1. Download the module file (it ends in `.tgz`). **Don't unzip it** — Companion
   wants it as-is.
2. In Companion, open the **Modules** page.
3. Choose the option to import/install a module from a file and select the
   `.tgz`.
4. Go to **Connections**, add **Advanced Speaker Timer**, and set:
   - **Host** — `127.0.0.1` if Companion runs on the same Mac as the app,
     otherwise that Mac's IP address
   - **Port** — `18765`
5. In the app's sidebar, turn on **Enable network control**.

The connection should go green. If it doesn't, check that network control is on
in the app and that nothing is blocking the port.

### Getting a timer onto a button

Open the **Presets** tab in Companion and drag one of the ready-made buttons
onto your Stream Deck. **Timer A countdown** shows the live time and recolours
itself — white when idle, green running, amber in the warning window, red in
overtime.

There are also presets for start/pause, reset, ±1 minute, output control, live
messages, and one button per timer preset you've set up in the app.

---

## Reporting a problem

Open an [issue](../../issues) and include your macOS version, the app version,
and what you expected to happen.
