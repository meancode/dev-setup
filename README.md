# Development Workstation Setup

## Install Order

1. [Git](https://git-scm.com/downloads)
1. GitHub Desktop
1. [GitKraken](https://www.gitkraken.com/)
1. Node.js
1. Sublime Text
1. Sublime Theme(s)
1. Sublime Packages
1. GULP
1. Grunt

## Git Considerations

* [Formatting and Whitespace](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration#Formatting-and-Whitespace)

### Sublime Themes

* [Cobalt2](https://github.com/wesbos/cobalt2)
* [Predawn](https://github.com/jamiewilson/predawn)

### Sublime Packages 🔥

* [Package Control](https://packagecontrol.io/installation)
* PackageResourceViewer
* Alignment
* AutoFileName
* Autoprefixer
* Babel
* Babel Snippets
* Bracket Highlighter
* Colorpicker
* ChangeQuotes
* [Delete​Blank​Lines](https://github.com/NicholasBuse/sublime_DeleteBlankLines)
* EditorConfig
* EditorConfig Snippets
* Emmet
* Emmet CSS Snippets
* Emoji
* EncodingHelper
* Dockblockr
* Git
* Gitgutter
* Gist
* JavaScript Completions
* JSHint Gutter
* ScopeHunter
* Sidebar Enhancements
* [HTML-CSS-JS Prettify](https://github.com/victorporof/Sublime-HTMLPrettify)
* HTML5
* MarkdownEditing
* phpfmt
* SmartMarkdown
* [Trailing Spaces](https://github.com/SublimeText/TrailingSpaces)
* Markdown Preview
* LiveReload
* Origami
* Syntax Manager

### Misc. Key Bindings

    [
        { "keys": ["ctrl+alt+p"], "command": "prompt_select_workspace" }
    ]


### HTML-CSS-JS Prettify

If you are working with React (or similar), there is one setting you need to pay attention to:

```
"e4x": true, // Pass E4X xml literals through untouched
```

See my full `.jsbeautifyrc` [settings file](jsbeautifyrc.js) for other changes I have made. Note that in order for GitHub to display it all pretty like, I had to change the name of this file to `jsbeautifyrc.js` but that will not work in Sublime Text.

### Delete​Blank​Lines

Windows:
- Ctrl+Alt+Backspace --> Delete Blank Lines
- Ctrl+Alt+Shift+Backspace --> Delete Surplus Blank Lines

OSX:
- Fn+Ctrl+Option+Delete --> Delete Blank Lines
- Fn+Ctrl+Option+Shift+Delete --> Delete Surplus Blank Lines

Linux:
- Ctrl+Alt+Backspace --> Delete Blank Lines
- Ctrl+Alt+Shift+Backspace --> Delete Surplus Blank Lines

### Trailing Spaces

The main feature you gain from using this plugin is that of deleting all
trailing spaces in the currently edited document. In order to use this
deletion feature, you may either:

* click on "Edit / Trailing Spaces / Delete";
* bind the deletion command to a keyboard shortcut:

To add a key binding, open "Preferences / Key Bindings - User" and add:

``` js
{ "keys": ["ctrl+shift+t"], "command": "delete_trailing_spaces" }
```

With this setting, pressing <kbd>Ctrl + Shift + t</kbd> will delete all
trailing spaces at once in the current file! For OSX users, quoting wbond:
"When porting a key binding across OSes, it is common for the ctrl key on
Windows and Linux to be swapped out for super on OS X"
(eg. use "super+ctrl+t" instead).

*Beware*: the binding from this example overrides the default ST's mapping
for reopening last closed file. You can look at the default bindings in
"Preferences / Key Bindings - Default".

At any time, you can toggle highlighting on and off. You may either:

- click on "Edit / Trailing Spaces / Highlight Regions"
- bind the toggling command to a keyboard shortcut:

``` js
// I like "d", as in "detect" (overrides a default binding, though).
{ "keys": ["ctrl+shift+d"], "command": "toggle_trailing_spaces" }
```

### Cobalt2 Changes

Using PackageResourceViewer, edit the `Cobalt2.sublime-theme` file.

    // Sidebar heading
    {
        "class": "sidebar_heading",
        "color": [255, 255, 255],
        "font.bold": true,
        "shadow_color": [0, 0, 0],
        "shadow_offset": [0, -1]
    },
    // Sidebar entry
    {
        "class": "sidebar_label",
        "color": [255, 255, 255],
        "shadow_color": [0, 0, 0],
        "shadow_offset": [0, -1],
        "font.size": 12
    },

# Global NPM Install

Install [Node.js](https://nodejs.org/en/) first.

* create-react-app
* grunt-cli@
* grunt-init@
* node-static
* serve
* webpack

To list all global modules:

```
npm list -g --depth=0
```


## Browser Extensions
* Firebug for [Chrome](http://getfirebug.com/releases/lite/chrome/) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/firebug/)
* Web Developer for [Chrome](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm?hl=en-US) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/web-developer/)
* YSlow for [Chrome](http://yslow.org/) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/yslow/?src=search)
* CSS Dig for [Chrome](https://chrome.google.com/webstore/detail/css-dig/lpnhmlhomomelfkcjnkcacofhmggjmco?hl=en)
* High Contrast for [Chrome](https://chrome.google.com/webstore/detail/high-contrast/djcfdncoelnlbldjfhinnjlhdjlikmph?hl=en)
* Live HTTP Headers for [Chrome](https://chrome.google.com/webstore/detail/live-http-headers/iaiioopjkcekapmldfgbebdclcnpgnlo?hl=en)
* User-Agent Switcher for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-for-c/djflhoibgkdhkhhcedjiklpkjnoahfmg?hl=en)
* WAVE Evaluation Tool for [Chrome](https://chrome.google.com/webstore/detail/wave-evaluation-tool/jbbplnpkjmmeebjpijfedlgcdilocofh?hl=en)
* Juicy Studio Accessibility Toolbar for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/juicy-studio-accessibility-too/)
* Window Resizer for [Chrome](https://chrome.google.com/webstore/detail/window-resizer/kkelicaakdanhinjdeammmilcgefonfh?hl=en)
* React Devtools for [Chrome](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/)

## Sublime Text Links
* [PHP Setup](http://tornike.me/notes/my-sublime-setup-for-php-development)