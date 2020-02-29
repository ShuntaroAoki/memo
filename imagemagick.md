# ImageMagick

## 画像形式の変換

``` shellsession
$ convert hoge.jpg hoge.png
$ convert -density 200 hoge.eps hoge.png
```

## 画像サイズの変更

``` shellsession
$ convert -geometry 1000x500 hoge.png hoge_resize.png
$ convert -geometry 50% hoge.png hoge_resize.png
```

## 画像の結合

``` shellsession
$ convert +append images_*.jpg images_all.jpg  # 横に結合
$ convert -append images_*.jpg images_all.jpg  # 縦に結合
```

## GIF アニメを作成する

``` shellsession
$ convert -delay 200 -loop 0 images_*.jpg images_all.gif
```

- `-delay` の単位は 1/100 秒
- `-loop 0` で無限にループする
