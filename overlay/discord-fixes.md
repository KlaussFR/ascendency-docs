# Discord fixes

Overlay missing, black screen, flicker, or the loader waiting forever for Discord.

## Overlay never appears

1. Finish [Discord setup](discord-setup.md) — new overlay on, legacy off, hardware acceleration on.
2. Quit Discord from the system tray, then launch Ascendency so it can start Discord itself.
3. Use Discord stable. PTB / Canary often will not be detected.
4. Game must be borderless or windowed.

## Windows 11 composition

The loader already restarts Discord with this flag. If you need to do it by hand before launching:

```powershell
& "$env:LOCALAPPDATA\Discord\Update.exe" --processStart Discord.exe --process-start-args "--disable-direct-composition"
```

## UI flicker

Unpin every widget from the Discord overlay (voice, stream, now playing). Extra overlay widgets fight Ascendency’s host layer.

## Console clues

- `no Discord overlay hwnd yet` — overlay disabled or game exclusive fullscreen.
- `Discord Update.exe not found` — Discord is not installed in the default LocalAppData path.
- `ovhost armed` — overlay mapped; if you still see nothing, widgets or exclusive fullscreen are usually left.

{% hint style="danger" %}
Do not run two Discord clients. Close the tray icon so only the instance the loader starts remains.
{% endhint %}
