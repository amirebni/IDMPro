# MyDM — visual refresh

This is a presentation-only refresh of amirebni/idm. The segmented download engine, browser bridge, scheduling, settings, clipboard capture, media selection and saved-state format remain unchanged.

## Changes
- Neutral surfaces and a restrained emerald accent, with coordinated light and dark palettes.
- More comfortable spacing, quieter file-type tiles and flatter download rows.
- Organized toolbar: Start, Pause and Remove stay visible; Paste, Import, Export and Clear completed move to More.
- Refined library navigation and matching browser-extension popup.

## Run
Python 3 with Tk support is required.

```sh
pip install "requests[socks]" tkinterdnd2
python dm.py
```

Optional helper files (`yt-dlp`, `ffmpeg.exe`, `qjs.exe`) are acquired by the existing Windows build workflow. To build the Windows installer, use the included .github/workflows/build.yml in the repository root.

The web app is an interactive visual preview with sample downloads. It is not connected to the Python download engine. No compiled Windows installer is included. Desktop syntax was checked; native desktop rendering requires testing on Windows/macOS/Linux with Tk.
