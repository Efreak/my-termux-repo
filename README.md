This is a termux repo I'm playing with. It's quite unlikely anything here will ever be updated; all packages are created manually with `termux-create-package`, and I'm lazy. Most of my nonpackaged software actually goes in ~/.local/bin so I can transfer it between devices with git.

```
wget https://github.com/Efreak/my-termux-repo/raw/main/gpg-key -qO-|apt-key add
```


TODO:

- [tetris](https://github.com/samtay/tetris)?
- fix xi-term metadata, apt doesnt like version without a digit
- [ncursesFM](https://github.com/FedeDP/ncursesFM) requires libudev...
