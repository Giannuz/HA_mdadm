# RAID Status - Custom Component - Home Assistant

This is a custom component that is used to monitor the status of a RAID device created with `mdadm`

 ## Requirements

`mdadm` installed into local server

## How to install

HACS (**now not available**): Search `RAID Status - MDADM` into Integration 

Without HACS: 

1. Download the repository
2. Copy folder 'custom_components/mdadm_state' folder into the configuration folder

## Setup YAML Configuration

```yaml
# Example configuration.yaml entry
binary_sensor:
  - platform: mdadm_state
    device: devicename
```

### Configuration Variables

`device` [**REQUIRED**] : name of device. Example `device: md0` if the path of device is `/dev/md0`

## Contributions

`mdstat` library: https://pypi.org/project/mdstat/

`simplejson` library: https://pypi.org/project/simplejson/



