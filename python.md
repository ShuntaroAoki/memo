# Python 

## pip

- パッケージのインストール
    - `$ pip install <package>`
    - `$ pip install <package>==<version>`
- パッケージのアップグレード
    - `$ pip install --upgrade <package>`
    - `$ pip install --U <package>`
    - `--upgrade-strategy`: 依存パッケージのアップグレード方針を指定する
        - `only-if-needed` (デフォルト): アップグレードするパッケージの依存関係を満すために必要な場合だけ，依存パッケージをアップグレードする．
        - `eager`: 依存パッケージをすべてアップグレードする．

## pyenv

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

### pyenv + vertualenv による仮想環境

- 仮想環境の作成
    - `$ pyenv virtualenv 3.6.4 test`
    - Python 3.6.4 を元に仮想環境 test を作成する
- 仮想環境の削除
    - `$ pyenv uninstall 3.6.4/test`
- 仮想環境の切り替え
    - `$ pyenv global 3.6.4/test`
    - `$ pyenv local 3.6.4/test`

## pipenv

- パッケージのインストール
    - `$ pipenv install <package>`
    - `$ pipenv install <package>~=<version>`
    - `$ pipenv install`
        - Pipfile があるとき，必要なパッケージをすべてインストールする
- パッケージのアップデート
    - `$ pipenv update --outdated`
        - 更新のあるパッケージを表示する
    - `$ pipenv update`
        - 更新のあるパッケージをすべてアップデートする
    - `$ pipenv update <package>`
        - 指定されたパッケージをアップデートする
- Python のバージョンを指定する
    - `$ pipenv --python 3.6`
- pipenv シェル (仮想環境) の有効化
    - `$ pipenv shell`
- 仮想環境のパスを表示
    - `$ pipenv --venv`

参考:

- [Pipenvの基本的な使い方 — pipenv 2018.11.27.dev0 ドキュメント](https://pipenv-ja.readthedocs.io/ja/translate-ja/basics.html)
