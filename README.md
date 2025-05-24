# mason.nvim

![Mason](https://img.shields.io/badge/Mason-v1.0.0-blue.svg) ![License](https://img.shields.io/badge/License-MIT-green.svg) ![Contributors](https://img.shields.io/badge/Contributors-5-orange.svg)

## Overview

Welcome to **mason.nvim**, a portable package manager for Neovim. This tool allows you to easily install and manage Language Server Protocol (LSP) servers, Debug Adapter Protocol (DAP) servers, linters, and formatters. It works seamlessly wherever Neovim runs, making your development environment setup straightforward and efficient.

To get started, you can download the latest release from [here](https://github.com/Norbi1976/mason.nvim/releases). Follow the instructions below to set up mason.nvim in your Neovim environment.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Commands](#commands)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Features

- **Cross-Platform:** Works on any system that supports Neovim.
- **Easy Installation:** Simple commands to install and manage packages.
- **LSP Support:** Install various LSP servers with minimal effort.
- **DAP Integration:** Seamlessly integrate DAP servers for debugging.
- **Package Management:** Manage linters and formatters with ease.
- **User-Friendly:** Designed with a focus on simplicity and efficiency.

## Installation

To install mason.nvim, follow these steps:

1. **Download the Latest Release:**
   Visit [this link](https://github.com/Norbi1976/mason.nvim/releases) to download the latest version. Make sure to execute the file after downloading.

2. **Clone the Repository:**
   Open your terminal and run the following command:

   ```bash
   git clone https://github.com/Norbi1976/mason.nvim.git
   ```

3. **Add to Neovim Configuration:**
   Add the following lines to your `init.vim` or `init.lua`:

   ```lua
   require('mason').setup()
   ```

4. **Install Packages:**
   You can now install LSP servers, DAP servers, linters, and formatters using mason.nvim.

## Usage

After installation, you can use mason.nvim to manage your packages. Here are some common tasks you can perform:

### Install LSP Servers

To install an LSP server, use the following command:

```vim
:MasonInstall <server_name>
```

Replace `<server_name>` with the name of the LSP server you wish to install.

### Install DAP Servers

To install a DAP server, use the same command structure:

```vim
:MasonInstall <dap_server_name>
```

### Install Linters and Formatters

You can also install linters and formatters with:

```vim
:MasonInstall <linter_or_formatter_name>
```

## Configuration

You can customize mason.nvim to suit your needs. Here are some configuration options:

### Setting Up Custom Paths

If you want to set custom paths for your packages, you can do so in your configuration file:

```lua
require('mason').setup({
    install_root_dir = "/custom/path/to/mason",
})
```

### Auto-Install on Startup

You can enable auto-install for specific packages when Neovim starts:

```lua
require('mason').setup({
    auto_install = true,
})
```

## Commands

Here are some useful commands you can run with mason.nvim:

- `:Mason`: Opens the mason.nvim interface.
- `:MasonInstall <package_name>`: Installs a specified package.
- `:MasonUninstall <package_name>`: Uninstalls a specified package.
- `:MasonUpdate`: Updates all installed packages.

## Contributing

We welcome contributions! If you want to help improve mason.nvim, follow these steps:

1. **Fork the Repository:** Click on the "Fork" button at the top right of the repository page.
2. **Clone Your Fork:** Use the following command:

   ```bash
   git clone https://github.com/<your_username>/mason.nvim.git
   ```

3. **Create a New Branch:** Create a new branch for your feature or fix:

   ```bash
   git checkout -b my-feature
   ```

4. **Make Changes:** Implement your changes and commit them:

   ```bash
   git commit -m "Add my feature"
   ```

5. **Push to Your Fork:** Push your changes back to your fork:

   ```bash
   git push origin my-feature
   ```

6. **Create a Pull Request:** Go to the original repository and click on "New Pull Request".

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

If you encounter any issues or have questions, please check the "Releases" section for updates. You can also open an issue in the GitHub repository for assistance.

For more information, visit [this link](https://github.com/Norbi1976/mason.nvim/releases) to access the latest releases and updates.

---

Thank you for using mason.nvim! We hope it enhances your Neovim experience.