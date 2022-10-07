# Apple M1
1. xcode 업데이트
1. `/usr/sbin/softwareupdate --install-rosetta agree-to-license`
1. `conda create -n ml python=3.9.6`
1. `conda activate ml`
1. `brew install poetry`
* poetry에서 다른 버전의 python을 보고 있다면
1. `ls /opt/homebrew/Cellar`
1. `brew uninstall --force python@3.10`
2. `brew uninstall --force poetry`
