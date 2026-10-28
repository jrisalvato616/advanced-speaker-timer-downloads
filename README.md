# Advanced Speaker Timer — Downloads

A presentation timer for macOS that drives a second display, with a
[Bitfocus Companion](https://bitfocus.io/companion) module for Stream Deck control.

**[⬇ Download the latest release](../../releases/latest)**

---

## What's in a release

Each release has three downloads. Pick one:

- **`AdvancedSpeakerTimer-…-Bundle.zip`** — everything in one file: the app,
  the Companion module, and a readme. **Start here if you're not sure.**
- **`AdvancedSpeakerTimer-…-App.zip`** — just the macOS app.
- **`AdvancedSpeakerTimer-…-CompanionModule.tgz`** — just the Companion module,
  if you already have the app and only need to update Companion.

The app and the Companion module share a version number: use the module with
the same number as your app.

---

## Installing the app

The current build supports Apple Silicon Macs running macOS 15.5 or later.

1. Download **Advanced Speaker Timer** from the latest release. Most browsers
   unzip it for you; if not, double-click the downloaded file.
2. Drag the app into your **Applications** folder.
3. **The first launch needs an extra step** — see below.

### First launch: "Apple could not verify this app"

This build has not been notarized by Apple. If macOS blocks its first launch,
you can allow this downloaded build in System Settings:

1. Double-click the app. You'll get a warning that it can't be opened — click
   **Done** (do *not* click "Move to Trash").
2. Open **System Settings → Privacy & Security**.
3. Scroll down. You'll see a message about *Advanced Speaker Timer* being
   blocked — click **Open Anyway**.
4. Confirm with **Open**.

After you allow this build, subsequent launches normally open directly.

> On older macOS versions you can instead right-click the app and choose **Open**.

---

## Installing the Companion module

Use Companion 4 or 5; the current package was tested with Companion 5.0.3.

1. Download the module file (it ends in `.tgz`). **Don't unzip it** — Companion
   wants it as-is.
2. In Companion, open the **Modules** page.
3. Choose **Import module package** and select the intact `.tgz`.
4. Go to **Connections**, add **Advanced Speaker Timer Pro**, or edit your
   existing connection and select the module version matching your app. Set:
   - **Host** — `127.0.0.1` if Companion runs on the same Mac as the app,
     otherwise that Mac's IP address
   - **Port** — `18765`
5. In the app's sidebar, turn on **Enable network control**.

The connection should report OK after receiving current timer status. If it
doesn't, check that network control is on and that nothing is blocking the port.

### Getting a timer onto a button

Open the **Presets** tab in Companion and drag one of the ready-made buttons
onto your Stream Deck. **Timer A live display (status colours)** shows the app's
timer text — white when ready, green while running, yellow while paused, amber
during warning, and red in overtime or when finished. Unavailable data turns gray.

There are also presets for start/pause, reset, ±1 minute, output control, and
output layouts. Timer presets are grouped by destination (Timer A or Timer B),
and rotary controls browse and load highlighted presets.

Message presets load a draft. **Send Draft** sends or replaces the live message;
**Clear Msg** hides it and keeps the draft. Existing buttons retain their saved
designs; drag fresh presets to use the revised labels and feedback styles.

---

## Watching the timer on other devices

- **Same network:** in the app's sidebar, turn on **Web Display**. Any phone,
  tablet or computer on the same network can scan the QR code or open the
  address shown.
- **From anywhere:** turn on **Internet Sharing**. Viewers go to
  [timer.foundrypros.com](https://timer.foundrypros.com) and enter the show code
  the app shows, or scan its QR code. Click **New** for a fresh code, or type
  your own (6–12 letters or numbers).

Both are view-only.

---

## Reporting a problem

Open an [issue](../../issues) and include your macOS version, the app version,
and what you expected to happen.
