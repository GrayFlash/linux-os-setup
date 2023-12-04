# Basic dev environment

Automate this stuff!

## browser & nvim

```
sudo pacman -Syu
sudo pacman -S brave-browser

sudo pacman -Syu
sudo pacman -S neovim

cd .config && cp -r codes/grayflash/linux-os-setup/nvim nvim
```

## vscode

```
curl -L -O https://aur.archlinux.org/cgit/aur.git/snapshot/visual-studio-code-bin.tar.gz
tar -xvf visual-studio-code-bin.tar.gz
cd visual-studio-code-bin/ && makepkg -si
cd .. && rm -rf visual-studio-code-bin.tar.gz 
```

## git setup

```
gpg --full-generate-key
gpg --list-secret-keys --keyid-format=long
gpg --armor --export <KEY-ID>
# <Add GPG key to github account>
git config --global credential.helper /usr/lib/git-core/git-credential-libsecret
# <Generate and use a Personal Access Token>
git config --global user.email "gk74533@gmail.com" 
git config --global user.name "GrayFlash"
git clone https://github.com/GrayFlash/travel-log.git
```

## python

```
sudo pacman -Syu python-pip
pip -m venv env
python -m venv env
source env/bin/activate
pip install jupyter
```

## node

```
sudo pacman -Syu nvm
echo 'source /usr/share/nvm/init-nvm.sh' >> ~/.bashrc
nvm --version
nvm install 20
```

## golang

## java

## docker

## kubectl <> gcs <> aws
