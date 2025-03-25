# Installing syntax highlighting and autosuggest plugins
## Recommended Easy Way
---
1. Install Oh My Zsh to manage packages
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
If asked "Do you want to change your default shell to zsh?", press Y

At the end your terminal should look like this:
![oh_my_zsh](https://github.com/mvbennett/zshconfigs/assets/94943459/85b3d874-ef0c-4c72-bf8c-aac00120e469)

```
exec zsh
```
2. Download script to install syntax highlighting and autosuggest plugins
```
git clone git@github.com:mvbennett/zshconfigs.git
```
3. Install syntax plugins
```
cd /zshconfigs && zsh install.sh
```

```
exec zsh
```

## Hard way
---
1. Download zsh syntax highlighting and zsh autosuggest directly
```
git clone https://github.com/zsh-users/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting
```
2. find directory of packages
```
pwd
```
3. construct and run command for adding plugin to zshrc
```
echo "source <insert path to package>/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
echo "source <insert path to package>/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
```

```
exec zsh
```
4. In your zshrc you should see two lines similar to the ones below (the path will differ)
```
source usr/mike/zsh-autosuggestions/zsh-autosuggestions.zsh
source usr/mike/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```


This repository is based on the one used by [Le Wagon](https://www.lewagon.com) students but with some major changes.

## Toolset

- [oh-my-zsh](http://ohmyz.sh/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [git](https://git-scm.com/)
