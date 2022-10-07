# Apple M1
## poetry
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
* poetry bad interpreter: No such file or directory 발생시
1. `/opt/homebrew/bin/brew uninstall poetry`
1. `arch -x86_64 /usr/local/Homebrew/bin/brew poetry`
1. `brew link poetry`
## Stable diffustion
1. `git clone -b apple-silicon-mps-support https://github.com/bfirsh/stable-diffusion.git`
1. `cd stable-diffusion`
1. `mkdir -p models/ldm/stable-diffusion-v1/`
1. `pip install virtualenv`
1. `python -m virtualenv venv`
1. `source venv/bin/activate`
1. `pip install -r requirements.txt`
1. sd-v1-4.ckpt 다운 받고 `https://huggingface.co/CompVis/stable-diffusion-v-1-4-original#download-the-weights`
1. `models/ldm/stable-diffusion-v1/model.ckpt`로 저장
* 참고 : https://replicate.com/blog/run-stable-diffusion-on-m1-mac
