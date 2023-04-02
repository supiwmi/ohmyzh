# ohmyzh
How to use ohmyzh on mac

[Check out Top 12 Oh My Zsh Themes For Productive Developers](https://travis.media/top-12-oh-my-zsh-themes-for-productive-developers/#20210921-gozilla)

### 1.  Install oh my zh 

`sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

### 2. Install zsh autosuggestion
`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

Once install then we need to add the plugin to the list of plugins for Oh My Zsh to load (inside ~/.zshrc):

```
plugins=( 
    # other plugins...
    zsh-autosuggestions
)
```
### 3. Start a new terminal session.
`press Command+N`


### Tip: 

To run code from termal see [VSCode on Mac](https://code.visualstudio.com/docs/setup/mac#:~:text=Launching%20from%20the%20command%20line,code'%20command%20in%20PATH%20command.)


# Customize for bettert Mac Terminal

1. Upgrade Howebrew on your mac The Missing Package Manager for macOS (or Linux) [see more detail of Homebrew](https://brew.sh/)

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

`brew --version`

```
Homebrew 4.0.10-119-g931327d
Homebrew/homebrew-core (git revision c96024f2ce4; last commit 2022-05-04)
Homebrew/homebrew-cask (git revision 7045cdb1a2; last commit 2022-05-04)
```
2. We are going to use iTerm2 so we need to install it with brew

`brew install --cask iterm2`

3. Install git
`brew install git`

4. Install ohmyzh

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

5. Install PowerLevel10K Theme for Oh My Zsh

`git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k`

Now that it's installed, open the "~/.zshrc" file with your preferred editor and change the value of "ZSH_THEME" as shown below:

`ZSH_THEME="powerlevel10k/powerlevel10k"`

To reflect this change on your terminal, restart it or run this command:

`source ~/.zshrc`

6. Install Meslo Nerd Font
Install the font by pressing "y" and then quit iTerm2.
Update VSCode Terminal Font (Optional)
Open settings.json and add this line:

`"terminal.integrated.fontFamily": "MesloLGS NF"`

7. Configure PowerLevel10K

Restart iTerm2. You should now be seeing the PowerLevel10K configuration process. If you don't, run the following:

`p10k configure`

8. Follow the instructions for the PowerLevel10K configuration to make your terminal look as desired.
Increase Terminal Font Size
* 1. Open iTerm2 preferences
* 2. Go to Profiles > Text
* 3. I increase my font size to about 20px
Change iTerm2 Colors to My Custom Theme
1. Open iTerm2
2. Download my color profile by running the following command (will be added to Downloads folder):

`curl https://raw.githubusercontent.com/josean-dev/dev-environment-files/main/coolnight.itermcolors --output ~/Downloads/coolnight.itermcolors`

3. Open iTerm2 preferences
4. Go to Profiles > Colors
5. Import the downloaded color profile (coolnight)
6. Select the color profile (coolnight)

You can find other themes here: [Iterm2 Color Schemes](https://iterm2colorschemes.com/)

9. Install ZSH Plugins

Install zsh-autosuggestions:

`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

Install zsh-syntax-highlighting:

`git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`

Open the "~/.zshrc" file in your desired editor and modify the plugins line to what you see below.

`plugins=(git zsh-autosuggestions zsh-syntax-highlighting web-search)`

Load these new plugins by running:
`source ~/.zshrc`

### You're Done!
You should have a much better terminal experience!