# Discord overlay

Ascendency draws through Discord’s **new Game Overlay**. If that overlay is off, legacy overlay is still on, or the game is exclusive fullscreen, the menu will not show.

{% hint style="info" %}
Use the Discord **desktop** app. The browser client has no overlay.
{% endhint %}

{% stepper %}
{% step %}
### Open Discord settings

In the desktop app, click the **gear** next to your username (bottom left).
{% endstep %}

{% step %}
### Game Overlay

In the left sidebar, open **Game Overlay** and set it like this:

| Setting | Value |
| --- | --- |
| Enable Overlay | **On** |
| Enable Legacy Overlay | **Off** |
| Your game (e.g. Rob Run) | Overlay **on** for that title |

<figure><img src=".gitbook/assets/game-overlay.png" alt="Discord Game Overlay panel"><figcaption>Game Overlay — new overlay on, legacy off, enabled for the game you are injecting.</figcaption></figure>
{% endstep %}

{% step %}
### Hardware acceleration

Open **System** (sometimes under Advanced) and turn **Enable Hardware Acceleration** on.

<figure><img src=".gitbook/assets/hardware-acceleration.png" alt="Discord Hardware Acceleration enabled"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Display mode

The new overlay only works in **windowed** or **borderless / windowed fullscreen**. Exclusive fullscreen hides it.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Wait until overlay is actually up before you press OK in the loader.

1. Start Ascendency first — on Windows 11 it relaunches Discord with `--disable-direct-composition`.
2. Give Discord up to about a minute. You should see overlay initialise on the game (the status in Game Overlay).
3. Then join. Press `+` / Numpad `+` once the overlay is live.
{% endhint %}
