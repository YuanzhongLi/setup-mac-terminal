## 1.Xcodeをインストール
```
# bash
xcode-select --install
```

## 2. hombrew install
参照: https://brew.sh/index_ja

homebrewへのpathを追加
```
# .bash_profile
export PATH=/usr/local/bin:$PATH
```

## 3.Git install
```
# bash
brew install git
```

## 4.terminal ブランチ名/ディレクトリ名表示
参照：https://qiita.com/koyopro/items/3fce94537df2be6247a3

```
# .bash_profile
export TERM="xterm-color"

source /usr/local/Cellar/git/2.20.1/etc/bash_completion.d/git-prompt.sh
source /usr/local/Cellar/git/2.20.1/etc/bash_completion.d/git-completion.bash

GIT_PS1_SHOWDIRTYSTATE=true
export PS1='\[\e[0;33m\]\u\[\e[0m\] \[\e[0;32m\]\h\[\e[0m\] \[\e[0;34m\]\w\[\e[0m\] $(__git_ps1 "\[\033[31m\]%s\[\033[0m\]")\n\[\033[35m\]\$\[\033[0m\] '
```
## 5.terminal tab補完 大文字小文字区別なし
```
# .inputrc
set completion-ignore-case on
```
