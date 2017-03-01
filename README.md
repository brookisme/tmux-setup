
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
