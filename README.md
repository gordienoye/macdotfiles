macdotfiles
===========

Another dotfiles repository styled after https://github.com/stash/dotfiles

Setting up:
===========
1. Clone the repo with `--recursive` (or run `git submodule update --init --recursive` after cloning)
2. copy `gitconfig` to `~/.gitconfig`, add your github key
3. link other dotfiles to `~`
4. link `.git/hooks` to `githooks`

Things to remember to do:
=========================

Install homebrew and a couple of necessary things:
- http://brew.sh/
  - `brew install coreutils git ack python`
  - `brew install vim --with-python --with-ruby --with-perl`
    - note that vim should be done after python for the correct bindings

Powerline demands the following:
- `pip install git+git://github.com/Lokaltog/powerline`
- change the terminal type that iTerm2 reports (Profiles -> Terminal -> Report Terminal Type) to be `xterm-256color`.
- install the Powerline fonts in the Macintosh (if they are not already there).
  - Currently using Inconsolata from https://github.com/Lokaltog/powerline-fonts
  - Update iTerm2 font to be Inconsolata 14pt for Regular and Non-ASCII font.

Pathogen (https://github.com/tpope/vim-pathogen) is installed by default and the following bundles are added
- syntastic: https://github.com/scrooloose/syntastic
- powerline: https://github.com/Lokaltog/powerline
- vim-javascript-syntax: https://github.com/jelera/vim-javascript-syntax

syntastic needs to have JSHint installed.
- `npm install -g jshint`
