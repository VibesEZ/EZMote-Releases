# EZMote

Control your Android TV or Google TV from your Android phone over Wi-Fi, with optional Bluetooth backup.

**[Download the latest EZMote APK](https://github.com/VibesEZ/EZMote-Releases/releases/latest)**

Current release: **v1.0.1 / build 2**. This update improves Wi-Fi/Bluetooth
recovery, prevents volume commands from building up behind delayed TV feedback,
and keeps the remote layout fixed while connections change. Connection activity
appears in the TV header icon; tap it for details and recovery actions.

This public repository contains download documentation, signed APK releases and checksums. The Android application source is maintained privately. GitHub's automatic Source code archives contain this repository's documentation, not the app source.

## Requirements

- Android 9 or newer on your phone.
- A compatible Android TV or Google TV Remote Service for Wi-Fi control.
- The phone and TV on the same local network.

TV developer mode, wireless debugging and a companion app are not needed. Optional Bluetooth backup requires phone firmware that supports Classic Bluetooth HID; Wi-Fi remains available if it is unsupported.

## Install and pair

1. Open the latest release and download `EZMote-VERSION-release.apk` from its assets. Choose the APK rather than a Source code archive.
2. Open the APK. If Android asks, allow installation from the browser or file manager you used, then confirm installation.
3. Open EZMote, choose **Set up my TV**, select your TV and enter the code shown on it.
4. Add Bluetooth backup using the guided setup, or skip it.

Existing public **v1.0** users can install this update over the existing app and
keep preferences and TV pairing. Use **Settings → App updates** or download the
latest signed APK. The public channel began at v1.0 / build 1; older internal
HID Nexus Remote installations remain outside that channel.

## Controls and appearance

- Direction buttons or a swipe pad, playback controls, power, volume and a separate mute button.
- Live keyboard synchronization and phone microphone input over Wi-Fi, including voice typing and supported TV app voice requests.
- Automatic connection management with optional Bluetooth backup for basic controls.
- Online app search, listing icons, saved shortcuts and home-screen widgets.
- AMOLED dark or light appearance, custom accent colors, glass or solid surfaces, and reduced-motion support.

Bluetooth HID supports basic controls according to the TV and phone firmware. Full keyboard/focus synchronization, microphone streaming, TV volume feedback and app launching need the Wi-Fi connection. Online app search uses Google Play listings; it does not fetch the TV's installed-app inventory. A shortcut needs its app installed on the TV and a supported launch link.

## Update in the app

Open **Settings → App updates** to check for a newer stable release, read its notes and download it. Automatic checks are off by default; enabling them checks at most once daily when the app opens.

Downloads can be cancelled or retried and can resume after the app restarts. EZMote verifies the APK checksum, package, signing certificate, version and Android compatibility before offering installation. Android installation access is explained when the update is ready, and Android separately asks you to confirm installation. Updates never install silently.

## Permissions and privacy

The Welcome screen requests no permissions. Optional access is explained when its feature is used. Bluetooth discovery requires location permission on Android 9–11; microphone and notification access are optional.

Microphone audio goes to your selected TV during Voice and is not saved by EZMote. The TV's assistant provider may process speech online. App searches contact Google Play. Optional update checks contact GitHub, which receives the connection IP address and app version; TV pairing credentials and microphone audio are not sent to GitHub.

## Help and feedback

If Wi-Fi discovery does not find your TV, confirm both devices are on the same network and that the router allows devices to communicate. Bluetooth support depends on phone firmware; Wi-Fi is the main connection for advanced controls.

[Open an issue](https://github.com/VibesEZ/EZMote-Releases/issues) with your phone model, Android version, TV model and steps to reproduce the problem. **Settings → Help & about → Diagnostics** shows connection information on your phone.

Each release includes its notes, compatibility limits and `SHA256SUMS.txt` for manual download verification.
