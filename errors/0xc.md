# 0xC1–0xC9 — Driver load

Console mapped a driver-stage failure to a short code.

- `0xC1` — missing debug / load-driver privilege. Run as admin.
- `0xC2` — leftover or blocked driver. Reboot, then retry.
- `0xC3`–`0xC6` — map / ping / channel failed. Close other kernel tools, reboot, exclusion in AV.
- `0xC7` / `0xC8` — driver file missing or unread. Usually [0xA04 download](0xa04.md).
- `0xC9` — unload failed, driver still active. Reboot before the next launch.

{% hint style="warning" %}
Always reboot once after a C-series fail before you ticket. Half the reports clear on a clean boot.
{% endhint %}
