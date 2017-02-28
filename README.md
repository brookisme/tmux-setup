
### setup
```bash
pushd ~/
git clone https://github.com/brookisme/tmux-setup.git
mv tmux-setup/tmux.conf .tmux.conf
rm tmux-setup/
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
popd
```

### tmux
```bash
# start session
tmux
# install plugins
C-a P (shift p)
```
