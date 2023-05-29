# my-lvim-config

{
  "vim.easymotion": true,
  "vim.incsearch": true,
  "vim.useSystemClipboard": true,
  "vim.useCtrlKeys": true,
  "vim.hlsearch": true,
  "vim.sneak": true,

  "vim.normalModeKeyBindings": [
    {
      "before": ["<leader>", "t"],
      "commands": ["editor.fold"]
    },
    {
      "before": ["<leader>", "r"],
      "commands": ["editor.unfold"]
    },
    {
      "before": ["<leader>", "d"],
      "commands": ["editor.action.goToTypeDefinition"]
    },
    {
      "before": ["<leader>", "q"],
      "commands": [":q"]
    },
    {
      "before": ["<tab>"],
      "commands": ["workbench.action.nextEditor"]
    },
    {
      "before": ["<S-tab>"],
      "commands": ["workbench.action.previousEditor"]
    }
  ],
  "vim.insertModeKeyBindings": [
    {
      "before": ["j", "k"],
      "after": ["<Esc>"]
    },
    {
      "before": ["<C-j>"],
      "after": ["<Esc>"]
    },
    {
      "before": ["<C-k>"],
      "after": ["<Esc>"]
    }
  ],
  "vim.visualModeKeyBindings": [
    {
      "before": [">"],
      "after": [">", "g", "v"]
    },
    {
      "before": ["<"],
      "after": ["<", "g", "v"]
    }
  ],
  "vim.normalModeKeyBindingsNonRecursive": [
    {
      "before": ["<leader>", "d"],
      "after": ["d", "d"]
    },
    {
      "before": ["<leader>", "/"],
      "commands": ["editor.action.commentLine"]
    },
    {
      "before": ["<leader>", "w"],
      "commands": [":w"]
    },
    {
      "before": ["<leader>", "e"],
      "commands": ["workbench.action.toggleSidebarVisibility"]
    },
    {
      "before": ["<leader>", "f"],
      "commands": ["workbench.action.quickOpen"]
    },
    {
      "before": ["<leader>", "h"],
      "after": ["_"]
    },
    {
      "before": ["<leader>", "l"],
      "after": ["$"]
    }
  ],
  "vim.leader": "<space>",

  "vim.handleKeys": {
    "<C-a>": false,
    "<C-f>": false,
    // VS Code new marker @ next occurence
    "<C-c>": false,
    // Cut
    "<C-x>": false,
    // Paste
    "<C-v>": false,
    "<C-z>": false,
    "<C-y>": false,
    "<C-d>": false,
    "<C-r>": false
  },
  "workbench.iconTheme": "material-icon-theme",
  "editor.formatOnSave": true,
  "editor.lineHeight": 1.8,
  "editor.lineNumbers": "relative",
  "editor.minimap.enabled": false,
  "workbench.colorTheme": "Material Theme",
  "workbench.startupEditor": "none",
  "[dart]": {
    "editor.formatOnSave": true,
    "editor.formatOnType": true,
    "editor.rulers": [80],
    "editor.selectionHighlight": false,
    "editor.suggest.snippetsPreventQuickSuggestions": false,
    "editor.suggestSelection": "first",
    "editor.tabCompletion": "onlySnippets",
    "editor.wordBasedSuggestions": false
  },
  "window.zoomLevel": 1
}
