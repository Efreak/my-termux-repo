This is a termux repo I'm playing with. It's quite unlikely anything here will ever be updated; all packages are created manually with `termux-create-package`, and I'm lazy. Most of my nonpackaged software actually goes in ~/.local/bin so I can transfer it between devices with git.

```
wget https://github.com/Efreak/my-termux-repo/raw/main/gpg-key -qO-|apt-key add
```

A number of apps require ncurses, some of them may not notify you of this, while others will be statically compiled. use `ldd` to check if in doubt. static binaries are larger; some are stripped and compressed with upx.

These apps will likely not ever be updated, as some of them are just things I'm playing with. Others are simply rust software I wanted to install on multiple devices.

Included software is listed below; particularly useful or interesting software is *italicized*.

- amfora
- atuin
- *cargo-trim* - cleans up cargo caches
- cargo-whatfeatures
- *cbonsai* - draw trees in the terminal
- damo
- dekryptize - fake decryption animation using ncurses
- *freesweep* - minesweeper
- git-anger-management
- *git-interactive-rebase-tool*
- git-stack
- *git-summary*
- gitopen
- gitty
- *goful*
- hoard-rs
- *imgcurses*
- macchina
- *mandown*
- mazegenerator
- mnem
- ncdu
- *neo*
- os_info
- pipes.sh
- pipesX.sh
- *powerline-rs*
- *pspg*
- rocketfetch
- rpipes
- ru
- *scdoc*
- shed
- *steamguard-cli*
- stor-age
- sttr
- terminal-mines
- tiny-moon-runner
- tuxfetch
- vadersay
- weave.sh
- web-grep
- *wttr*
- xi-core
- xi-syntect-plugin
- yadf
- yarf-fetch
- yayagram

TODO:

- [tetris](https://github.com/samtay/tetris)?
- fix xi-term metadata, apt doesnt like version without a digit
- [ncursesFM](https://github.com/FedeDP/ncursesFM) requires libudev...
- [maze5](http://www.fiveoclock.de/?page_id=81) requires cairo and xorg stuff. Add parentheses to build/Sconscript:32 to enable building with python3 scons. install scons with pip/pipx.
- [tetris](https://github.com/brenns10/tetris) requires libsdl for sound
- [ngp](https://github.com/jonathanklee/ngp) is an ncurses based grep viewer that requires more pthread than is available...
- [bookwyrm](https://github.com/tmplt/bookwyrm) - download books from the internet

Other:

- pipx - `python -m pip install pipx`
