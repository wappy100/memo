# mac初期設定

### homebrew

```shell
sudo mkdir -p /usr/local/bin/
vim ~/.bash_profile
----
export PATH=/usr/local/bin:$PATH
----

ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
source ~/.bash_profile

wappy100:~ wappy100$ brew -v
Homebrew 0.9.5
```

### zsh

```shell
brew install zsh

sudo vim /etc/shells
----
/usr/local/bin/zsh
----

chsh -s /usr/local/bin/zsh
```

### iterm2

```shell
http://iterm2.com/
```

### oh-my-zsh

```shell
curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
```

### solarized

```shell
mkdir ~/Documents/work/solarized; cd ~/Documents/work/solarized/
git clone git://github.com/altercation/solarized.git

# iterm2, .vimrc に適用
```

### vagrant

```shell
http://www.vagrantup.com/downloads.html
```

### virtualbox

```shell
https://www.virtualbox.org/wiki/Downloads
```

### google ime

```shell
http://www.google.co.jp/ime/index.html
```

### neobundle

```shell
mkdir -p ~/.vim/bundle
git clone https://github.com/Shougo/neobundle.vim ~/.vim/bundle/neobundle.vim
```

### .vimrc

```shell
"---------------------------
" Start Neobundle Settings.
"---------------------------
" bundleで管理するディレクトリを指定
set runtimepath+=~/.vim/bundle/neobundle.vim/
 
" Required:
call neobundle#begin(expand('~/.vim/bundle/'))
 
" neobundle自体をneobundleで管理
NeoBundleFetch 'Shougo/neobundle.vim'
 
" 今後このあたりに追加のプラグインをどんどん書いて行きます！！"
 
call neobundle#end()
 
" Required:
filetype plugin indent on
 
" 未インストールのプラグインがある場合、インストールするかどうかを尋ねてくれるようにする設定
" 毎回聞かれると邪魔な場合もあるので、この設定は任意です。
NeoBundleCheck
 
"-------------------------
" End Neobundle Settings.
"-------------------------
```

