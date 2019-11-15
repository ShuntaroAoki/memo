# yum

- パッケージのインストール
    - `# yum install <package>`
- パッケージのアップデート
    - `# yum update <package>`
    - `# yum update`
        - アップデート可能なパッケージをすべてアップデートする
- パッケージのアンインストール
    - `# yum remove <package>`
- パッケージの検索
    - `# yum search <hoge>`
- パッケージの情報を表示する
    - `# yum info <package>`
- パッケージの依存関係を表示する
    - `# yum deplist <package>`
- インストール済みパッケージの一覧表示
    - `# yum list installed`
- アップデートのあるパッケージの一覧表示
    - `# yum list updates`
- パッケージリポジトリの一覧を表示する
    - `# yum repolist`
    - `# yum repolist all` (disabled なリポジトリも表示する)
- パッケージリポジトリの情報を表示する
    - `# yum repoinfo <repository>`

## References

- [YUM コマンドチートシート (pdf)](https://access.redhat.com/sites/default/files/attachments/rh_yum_cheatsheet_1214_jcs_print-ja.pdf)
