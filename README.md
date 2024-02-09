# wazo-asterisk-restart-plugin

Restart Asterisk every night, once no calls are active

## Installation

```sh
wazo-plugind-cli -c "install git https://github.com/wazo-platform/wazo-asterisk-restart-plugin"
```

## Monitoring

Use standard `systemd` tools to check the status:

```
systemctl status wazo-asterisk-restart.timer
systemctl status wazo-asterisk-restart.service
```
