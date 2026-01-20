# Zed bug report

This repo contains an example project to reproduce a bug in Zed regarding devcontainers and the Delve (go) debugger.

## Bug details

When launching the Delve debugger inside the provided devcontainer, the debugger shuts down unexpectedly.

## How to reproduce
1. Open the project in Zed using the provided devcontainer (`./.devcontainer`)
2. Start the Zed debugger for the `Launch server` debug preset (`.zed/debug.json`)
3. The debugger shuts down unexpectedly

## Output
Console output:
```
Downloading from https://github.com/zed-industries/delve-shim-dap/releases/download/v0.0.3/delve-shim-dap-aarch64-unknown-linux-gnu.tar.gz...
Download complete
error: debugger shutdown unexpectedly
```

DAP Logs
```
stderr: the input device is not a TTY
```
