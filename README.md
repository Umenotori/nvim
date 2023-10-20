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

### Nvim Harpoon

<leader>a  -> mark add file
<C-e>      -> ui toggle menu
<C-h>	 -> nav file 1
<C-t>      -> nav file 2
<C-n>      -> nav file 3
<C-s>      -> nav file 4

### Nvim Undotree

<leader>u  -> undotreetogl
<C-w>h     -> change window

### Nvim Fugitive

<leader>gs -> Git status

### Nvim LSP-Zero

<C-p>      -> prev item
<C-n>      -> next item
<C-y>      -> confirm
<C-Space>  -> complete
gd         -> definition
K          -> hover
<leader>vws-> workspace_symbol 
<leader>vd -> diagn open_float
[d         -> diagn goto_next
]d         -> diagn goto_prev 
<leader>vca-> code_action 
<leader>vrr-> references 
<leader>vrn-> rename
"i", <C-h> -> signature_help pv

### Nvim Refactoring

<leader>ri -> refactor inline var

### Nvim Trouble

<leader>xq -> TrToggle quickfix
