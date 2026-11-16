# SHADOW SECRETS

A Persian-language, noir-style detective mystery game.

## Play

Open [index.html](./index.html) in a modern browser. The game is implemented as a self-contained HTML document: its CSS, JavaScript, rendering code, and audio logic are embedded in the file.

## Offline support

The game source currently has no external script, stylesheet, image, font, or network dependency. It is therefore suitable as the web payload for an offline Android wrapper. Device compatibility still needs to be tested, especially WebGL rendering and audio playback inside Android WebView.

## Repository layout

```text
SHADOW-SECRETS/
├── index.html
├── README.md
└── docs/
    ├── PROJECT-STRUCTURE.md
    └── OFFLINE-ANDROID.md
```

## Android packaging

See [docs/OFFLINE-ANDROID.md](./docs/OFFLINE-ANDROID.md) for the intended offline WebView packaging layout. The Android wrapper project and signed APK are not included yet.
