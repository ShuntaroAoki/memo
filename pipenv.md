# pipenv

- 仮想環境の作成
    - `$ pipenv --python  <version>`
    - `$ pipenv install --python <version>`
- pipenv シェル (仮想環境) の有効化
    - `$ pipenv shell`
- 仮想環境のパスを表示
    - `$ pipenv --venv`
- 仮想環境の削除
    - `$ pipenv --rm`
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

参考:

- [Pipenvの基本的な使い方 — pipenv 2018.11.27.dev0 ドキュメント](https://pipenv-ja.readthedocs.io/ja/translate-ja/basics.html)
- [Pythonで、Pipenvを使う - Narito Blog](https://narito.ninja/blog/detail/58/)
