# base16-tilix

This repository is meant to work with 
[chriskempson/base16](https://github.com/chriskempson/base16). It provides a 
simple template that can be used with the base16 colour schemes to generate a 
functional config file for [gnunn1/tilix](https://github.com/gnunn1/tilix).

To use, you can symlink the directory to ``~/.config/tilix/schemes``:

```bash
git clone https://github.com/karlding/base16-tilix.git && cd base16-tilix/
cd tilix/
BASE16_TILIX_THEME_DIR=`pwd`
mkdir -p ~/.config/tilix/schemes
cd ~/.config/tilix/schemes
ln -sf $BASE16_TILIX_THEME_DIR/*.json .
```

Or you can copy one of the config files in ``tilix/`` or use ``wget``:

```bash
mkdir -p ~/.config/tilix/schemes
cd ~/.config/tilix/schemes
wget https://raw.githubusercontent.com/karlding/base16-tilix/master/tilix/base16-ocean.json
```
