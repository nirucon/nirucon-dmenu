# nirucon dmenu scripts launcher

## Overview

`nirucon-dmenu-scripts-launcher` is a lightweight script that uses `dmenu` to provide a convenient launcher for various scripts located in `/usr/local/bin`. The launcher allows users to quickly access and run predefined scripts through a simple and user-friendly interface.

Designed to be used with my [nirucon-alpi post install script](https://github.com/nirucon/nirucon-alpi) and [nirucon-suckless-arch dwm setup](https://github.com/nirucon/nirucon-suckless-arch)

## Features

- **Exit System Options**: Launches the `dwmexit-dmenu` script.
- **Scan for WiFi**: (Visible only if the system has a WiFi card) Launches the `wifi-dmenu` script.
- **Optimize Arch System**: Launches the `arch-optimizer-dmenu` script.
- **Swedish Radio**: Launches the `srplay-dmenu` script.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/nirucon/nirucon-dmenu
    ```

2. Move the script to `/usr/local/bin` and make it executable:
    ```sh
    sudo mv nirucon-dmenu/nirucon-dmenu-scripts-launcher /usr/local/bin/
    sudo chmod +x /usr/local/bin/nirucon-dmenu-scripts-launcher
    ```

## Usage

Run the `nirucon-dmenu-scripts-launcher` script from dmenu or your terminal:
```sh
nirucon-dmenu-scripts-launcher
```

Select the desired script from the `dmenu` prompt and the chosen script will be executed.

## Adding More Options

To add more script options:
1. Edit the `MENU_OPTIONS` variable in the script to include new script names.
2. Add corresponding cases in the `case` statement to handle the execution of new scripts.

## License

Feel free to use and modify, donate if you want :) https://www.paypal.com/paypalme/nicklasrudolfsson
