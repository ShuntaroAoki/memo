# ffmpeg

## 動画の結合

``` shellsession
$ ffmpeg -f concat -safe 0 -i input_files.txt -c copy out.mp4
```

## 動画のトリミング

``` shellsession
$ ffmpeg -i <input.mp4> -vf crop=640:360:0:0 <output.mp4>
```

- `-vf`: エフェクトの指定
- `crop=w:h:x:y`: `w` と `h` は出力動画の幅と高さ，`x` と `y` は元動画の左上を (0, 0) としたときの出力動画の左上の位置

## 連番画像から動画を作成する

``` shellsession
$ ffmpeg -r 100 -i input_%d.jpg -c:v mpeg4 -qscale:v 1 -pix_fmt yuv420p -r 100 -threads 8 out.mp4
```

- `-r`: フレームレート (前半のは入力画像の，後半のは出力動画の fps)
- `-qscale:v`: 動画品質の指定 (1-31，1 が最高品質)
