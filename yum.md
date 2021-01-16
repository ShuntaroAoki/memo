# yum

## コマンド

| 機能 | コマンド |
|:--|:--|
| パッケージのインストール | `# yum install <package>` |
| パッケージのインストール | `# yum update <package>` |
| アップデート可能なパッケージのすべてアップデート | `# yum update` |
| パッケージのアンインストール | `# yum remove <package>` |
| パッケージの検索 | `# yum search <hoge>` |
| パッケージの情報を表示する | `# yum info <package>` |
| パッケージの依存関係を表示する | `# yum deplist <package>` |
| ファイルを含むパッケージを表示する | `# yum provides <file>` |
| インストール済みパッケージの一覧表示 | `# yum list installed` |
| アップデートのあるパッケージの一覧表示 | `# yum list updates` |
| パッケージリポジトリの一覧を表示する | `# yum repolist` |
| パッケージリポジトリの一覧を表示する (disabled なリポジトリも表示する) | `# yum repolist all` |
| パッケージリポジトリの情報を表示する | `# yum repoinfo <repository>` |
| キャッシュ (rpm ファイル、ヘッダファイルなど) を削除する | `# yum clean all` |

## References

- [YUM コマンドチートシート (pdf)](https://access.redhat.com/sites/default/files/attachments/rh_yum_cheatsheet_1214_jcs_print-ja.pdf)
- [yumコマンドの基本操作とリポジトリの追加・削除方法のまとめ \| 己で解決！泣かぬなら己で鳴こうホトトギス](https://onoredekaiketsu.com/yum-command-and-repository/)
- [yum update と yum upgradeの違い（ついでにDebianも） - Qiita](https://qiita.com/aki3061/items/4e0597505097538b6e2c)
