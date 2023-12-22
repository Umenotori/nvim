# Nvim Config

## Minimal requirements

The bare minimum plugins are:

* A package manager ([Packer.nvim][packer])
* A fuzzy finder ([Telescope.nvim][telescope])
* [Treesitter][treesitter]
* A LSP server and auto completion ([LSP zero][lsp])

## Complementary configurations

* Custom Keymaps
* Custom Theme ([Kanagawa dragon][theme])
* file swapping ([harpoon.nvim][harpoon])
* undotree ([undotree.nvim][undotree])
* git integration ([fugitive.nvim][fugitive])
* refactoring ([refactoring.nvim][refactoring])
* [treesitter context][context]
* diagnostics ([trouble.nvim][trouble])

## General Instructions

First install need to download packer from 'git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim' and run ':PackerSync'.
 May be needed to download java from the package manager to instal .npm files.
It's needed to ` :source ` (`:so`) the packer.lua file everytime a plugin is changed, including on install.
Almost every plugin includes a file in after/plugin for settings.
The lsp server can be downloaded by mason.nvim using ` :Mason `

## Custom Keymaps Used

### Nvim

| Keymaps                   | Description                    |
| ------------------------- | ------------------------------ |
| vim.g.mapleader = " "     | [leader] = <kbd>space          |
| "v", J                    | moves selected text down       |
| "v", K                    | moves selected text up         |
| J                         | cursor stays in place          |
| [leader] p                | p multiple times same text     |
| [leader] y                | y into + register (clipboard)  |
| [leader] d                | d into void register           |
| [C-k]                     | quickfix navigation            |
| [C-j]                     | quickfix navigation            |
| [leader] k                | quickfix navigation            |
| [leader] j                | quickfix navigation            |
| [leader] s                | replace word on cursor (`:%s`) |
| [leader] pv               | back to netrw   (`:Ex`)        |

### Nvim Telescope

| Keymaps         | Description |
| --------------- | ----------- |
| [leader] pf     | find files  |
| [C-p]           | git files   |
| [leader] ps     | grep        |
| [leader] vh     | help tags   |

### Nvim Harpoon

| Keymaps   | Description    |
| --------- | -------------- |
| [leader] a| mark add file  |
| [C-e]     | ui toggle menu |
| [C-h]     | nav file 1     |
| [C-t]     | nav file 2     |
| [C-n]     | nav file 3     |
| [C-s]     | nav file 4     |

### Nvim Undotree

| Keymaps   | Descriptions   |
| --------- | -------------- |
| [leader] u| undotreetoggle |
| [C-w]h    | change window  |

### Nvim Fugitive

| Keymaps    | Descriptions |
| ---------- | ------------ |
| [leader] gs| Git status   |

### Nvim LSP-Zero

| Keymaps     | Descriptions     |
| ----------- | ---------------- |
| [C-p]       | prev item        |
| [C-n]       | next item        |
| [C-y]       | confirm          |
| [C-Space]   | complete         |
| gd          | definition       |
| K           | hover            |
| [leader] vws| workspace_symbol |
| [leader] vd | diagn open_float |
| [d          | diagn goto_next  |
| ]d          | diagn goto_prev  |
| [leader] vca| code_action      |
| [leader] vrr| references       |
| [leader] vrn| rename           |
| "i", [C-h]  | signature_help   |

### Nvim Refactoring

| Keymaps        | Descriptions        |
| -------------- | ------------------- |
| [leader] ri    | refactor inline var |

### Nvim Trouble

| Keymaps    | Descriptions           |
| ---------- | ---------------------- |
|[leader] xq | TroubleToggle quickfix |

[packer]: https://github.com/wbthomason/packer.nvim
[telescope]: https://github.com/nvim-telescope/telescope.nvim
[treesitter]: https://github.com/nvim-treesitter/nvim-treesitter
[lsp]: https://github.com/VonHeikemen/lsp-zero.nvim
[theme]: https://github.com/rebelot/kanagawa.nvim
[harpoon]: https://github.com/ThePrimeagen/harpoon
[undotree]: https://github.com/mbbill/undotree
[fugitive]: https://github.com/tpope/vim-fugitive
[refactoring]: https://github.com/ThePrimeagen/refactoring.nvim
[context]: https://github.com/nvim-treesitter/nvim-treesitter-context
[trouble]: https://github.com/folke/trouble.nvim
