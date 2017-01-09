# Better P4 Output

<div style="text-align: center;">
<script type="text/javascript" src="https://asciinema.org/a/96884.js" id="asciicast-96884" async data-autoplay="true" data-size="medium"></script>
</div>

# Colored Diffs!

BP4O will use [colordiff](http://www.colordiff.org/) to output diffs in color from commands like `p4 diff` and `p4 describe`

To get colored diffs, install [colordiff](http://www.colordiff.org/) and unset `P4DIFF`.

# Aliases!

BP4O works with Perforce's builtin [aliasing](https://www.perforce.com/perforce/r16.1/manuals/cmdref/chapter.introduction.html#introduction.aliases)!

And BP4O provides its own aliasing!

To use BP4O aliases, add a file named `aliases` to `~/.config/bp4o/`.
Each line of `~/.config/bp4o/aliases` is treated as an alias with the syntax `<alias> = <command>`.

e.g.

```
ch = change
op = opened
su = submit
log = changes -s submitted -l
```

# Install!

BP4O works with Bash, Zsh[*](https://github.com/zachwhaley/bp4o#zsh-users), and Fish shell, and is available for

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

## Fedora/CentOS

```
sudo dnf copr enable zachwhaley/bp4o
sudo dnf install bp4o
```
