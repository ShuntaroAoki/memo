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

``` shellsession
$ convert -resize 256x256 input.png output.png   # 縦横比を維持し、指定サイズに収まるようにリサイズ
$ convert -resize 256x256! input.png output.png  # 縦横比を無視してリサイズ
```

複数画像を一括変換:

``` shellsession
$ mogrify -resize 1920x1080 *.png
```

## 画像の結合

``` shellsession
$ convert +append images_*.jpg images_all.jpg  # 横に結合
$ convert -append images_*.jpg images_all.jpg  # 縦に結合
```

## RGB -> RGBA

``` shellsession
$ convert rgb.png -define png:color-type=6 rgba.png
```

## GIF アニメを作成する

``` shellsession
$ convert -delay 200 -loop 0 images_*.jpg images_all.gif
```

- `-delay` の単位は 1/100 秒
- `-loop 0` で無限にループする
