#Nvim Config

## Minimal requirements

The bare minimum plugins are:

- A package manager (Packer.nvim)
- A fuzzy finder (Telescope)
- Treesitter
- A LSP server and auto completion (LSP zero)

## Complementary configurations

- Custom Keymaps
- Custom Theme (Kanagawa dragon)
- file swapping (harpoon.nvim)
- undotree (undotree.nvim)
- git integration (fugitive.nvim)
- refactoring (refactoring.nvim)
- treesitter context
- diagnostics (trouble.nvim)

## General Instructions

It's needed to :source (:so) the packer.lua file everytime a plugin is changed, including on install.
Almost every plugin includes a file in after/plugin for settings.

## Custom Keymaps Used

### Nvim

vim.g.mapleader = " " (<leader> key = space)
<leader>pv -> return to netrw


### Nvim Telescope

<leader>pf -> find files
<C-p>      -> git files
<leader>ps -> grep
<leader>vh -> help tags


