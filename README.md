# Generic SIP Video Doorbell Card for Lovelace

Addapted version of vivint/vivotek video doorbell card for lovelace addapted from the awesome work made by https://github.com/tommyjlong 
here https://github.com/tommyjlong/doorvivint-card, and addapted to meet my needs.

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)

# CARD CODE
```
- cards:
    - type: custom:gensipdoor-card
    camera_entity: camera.cam
    sip_settings:
        sip_password: !secret sip_doorphone
        sip_server: ASTERISK_IP
        sip_username: "THIS_EXTENSION_NUMBER"
        sip_wss_url: "wss://YOUR.duckdns.org:8089/ws"
        sip_doorbell_username: "DOORPHONE_EXTENSION_NUMBER"
    title: null
    style: |
        ha-card {
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 88%;
        }
   type: horizontal-stack
```


# Install instructions:
- What do you need:
  - a working instance of asterisk
  - a sip compatible doorphone
  - install this with HACS
  - setup a extension with wss support
  - a lot of goodwill

- HOW CAN YOU DO THAT:
  - TODO


# Credits:
- https://github.com/tommyjlong/doorvivint-card
- The original DoorDroid Call came from Ronald Dehuysser [rdehuyss](https://github.com/rdehuyss/DoorDroid).
- The JavaScript SIP Library (JSSIP) is used to provide the SIP Protocol for the Browser. Reference: [jssip home](https://jssip.net/), and [jssip github](https://github.com/versatica/JsSIP/).



