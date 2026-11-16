# Offline Android packaging notes

The target is an installable APK that runs without an internet connection.

## Web payload location

When an Android WebView wrapper is added, copy the game file to:

```text
app/src/main/assets/index.html
```

The wrapper should open the local file:

```text
file:///android_asset/index.html
```

## WebView requirements

- Enable JavaScript because the game logic is JavaScript-based.
- Keep hardware acceleration enabled; the game uses WebGL.
- Test pointer/touch input on physical Android devices.
- Test audio after a user gesture; the game uses the browser audio API.
- Do not load remote scripts, stylesheets, images, or fonts.
- For a fully offline build, do not add the Android `INTERNET` permission unless a later feature genuinely requires network access.

## Current status

This repository currently contains the web game source and packaging notes only. It does not yet contain an Android Studio project, an App Inventor project, a signing configuration, or a compiled APK. Those should be added as a separate, testable step rather than represented as already completed.
