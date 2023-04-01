# ohmyzh
How to use ohmyzh on mac

[check out Top 12 Oh My Zsh Themes For Productive Developers](https://travis.media/top-12-oh-my-zsh-themes-for-productive-developers/#20210921-gozilla)

### 1.  Install oh my zh 

sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

### 2. Install zsh autosuggestion
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

Once install then we need to add the plugin to the list of plugins for Oh My Zsh to load (inside ~/.zshrc):

```
plugins=( 
    # other plugins...
    zsh-autosuggestions
)

```
### 3. Start a new terminal session.
