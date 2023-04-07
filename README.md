# PLCC IEC 61131-3 Development Environment

## Features:
- Multi-platform support
  - Windows, macOS, Linux
- Cloud-based Compile Farm.
- Built-in Standard and Motion (PLCopen) libraries.
- Support for ST/IL/LD programming languages.
- IEC 61131-3 project templates.
- CJK support.
- Remote Language Server
  - Live Diagnostics.
  - Semantic Highlighting.
  - Goto Definition.
  - Suggestions.
- Built-in support for
  - CANopen configuration (DCF)
  - EtherCAT configuration (ENI)
  - Modbus configuration (YAML)
  - IO mapping (Yaml)
- EtherCAT/IO/Modbus mapping editor.
- Simple real-time data visualization.
- Supported targets:
  - HCFA PLCs (R8A, R8C, Q5... with specific firmware)
  - Linux (amd64)
  - WebAssembly
- Edge Controller support:
    - HCFA Q5 as Edge Controller (The firmware will be released soon)
    - Raspberry Pi 4B as Edge Controller (The image will be released soon)
- A simple Testing Framework.

## Recommended color themes for the semantic highlighting feature:
- Dark+ (default dark)
- Light+ (default light)

With additional settings
```json
 "editor.semanticTokenColorCustomizations": {
    "enabled": true,
    "rules": {
      "property": "#2ea154",
      "operator": "#3b8abb",
      "parameter": "#a89f23"
    }
 }

```

## How to Turn Your Raspberry Pi 4B into an Edge Controller

Follow these steps:

1. Install Ubuntu 22.04 LTS on your Raspberry Pi 4B. Ensure that WiFi is properly configured and able to connect to the internet.
2. Connect to the device using SSH via WiFi.
3. Obtain the MAC address of the wired network device using `ifconfig`.
4. Run `curl -sL https://raw.githubusercontent.com/david9991/plcc-edge/main/raspi/install.sh | sudo sh -s <The Mac Address> <Username>`. Replace `<The Mac Address>` and `<Username>` with the MAC address of your Raspberry Pi's wired network device and a non-root username that you are currently using, respectively. For example: `curl -sL https://raw.githubusercontent.com/david9991/plcc-edge/main/raspi/install.sh | sudo sh -s e4:5f:01:05:95:3c david`.
5. Finally, reboot your device.
6. Change the `target` to `linux-arm64` in your `project.json` file in your project folder to run on Raspberry Pi.

Note: Currently, all devices are exposed to the whole cloud. We do not support private devices at the moment. You can change the device name by changing the `--name` parameter of `plcc-edge` services.


## Service Availability Notice
Please be advised that we do not guarantee that our services will always be available. As a growing free service, we may experience downtime, technical issues, or other interruptions in service. We apologize for any inconvenience this may cause and we are continually working to improve our systems and minimize disruptions. Thank you for your understanding.

## Privacy & Terms

- By using this extension, you agree that we can temporarily save your project data on our server for syntax analysis, diagnosis, and compiling. All temporary files are immediately deleted after you disconnect from the server.
- The extension will download a helper from our server for local project folder access and as a gateway between your computer and the Language Server. It only accesses your opening project folders and doesn't collect any information otherwise.
- The opening project mentioned above only affects our IEC61131-3 projects that contain a project.json file in the folder with the map {"type": "PLCC-IEC61131-3"}. The Helper will never access your other kinds of folders and files.

## TODO:

- Onshape CAD integration (for simulating/digital twin).
- WebAssembly runtime environment (Enhanced WASI).
- Remote Language Server
    - Goto Type Definition.
    - Goto Implementation.
    - Formatting.
    - Find References.
    - Outline.
- PLC Module Marketplace.
- Web3-based experimental features.
    - PLC Module Marketplace with NFT support.
- FBD/SFC programming languages.
- IEC 61131-3 project view.
- Debug adapter.
- EtherCAT/IO/Modbus configurator.
- PLC Module Packaging & Publishing Tools.
- Open-source PLC device.
- IEC 61850 support.
- IEC 61499 support.
- PLCopenXML export/import/as a project.
- Natural Language-driven configuration.

## Discussion:

Telegram: [https://t.me/plcc_support](https://t.me/plcc_support)
