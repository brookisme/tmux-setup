
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

### layouts

Save your layout (see [dot-tmux-slash-layout-a](https://github.com/brookisme/tmux-setup/blob/master/dot-tmux-slash-layout-a) for an example) to `.tmux/layout_a`.  Then add
```bash
bind S source-file ~/.tmux/layout_a
```
to your `.tmux.conf` file.

Now, once inside the tmux session just type `ctrl-a Shift-S` and you will automatically see your new layout.  

Note you will have re-run your conf file: `C-a I (shift i)`.

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