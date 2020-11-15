# pip

- パッケージのインストール
    - `$ pip install <package>`
    - `$ pip install <package>==<version>`
- パッケージのアップグレード
    - `$ pip install --upgrade <package>`
    - `$ pip install --U <package>`
    - `--upgrade-strategy`: 依存パッケージのアップグレード方針を指定する
        - `only-if-needed` (デフォルト): アップグレードするパッケージの依存関係を満すために必要な場合だけ，依存パッケージをアップグレードする．
        - `eager`: 依存パッケージをすべてアップグレードする．
