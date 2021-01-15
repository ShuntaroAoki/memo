# Anaconda

- <https://www.anaconda.com/>

| 機能 | コマンド |
|:--|:--|
| Anaconda の情報表示 | `$ conda info` |
| 環境の作成 | `$ conda create -n <env> python`<br>`$ conda create -n <env> numpy scipy`<br>`$ conda create -n <env> anaconda`<br>`$ conda create -n <env> python=3.7`<br>`$ conda create -n <env> --clone <source_env>`<br>`$ conda create -n <env> -f env.yaml` |
| 環境の削除 | `$ conda remove -n <env> --all` |
| 環境の一覧表示 | `$ conda info --envs`<br>`$ conda info -e` |
| 環境の切り替え | `$ conda activate <env>`<br>`$ conda deactivate` |
| パッケージのインストール | `$ conda install -n <env> <package>` |
| パッケージのインストール (バージョン指定) | `$ conda install -n <env> <package>=<version>` |
| パッケージのインストール (バージョンとビルド指定) | `$ conda install -n <env> <package>=<version>=<build>` |
| パッケージのインストール (channel 指定) | `$ conda install -n <env> -c <channel> <package>` |
| パッケージのアップデート | `$ conda update -n <env> <package>` |
| パッケージのアンインストール | `$ conda uninstall -n <env> <package>` |
