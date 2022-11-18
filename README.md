# PLCC IEC 61131-3 Development Environment

## Features:
- Cloud-based Compile Farm.
- Built-in Standard, Motion(PLCopen) libraries.
- Support ST/IL/LD programming languages.
- IEC 61131-3 project templates.
- CJK support.
- Remote Language Server
  - Live Diagnostic.
  - Semantic Highlighting.
  - Goto Definition.
  - Suggestion.
- Built-in support for
  - CANopen configuration (DCF)
  - EtherCAT configuration (ENI)
  - Modbus configuration (YAML)
  - IO mapping (Yaml)
- EtherCAT/IO/Modbus mapping editor.
- Simple Real-time data visualization.
- Supported targets:
  - HCFA PLCs. (R8A, R8C... with specific firmware.)
  - Linux (amd64)
  - WebAssembly
- A simple Unit Test Framework.

## Recommended color themes for the semantic highlighting feature:
- Dark+ (default dark)
- Light+ (default light)

With additional settings
```
 "editor.semanticTokenColorCustomizations": {
    "enabled": true,
    "rules": {
    "property": "#2ea154",
    "operator": "#3b8abb",
    "parameter": "#a89f23"
    }
 }
```

## Privacy & Terms
- When you use this extension, you agree that we can temporarily save your project data on our server for syntax analysis, diagnosing, and compiling. And all temporary files are immediately deleted after you disconnect from the server.
- The extension will download a helper from our server for local project folder access and as a gateway between your computer and the Language Server. It only accesses your opened project folders and doesn't collect any information otherwise.
- The `opened project` mentioned above only affects our IEC61131-3 projects that contained a `project.json` file in the folder with map ` {"type": "PLCC-IEC61131-3"}`, the helper will never access your other kind of folder and files.

## TODO:
- Onshape CAD integration (for simulation/digital twin).
- WebAssembly runtime envirenment.
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

## Discussion:
Telegram: https://t.me/plcc_support

<!-- ## Screenshots
Create a project.

Live Diagnostic and Semantic Highlighting.

References.

Outline.

Auto Completion.

Formating. -->

