# macOS

## ***개발환경 설정(CLI)***

### ***Dock***
```bash
defaults write com.apple.Dock position-immutable		-bool yes && killall Dock
sleep 1
defaults write com.apple.Dock size-immutable			-bool yes && killall Dock
sleep 1
defaults write com.apple.Dock contents-immutable		-bool yes && killall Dock
sleep 1
```

### ***Homebrew***
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/guangmin/.zprofile
```
```
eval "$(/opt/homebrew/bin/brew shellenv)"
```

### ***Oh My Zsh***
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

```
git clone https://github.com/dracula/iterm.git
```

### ***Homebrew Formulae***
- desktop
```
brew install --cask alfred bartender iterm2 typora google-chrome docker intellij-idea visual-studio-code
```

- laptop
```
brew install --cask aldente alfred bartender iterm2 typora google-chrome docker intellij-idea visual-studio-code
```

- business
```
brew install --cask microsoft-teams slack
```

### ***SDKMAN***
```bash
curl -s "https://get.sdkman.io" | bash
```

```
source "/Users/guangmin/.sdkman/bin/sdkman-init.sh"
```
```
sdk install java 17.0.10-oracle
```
