# GPG

## Table of Contents
* [Main commands](#main-commands)
* [Export and Import](#export-and-import)
* [Setup GPG on MacOS](#setup-gpg-on-macos)

## Main commands
````bash
gpg --help
gpg --version
```````
````bash
killall gpg-agent
```````
````bash
gpg --full-generate-key
gpg --list-keys
gpg --list-secret-keys
gpg --list-sigs
````
Sign all commits with your key
````bash
git config --global user.signingkey <your-key>
git config --global commit.gpgsign true
````
## Export and Import
````bash
gpg --export --armor <your-key or email> > public.gpg
gpg --export-secret-keys --armor <your-key or email> > private.gpg
````
````bash
gpg --import public.gpg
gpg --import private.gpg
````

## add correct GPG ID to gitconfig

List all possible keys
```bash
gpg --list-secret-keys --keyid-format=long
```

Possible result
```
/home/sascha/.gnupg/pubring.kbx
-------------------------------
sec   ed25519/D3B9288EA4CD1F88 2022-10-12 [SC]
      A583F85EC13EDF2142C72AEAD3B9288EA4CD1F88
uid                 [ unknown] Sascha Heinemann <sascha.heinemann@globalways.net>
ssb   cv25519/072AA55BA2A334E6 2022-10-12 [E]
```
use the string after the slash in the _sec_ output in the gitconfig

## Setup GPG on MacOS

### Steps on 🍎 MacOS
Things are easyier with [Homebrew](https://brew.sh/) installed.
* [Install GPG on Macos](#install-gpg-on-macos)
* [Install PinEntry on Macos](#install-pinentry-on-macos)

### Install GPG on Macos
```bash
brew install gpg
```
### Install PinEntry on Macos
For GUI or e.g. vscode and other integrations
```bash
brew install pinentry-mac
```
**Follow the Prompt** to add your GPG program path

e.g.
```bash
echo 'pinentry-program /opt/homebrew/bin/pinentry-mac' >> ~/.gnupg/gpg-agent.conf
```