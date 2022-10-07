# Apple M1
* poetry에서 다른 버전의 python을 보고 있다면
1. xcode 업데이트
1. `/usr/sbin/softwareupdate --install-rosetta agree-to-license`
1. `ls /opt/homebrew/Cellar`
1. `brew uninstall --ignore-dependencies --force python@3.10`
1. `brew uninstall --force poetry`
1. `brew doctor`
1. `brew cleanup`
1. `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
1. `echo 'alias brew="arch -x86_64 /usr/local/bin/brew"' >> ~/.alias`
1. `source ~/.zshrc`
