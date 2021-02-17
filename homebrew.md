# Homebrew

## Homebrew のインストール

    $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

## コマンド

| 機能 | コマンド |
|:--|:--|
| Formula のインストール | `$ brew install <formula>` |
| Formula のアップデート | `$ brew upgrade <formula>` |
| 更新のある formula をすべてアップデートする | `$ brew upgrade` |
| Formula のアンインストール | `$ brew uninstall <formula>` |
| 検索 | `$ brew search text` |
| 検索 (正規表現検索) | `$ brew search /text/` |
| Formula の情報表示 | `$ brew info <formula>` |
| Formula の依存関係の表示 |  `$ brew deps <formula>` |
| インストール済み formula の一覧表示 | `$ brew list` |
| 更新のある formula の一覧表示 | `$ brew outdated` |
| Outdated な formula の削除 | `$ brew cleanup`<br>`$ brew cleanup -n` (dry run) |
| Homebrew のアップデート | `$ brew update` |
| Tap (リポジトリ) の一覧表示 | `$ brew tap` |
| Tap (リポジトリ) の追加 | `$ brew tap <user/repo>`<br>`$ brew tap <user/repo> <URL>` |
| Tap (リポジトリ) の削除 | `$ brew untap <user/repo>` |
| Homebrew の診断 | `$ brew doctor` |

## References

- <https://brew.sh/index_ja>
- [The missing package manager for macOS (or Linux) — The missing package manager for macOS (or Linux)](https://brew.sh/)
- [Homebrew使い方まとめ - Qiita](https://qiita.com/vintersnow/items/fca0be79cdc28bd2f5e4)
