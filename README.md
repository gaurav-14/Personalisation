# Personalisation
Repositories containing personalisation files like tmux config file, bashrc file, etc.


## Why to use tmux plugins?
* Ease access to useful theme.
* Easier to manage and customise themes

## How to use tmux plugins ?
### Install tmux plugins manager
```bash
$ git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```
#### Put this at the bottom of ~/.tmux.conf ($XDG_CONFIG_HOME/tmux/tmux.conf works too):
#### List of plugins
```
set -g @plugin 'tmux-plugins/tpm'
set -g @plugin 'tmux-plugins/tmux-sensible'
```
#### Other examples:
#### set -g @plugin 'github_username/plugin_name'
#### set -g @plugin 'github_username/plugin_name#branch'
#### set -g @plugin 'git@github.com:user/plugin'
#### set -g @plugin 'git@bitbucket.com:user/plugin'

### Initialize TMUX plugin manager (keep this line at the very bottom of tmux.conf)
```
run '~/.tmux/plugins/tpm/tpm'
```
### type this in terminal if tmux is already running
```
tmux source ~/.tmux.conf
```
