# Better Ouput!

<div style="text-align: center;">
<script type="text/javascript" src="https://asciinema.org/a/96884.js" id="asciicast-96884" async></script>
</div>

# Colored Diffs!

BP4O will use [colordiff](http://www.colordiff.org/) to output diffs in color from commands like `p4 diff` and `p4 describe`

To get colored diffs, install [colordiff](http://www.colordiff.org/) and unset `P4DIFF`.

# Aliases!

BP4O works with most basic [Perforce aliases](https://www.perforce.com/perforce/r16.1/manuals/cmdref/chapter.introduction.html#introduction.aliases)!

BP4O also provides its own aliasing for p4 clients that don't support Perforce aliases:

Add a file named `aliases` to `~/.config/bp4o/`.
Each line of `~/.config/bp4o/aliases` is treated as an alias with the syntax `<alias> = <command>`.

e.g.

```
ch = change
op = opened
su = submit
log = changes -s submitted -l
```

# Install!

## macOS

```
brew tap zachwhaley/beer
brew install bp4o
```

## Ubuntu

```
sudo add-apt-repository ppa:zachwhaley/ppa
sudo apt update
sudo apt install bp4o
```

## Fedora

```
sudo dnf copr enable zachwhaley/bp4o
sudo dnf install bp4o
```

## Manually

See [README](https://github.com/zachwhaley/bp4o#others)

## Zsh Users

Load BP4O by adding this to your `~/.zshrc`:

```
autoload -Uz bp4o
bp4o
```
