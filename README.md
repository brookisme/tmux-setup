
### setup
```bash
pushd ~/
rm -rf .tmux*
git clone https://github.com/brookisme/tmux-setup.git
mv tmux-setup/tmux.conf .tmux.conf
rm -rf tmux-setup/
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
popd
```

### tmux
```bash
# start session
tmux
# install plugins
C-a I (shift i)
```

-------------
### plugins

#### https://github.com/tmux-plugins/tmux-logging
```bash
prefix + shift + p   toggles-log     
```


#### https://github.com/tmux-plugins/tmux-pain-control/
```bash
# Resizing panes
prefix + shift + h   resize current pane to the left
prefix + shift + j   resize current pane in the up direction
prefix + shift + k   resize current pane in the down direction
prefix + shift + l   resize current pane to the right


#Splitting panes
prefix + |           split current pane horizontally
prefix + -           split current pane vertically


Swapping windows
prefix + <           moves current window one position to the left
prefix + >           moves current window one position to the right
```

#### https://github.com/tmux-plugins/tmux-yank
```bash
prefix + y           copies text from the command line to clipboard
```