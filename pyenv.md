# pyenv

- Python のインストール
    - `$ pyenv install <python>`
- Python と環境のアンインストール
    - `$ pyenv uninstall <python>`
- インストール可能な Python の一覧表示
    - `$ pyenv install --list`
- インストール済み Python の一覧表示
    - `$ pyenv versions`
- Python の切り替え
    - `$ pyenv global <python>`
    - `$ pyenv local <python>`
- ローカル Python の指定解除
    - `$ pyenv local --unset`

## pyenv + vertualenv による仮想環境

- 仮想環境の作成
    - `$ pyenv virtualenv 3.6.4 test`
    - Python 3.6.4 を元に仮想環境 test を作成する
- 仮想環境の削除
    - `$ pyenv uninstall 3.6.4/test`
- 仮想環境の切り替え
    - `$ pyenv global 3.6.4/test`
    - `$ pyenv local 3.6.4/test`
