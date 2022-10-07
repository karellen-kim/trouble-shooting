# Apple M1
1. xcode 업데이트
1. 로제타 설치 : `/usr/sbin/softwareupdate --install-rosetta agree-to-license`
1. `ls /opt/homebrew/Cellar`
1. 다른 버전 python 삭제 : `brew uninstall --ignore-dependencies --force python@3.10`
1. `brew uninstall --force poetry`
1. `brew doctor`
1. `brew cleanup`
1. homebrew 재설치 : `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
1. python@3.10 재설치 : `arch -x86_64 /usr/local/Homebrew/bin/brew install python@3.10`
1. poetry 재설치 : `arch -x86_64 /usr/local/Homebrew/bin/brew install poetry`
1. `echo 'alias brew="arch -x86_64 /usr/local/Homebrew/bin/brew"' >> ~/.zshrc`
