# Redeem a license

Use a new key, replace an expired one, or recover a saved login.

{% stepper %}
{% step %}
### Open the loader

Launch `rob_run_handshake.exe` as administrator.
{% endstep %}

{% step %}
### Paste the key

If the license field appears, paste the full key and confirm. Do not add spaces. Keys look like grouped segments separated by dashes.
{% endstep %}

{% step %}
### Replace an old key

If a previous key was saved and you need a new one, delete `%LOCALAPPDATA%\asc\cred.json` and launch again, then paste the new license.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
One license is bound to your KeyAuth user. Sharing a key with someone else will lock or reset the session. Open a Discord ticket if you need a HWID reset.
{% endhint %}
