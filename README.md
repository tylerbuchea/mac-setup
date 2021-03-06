## Developer Environment

**Bash script**

```language-bash
# Manual steps
# Complete these after you run the script
# Manually install Xcode from Appstore
# Manually install Android Studio from website
# In ~/.zshrc set plugins variable: plugins=(git z react-native)
# In ~/.dotfiles/.credentials change the git credentials to your own
# In ~/.hyper.js set shell: '/bin/zsh'
# In ~/.hyper.js add Powerline font like so: fontFamily: '"Inconsolata for Powerline", Menlo, ...
# Install Operator Mono and make ~/.hyperterm.js fontFamily: '"Operator Mono", "Inconsolata for Powerline"
# Install Operator Mono and make Atom > Preferences... > Editor > Font Family: Operator Mono

# Generate new SSH key:
ssh-keygen -t rsa -b 4096 -C "tyler@buchea.com"

# Official brew download & install command
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install Git
brew install git
brew cask

# Install brew tools and stuff
brew install fd
brew install redis
brew install mongodb
brew install nginx
brew install postgresql
brew install trash

# Install gui apps via brew cask
brew cask install alfred
brew cask install android-file-transfer
brew cask install caffeine
brew cask install chrome
brew cask install docker
brew cask install filezilla
brew cask install google-cloud-sdk
brew cask install hyper
brew cask install java
brew cask install mamp
brew cask install medis
brew cask install robo-3t
brew cask install postman
brew cask install psequel
brew cask install reactotron
brew cask install sequel-pro
brew cask install skype
brew cask install slack
brew cask install spectacle
brew cask install sqlitebrowser
brew cask install transmission
brew cask install vlc
brew cask install visual-studio-code

# VSCode Sync
# code --install-extension Shan.code-settings-sync 
# Settings Sync Gist ID Old: 9f0e91fe94851f2832495a364d0b3b47
# Settings Sync Gist ID New: 67c90dc3c78d50271e877232cbf1b418

# Download and install `nvm` with latest version of node
cd ~
touch ~/.bash_profile
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.1/install.sh | bash
cd ~/.nvm
git pull
source ~/.bash_profile
nvm install node

# Install Node packages
npm install -g create-react-app
npm install -g firebase-tools
npm install -g hpm-cli
npm install -g ios-deploy
npm install -g ios-sim
npm install -g markdown-pdf
npm install -g nodemon
npm install -g now
npm install -g pm2
npm install -g react-native-cli
npm install -g surge

# Install Hyper packages
hpm install hyper-clean

# Download and install `rbenv` with latest version of ruby
cd ~
brew install rbenv ruby-build
latestruby=$(rbenv install -l | grep -v - | tail -1 | xargs)
rbenv install $latestruby
rbenv global $latestruby

# Install ruby gems
gem install rails

# Install Zshell
cd ~
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
source ~/.zshrc

# Download and install dotfiles see repo README for more info
cd ~
git clone https://github.com/tylerbuchea/.dotfiles
echo "source ~/.dotfiles/.includes" >> ~/.zshrc
source ~/.zshrc

# Download and partially install theme
cd ~/Downloads
git clone https://github.com/powerline/fonts.git
cp fonts/Inconsolata/Inconsolata\ for\ Powerline.otf /Library/Fonts

# Create a dev folder
mkdir -p ~/dev

# Download and install developer credentials
cd ~/dev
git clone https://github.com/tylerbuchea/developer-credentials.git
```
