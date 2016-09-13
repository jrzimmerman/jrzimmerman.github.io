+++
Categories = ["HyperTerm", "Terminal"]
Description = ""
Tags = ["HyperTerm", "Terminal"]
date = "2016-07-23T22:26:47-04:00"
menu = "main"
title = "Switching from iTerm to HyperTerm"

+++

Recently [zeit.co](https://zeit.co/) released to the world a wonderful terminal built with JavaScript / HTML / CSS called [HyperTerm](https://hyperterm.org/). Even better yet, this terminal is fully customizable with open source plugins.

I'm not one to change my development environment constantly, but this electron app was simple to install on OSX and even easier to customize programmatically.

My hope is to demo how simple it is to get started with HyperTerm, and show how I only added a few lines to the configuration file to have a terminal I enjoy to use.

### Installing HyperTerm

To install HyperTerm on OSX simply install the .pkg file from their [website](https://hyperterm.org/#installation).

Once installed, use your editor of choice to open `~/.hyperterm.js`

While the default configuration is very good, I have a few recommended configurations.

### Configuring HyperTerm

First, change the theme by simply adding `hyperterm-solarized-dark` to the plugins array.

```
plugins: [
    'hyperterm-solarized-dark',
  ]
```

Save the configuration, and HyperTerm will automatically update for you.

I also enjoy using the `hyperlinks` plugin to open links with your browser, we can also add this to the plugins array.

```
plugins: [
    'hyperterm-solarized-dark',
    'hyperlinks'
  ]
```

Since I use ZSH with a Powerline font, I can simply update the fonts to include `Meslo for Powerline`.

```
// font family with optional fallbacks
fontFamily: '"Meslo LG L DZ for Powerline", Menlo, "DejaVu Sans Mono", "Lucida Console", monospace'
```

We can also modify the default window size of HyperTerm.

```
// size of window by pixels (width, height)
windowSize: [1300, 650]
```

With a few lines of code, we now have a fully customizable terminal!
