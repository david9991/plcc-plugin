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
