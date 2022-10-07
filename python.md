# Apple M1
* poetry에서 다른 버전의 python을 보고 있다면
1. xcode 업데이트
1. `/usr/sbin/softwareupdate --install-rosetta agree-to-license`
1. `ls /opt/homebrew/Cellar`
1. `brew uninstall --ignore-dependencies --force python@3.10`
1. `brew uninstall --force poetry`
1. `brew doctor`
1. `brew cleanup`
