My #! Linux .config folder.


A quick and dirty list of other things I do:
* (Macbook only) add `Option "TapButon1" "1"` and `Option "TapButton2" "2"` to /usr/share/X11/xorg.conf.d/50-synaptics.conf 
** Touchpad scrolling:  `Option "HorizScrollDelta" "-033"` & `Option "VertScrollDelta" "-033"`

* Install subime text 2 into /usr/share/ and add symlink to it from /usr/bin/
** `sudo ln -s /usr/share/sublime/sublime_text sublime`

```
# web stuff
sudo apt-get install chromium
sudo update-alternatives --config x-www-browser

# Apple only - isight firmware
sudo apt-get install isight-firmware-tools

# add dotfiles.  Includes:
# * Apple only key bindings. .Xmodmap
mv ~/.config/dotfiles/* .

# git config
git config --global color.ui true
git config --global user.email "eah13@mac.com"
git config --global user.name "Elliott Hauser"
git config --global core.editor 'nano'

# in ~/.ssh:
ssh-keygen -t rsa -C "eah13@mac.com"
sudo apt-get install xclip
xclip -sel clip < ~/.ssh/id_rsa.pub
# test
ssh -T git@github.com

# clone repos
mkdir ~/git
cd ~/git && git clone git@github.com:eah13/subluser.git
cd ~/git && git clone git@github.com:eah13/forkshop.git




```

### TODO
Swipe horizonatally to switch 













