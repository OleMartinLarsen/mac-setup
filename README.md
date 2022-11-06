<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

## TOC
- [Mac Setup](#mac-setup)
- [Homebrew / Terminal / Shell](#homebrew--terminal--shell)
  - [Homebrew](#homebrew)
  - [Terminal](#terminal)
  - [Shell](#shell)
- [Finder](#finder)
- [Alfred](#alfred)
  - [Workflows](#workflows)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Mac Setup

**Specs:** Macbook Pro 16 M1 Pro, 16GB, 1TB

## Homebrew / Terminal / Shell

### Homebrew

[Homebrew](https://brew.sh/) to install tools and apps from the command line.

To install it, open up the built in `Terminal` app and run this command:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

This will also install the xcode build tools.

_Remember to add it to path if you are on a Apple Silicone machine_

### Terminal

Replace the built-in terminal with iTerm2.

We install this using a Homebrew "cask". Casks are full applications, similar to what you would install from the App store.

```
brew install iterm2
```

Documentation for more info on what iTerm2 can do: [https://iterm2.com/documentation.html](https://iterm2.com/documentation.html)

Once installed, launch it and customize the settings / preferences to your liking. These are my preferred settings:

* Appearance
  * Theme
    * Minimal
* Profiles
  * Default
    * General -> Working Directory -> Reuse previous session's directory
    * Text -> Font -> Fira Code
      * You can download this font [here](https://github.com/tonsky/FiraCode).
      * Same font for VS Code
    * Text -> Font Size -> 16
    * Keys -> Key Mappings -> Presets -> Natural Text Editing
      * This allows me to use the [keyboard shortcuts](https://gist.github.com/w3cj/022081eda22081b82c52) I know and love inside of iTerm2

### Shell

* Install Oh My Zsh, docs [here](https://github.com/ohmyzsh/ohmyzsh/wiki).
  * Config file in repo, file _.zshrc_

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

* Install Starship, docs [here](https://starship.rs/config/).
  * Config file in repo, file _.zshrc_
	* Add the following to the end of ~/.zshrc: ```eval "$(starship init zsh)"```
	
```
curl -sS https://starship.rs/install.sh | sh
```

## Finder

* Change "New Windows windows show" to home directory
* General -> Remove all items from desktop
* View -> Show Path Bar
* View -> Show Status Bar
* View -> Show Tab Bar
* Advanced -> Show file extensions
