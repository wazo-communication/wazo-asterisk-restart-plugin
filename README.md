# wazo-asterisk-restart-plugin

Restart Asterisk every night at 23:30, once no calls are active.
If calls are remaining after 1 hour of retrying, the restart task is cancelled until the next day.

## Installation

```sh
wazo-plugind-cli -c "install git https://github.com/wazo-communication/wazo-asterisk-restart-plugin"
```

## Monitoring

Use standard `systemd` tools to check the status:

```
systemctl status wazo-asterisk-restart.timer
systemctl status wazo-asterisk-restart.service
```
