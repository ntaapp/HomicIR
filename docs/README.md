 

## Overview
HomicIR is fork repo from SmartIR <br> <br> 

HomicIR is a custom integration for controlling **climate devices**, **media players** and **fans** via infrared controllers.<br>
HomicIR currently supports the following controllers:
* [Broadlink](https://www.home-assistant.io/integrations/broadlink/)
* [To learn new commands for your devices using Broadlink](https://community.home-assistant.io/t/broadlink-manager-nicer-way-to-learn-and-send-ir-rf-commands/58770).
* [Xiaomi IR Remote (ChuangmiIr)](https://www.home-assistant.io/integrations/remote.xiaomi_miio/)
* [LOOK.in Remote](http://look-in.club/devices/remote)
* [ESPHome User-defined service for remote transmitter](https://esphome.io/components/api.html#user-defined-services)
* [MQTT Publish service](https://www.home-assistant.io/docs/mqtt/service/)

More than 120 climate devices are currently supported out-of-the-box, mainly for the Broadlink controller, thanks to our awesome community.<br><br>
Don't forget to **star** the repository if you had fun!<br><br>


## Installation
### *Manual*
**(1)** Place the `custom_components` folder in your configuration directory (or add its contents to an existing `custom_components` folder).
It should look similar to this:
```
<config directory>/
|-- custom_components/
|   |-- homicir/
|       |-- __init__.py
|       |-- climate.py
|       |-- fan.py
|       |-- media_player.py
|       |-- etc...
```
**(2)** Add the following to your configuration.yaml file.
```yaml
homicir:
```

homicir automatically detects updates after each HA startup and asks you to install them. It also has a mechanism that prevents you from updating if the last homicir version is incompatible with your HA instance. You can disable this feature by setting homicir as follows:
```yaml
homicir:
  check_updates: false
```

If you would like to get updates from the rc branch (Release Candidate), configure homicir as follows:
```yaml
homicir:
  update_branch: rc
```

**(3)** Configure a platform.

### *HACS*
If you want HACS to handle installation and updates, add homicir as a [custom repository](https://hacs.xyz/docs/faq/custom_repositories/). In this case, it is recommended that you turn off automatic updates, as above.
<br><br>


## Platform setup instructions
Click on the links below for instructions on how to configure each platform.
* [Climate platform](/docs/CLIMATE.md)
* [Media Player platform](/docs/MEDIA_PLAYER.md)
* [Fan platform](/docs/FAN.md)
<br><br>



<br><br>

