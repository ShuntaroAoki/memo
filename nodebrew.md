# Nodebrew

## インストール

Mac なら homebrew でインストールできる．

```shellsession
$ brew install nodebrew
$ nodebrew setup
```

.bash_profile や .zprofile にパス設定を追加

```
export PATH=$HOME/.nodebrew/current/bin:$PATH
```

## コマンド

- Node.js のインストール
    - `$ nodebrew install-binary stable`
    - `$ nodebrew install-binary latest`
- インストールされている Node.js の確認
    - `$ nodebrew ls`
- インストール可能な Node.js の標示
    - `$ nodebrew ls-remote`
- 使用する Node.js の設定
    - `$ nodebrew use stable`
