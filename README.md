## Setup following tools in your local desktop
* Homebrew (Package Manager for macOS) - https://brew.sh/
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew tap caskroom/cask
```
* IntelliJ Idea Ultimate (IDE for development)
* Docker (Tool to containerize the applications) - http://tutorials.jenkov.com/docker/index.html
```
brew install docker docker-machine
brew cask install virtualbox virtualbox-extension-pack
brew cask install boot2docker
docker-machine create --driver virtualbox default
docker-machine env default
docker run hello-world
```
* Sublime Text Editor (Sophisticated text editor) - https://www.sublimetext.com/3
* JDK 8 (Java Development Kit) - https://www.oracle.com/technetwork/java/javase/downloads/index.html
* iterm2 (Terminal) - https://iterm2.com/ Configure Password Manager via Shell Integrations [link](https://medium.com/@ratchada.jududom/how-to-ssh-iterm2-with-password-manager-576b0452b493) to quickly enter passwords while login. Read more about Shell Integrations from [link](https://www.iterm2.com/documentation-shell-integration.html) if it excites you.
```
brew cask install iterm2
```
* Maven (Build automation tool) - https://maven.apache.org/
```
brew install maven
```
* Gradle (Build automation tool) - https://gradle.org/
```
brew install gradle
```
* Zsh (Unix shell) and Oh My Zsh (a delightful & open source framework for Zsh) - https://sourabhbajaj.com/mac-setup/iTerm/zsh.html
```
brew install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
zsh --version
upgrade_oh_my_zsh
```
Manage plugins [Plugins wiki page](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins) by updating ~/.zshrc. One can start with plugins=(gradle git git-extras aws). For more details, see [link](https://medium.com/ayuth/iterm2-zsh-oh-my-zsh-the-most-power-full-of-terminal-on-macos-bdb2823fb04c).
* Git (Free and open source distributed version control system) - http://tutorials.jenkov.com/git/index.html. Refer [git cheat sheet](https://github.github.com/training-kit/downloads/github-git-cheat-sheet/) for quick commands.
```
brew install git
```
* AWS CLI (A unified command line tool to manage your AWS services) - https://docs.aws.amazon.com/cli/latest/userguide/install-macos.html
```
curl -O https://bootstrap.pypa.io/get-pip.py
python3 get-pip.py --user
pip3 install awscli --upgrade --user
aws --version
```
* cURL (pronounced as curl) - An awesome command-line tool for transferring data from or to a server using various protocols.
```
brew install curl
```
* Ngrok [link](https://ngrok.com/) - A lightweight tool to create secure tunnel on your local machine along with a public URL you can use for browsing your local site.
```
brew cask install ngrok
```
* Snagit - Screen recording and screen capturing tool, will be useful for creating one demos.
```
brew cask install snagit
```
* MySQL - Relational database management system.
```
brew install mysql
```
* telnet - A protocol that allows you to connect to remote computers (called hosts) over a TCP/IP network (such as internet)
```
brew install telnet
```
* watch - Tool to run any designated command at regular intervals.
```
brew install watch
```
* tree [link](https://sourabhbajaj.com/mac-setup/iTerm/tree.html) - A command-line program used to recursively list or display the content of a directory in a tree-like format.
```
brew install tree
```
* wget - A free utility for non-interactive download of files from the web.
```
brew install wget
```
* jq [link](https://stedolan.github.io/jq/tutorial/) - JSON formatting tool or in other words sed for JSON data.
```
brew install jq
```
* ack [link](https://sourabhbajaj.com/mac-setup/iTerm/ack.html) - A search tool designed for code.
```
brew install ack
```
* MenuMeters - CPU, memory, disk, and network monitoring tools for Mac OS X.
```
brew cask install menumeters
```
* sshpass
```
brew install http://git.io/sshpass.rb
```
* Youtube-dl
```
brew install youtube-dl
```
* Telegram
```
brew cask install telegram
```
* Node.js
```
brew install node
```
* VLC
```
cask install vlc
```
* Fork - A fast and friendly git client for Mac and Windows - https://git-fork.com/
* Notion - A note-taking and collaboration application - https://www.notion.so/
* Localstack - https://github.com/localstack/localstack
```
pip install localstack
```
* ffmpeg
```
brew install ffmpeg
```
* Parquet tools
```
brew install parquet-tools
```
* Kap - Screen recorder - https://github.com/wulkano/kap
```
brew cask install kap
```
* fzf - A command-line fuzzy finder
```
brew install fzf

# To install useful key bindings and fuzzy completion:
$(brew --prefix)/opt/fzf/install
```
* bat - Cat clone with wings
```
brew install bat
```
* htop - Interactive text-mode process viewer for Unix systems
```
brew install htop
```
* piknik - Copy/paste anything over the network
```
brew install piknik
```
* fkill - Fabulously kill processes
```
npm install --global fkill-cli
```
* Broot - A better way to navigate directories
```
brew install broot
```

## Brew useful commands
* brew doctor
* brew search
* brew list
* brew remove <application-name>
* brew update
* ls /usr/local/Cellar/
* alias upgrade_all='brew update && brew upgrade && brew cask upgrade'
