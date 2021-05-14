# commitの様々なオプション

0. 準備
### フォークする
<img width="1435" alt="スクリーンショット 2021-05-15 3 35 28" src="https://user-images.githubusercontent.com/71377103/118317147-a7044800-b532-11eb-8497-b5de4df7c35f.png">

### クローンする
<img width="1435" alt="スクリーンショット 2021-05-15 3 36 41" src="https://user-images.githubusercontent.com/71377103/118317154-a9ff3880-b532-11eb-8aae-c165e806e01a.png">
```
git clone <リポジトリURL>
```

### ブランチをきる
```
git switch -c feature/01
```

## -m
コミットメッセージをつける

## -a
変更されたファイルを検出し(新規に追加されたファイルを除く)、git add と git commit を同時に実行する。
```
echo 'Hello World!!' > sample.txt
```
```
git commit -am 'commit No.1'
```
```
git log
```
<img width="1435" alt="スクリーンショット 2021-05-15 4 00 08" src="https://user-images.githubusercontent.com/71377103/118316857-4ecd4600-b532-11eb-999f-718bea562b20.png">

## --amend
直前のコミットを上書きしてコミットする。
```
echo 'Change!!' > sample.txt
```
```
git commit --amend -am 'commit No.2'
```
```
git log
```
<img width="1435" alt="スクリーンショット 2021-05-15 4 01 25" src="https://user-images.githubusercontent.com/71377103/118316881-57258100-b532-11eb-88e7-0242dfb4632f.png">

