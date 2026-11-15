# Discord setup

Ascendency draws through Discord’s Game Overlay. If overlay is off, legacy overlay is on, or the game is exclusive fullscreen, you will never see the menu.

{% stepper %}
{% step %}
### Open Discord settings

In the Discord desktop app, click the **gear** at the bottom left, next to your username.
{% endstep %}

{% step %}
### Game Overlay

Open **Game Overlay** and match these settings:

1. **Legacy overlay** — off.
2. **Enable overlay** — on (the new overlay).
3. Enable overlay on the game you are playing.
{% endstep %}

{% step %}
### Hardware acceleration

Open **System** (or Advanced, depending on your Discord build) and turn **Hardware Acceleration** on.
{% endstep %}

{% step %}
### Display mode

The new Discord overlay only appears in **windowed** or **borderless / windowed fullscreen**. Exclusive fullscreen hides it.

{% hint style="warning" %}
Wait for overlay before you play.

1. Launch the Ascendency loader first. On Windows 11 it restarts Discord with `--disable-direct-composition`.
2. Wait until Discord is open and the overlay is initialized — up to about a minute is normal.
3. Then join the game. Press `+` (or Numpad +) to open the menu once the overlay is live.
{% endhint %}
{% endstep %}
{% endstepper %}

If the console says `no Discord overlay hwnd yet`, overlay is still off or Discord has not created the overlay window. Continue to [Discord fixes](discord-fixes.md).
