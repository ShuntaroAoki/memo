# dd

```
$ dd if=<input> of=<output> bs=<ブロックサイズ (バイト)> count=<if から読み込むブロック数>
```

- `skip`: 入力からスキップするブロック数
- `seek`: 出力でスキップするブロック数

## Examples

ファイルに書き込む:

```
$ echo -n "hoge" | dd of=<ファイル> bs=1 seek=<書き込む位置のオフセット> conv=notrunc
```

ファイルの一部を取り出す:

```
$ dd if=<元ファイル> of=<output> bs=1 count=<取り出すデータサイズ> skip=<取り出す部分のオフセット>
```

ファイルの末尾をゼロ埋めする:

```
$ dd if=/dev/zero of=<ファイル> bs=1 count=<ゼロ埋めするサイズ> seek=<ファイルサイズ>
```
