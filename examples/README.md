## Description

These scripts are designed to interface with the plugin to expose the web-based switch.

## Requirements

* NodeMCU

* Relay

* Micro-USB cable

## How-to

1. First, follow [this](https://gist.github.com/Tommrodrigues/8d9d3b886936ccea9c21f495755640dd) gist which walks you through how to flash a NodeMCU.

2. Connect the NodeMCU to the relay board

3. Assuming that you already have [homebridge](https://github.com/nfarina/homebridge#installation) set up, the next thing you will have to do is install the plugin:
```
npm install -g homebridge-web-switch
```

4. Finally, update your `config.json` file following the example below:

```json
"accessories": [
     {
       "accessory": "WebSwitch",
       "name": "Switch",
       "apiroute": "http://switch.local"
     }
]
```
