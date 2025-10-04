<p align="center">
    <img src="docs/image/logo.avif" height="128">
    <h1 align="center">UniFi Protect Zabbix Template</h1>
</p>

This template, designed for monitoring the UniFi Protect application via the official API, is community‑driven and not affiliated with Ubiquiti Networks.

> [!WARNING]
> It has been tested on API version 6.1.78; preview releases have not been tested.

> [!IMPORTANT]
> Only Zabbix LTS versions are officially supported starting from 7.0. You can use an unsupported version by changing the Zabbix Release in the template file.

## Tested Devices

| Device Type | Status        |
| ----------- | ------------- |
| Cameras     | ✅ Tested     |
| Lights      | ⚠️ Not Tested |
| Sensors     | ⚠️ Not Tested |
| Chimes      | ⚠️ Not Tested |

> [!IMPORTANT]
> If you have tested this template with a device that has not been tested, please open an issue confirming its functionality or reporting any problems.

## How To Use

1. Import the Zabbix template file 'zbx_template_unifi_protect_api.yaml' that matches your Zabbix Server version.
2. Create a UniFi API key in Settings → Control Plane → Integrations → Your API Keys, and set it to never expire.
3. Create a Zabbix Host without interfaces. Assign the 'UniFi Protect API' template. Then modify '{$UNIFI_PROTECT_API_ADDRESS}'' and '{$UNIFI_PROTECT_API_KEY}' Macros as described in the 'Description'.

> [!WARNING]
> '{$UNIFI_PROTECT_API_ADDRESS}' Macros must contain only IP or DNS name.

## Contribute

This template is on early stage and can bee improved. Feel free to fork and submit pull request. 🙏🏻

## License

Licensed under the [MIT license](https://github.com/MassimilianoPasquini97/zbx_unifi_protect_api/blob/main/LICENSE.md).
