# my-kitty

### Requirements:
* nerdfont (To work the lsp icons)

----

### Using as default:
1. Create a *symlink* from the path that you have installed the kitty:

Kitty
```bash
$ sudo ln -s /your/kitty/path/kitty.app/bin/kitty /usr/bin/kitty
```
Kitten
```bash
$ sudo ln -s /your/kitty/path/kitty.app/bin/kitten /usr/bin/kitten
```

2. Install kitty as your new x-terminal-emulator (This way the kitty will be able to see in the next command to choose your default terminal)
```bash
$ sudo update-alternatives --install /usr/bin/x-terminal-emulator x-terminal-emulator `which kitty` 50
```

3. Run the command below and type the number that show your kitty
```bash
$ sudo update-alternatives --config x-terminal-emulator
```
