# Pre-requisites

## [Hyper-V on Windows 10](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v)

Open PowerShell as an Administrator and run:

If on Windows Pro:
```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All
```

If on Windows Home:
```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

## WSL

Install WSL. Open cmd as an Administrator and type the following:

```
wsl --install
wsl --set-default-version 2
```

Next, install the Linux distro of your choice (Ubuntu) via the Microsoft Store.

## [Remote Development pack](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)

This allows you to edit code in VSCode that lives on the WSL.

## [Microsoft Terminal](https://github.com/microsoft/terminal)

Search for Winows Terminal in the Microsoft Store.

## Docker

Install [Docker for Windows](https://hub.docker.com/editions/community/docker-ce-desktop-windows/). If prompted, install the WSL2 Backend.

**IMPORTANT NOTE:** Do _not_ install docker on the Linux subsystem via apt-get. You _must_ install Docker for Windows Desktop.
