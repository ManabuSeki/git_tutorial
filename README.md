#GitHub練習

##追加修正を行う場合の流れ
1. ローカルでmasterから新しいブランチを作成する。例えばb1というブランチを作成したとする。
2. ローカルのb1ブランチに修正をコミットする
3. GitHubにb1ブランチを作成し、そこにpushする
4. GitHub上で、b1からmasterにPullRequestを作成する
5. PullRequestを別の人がレビューする
6. 必要があればローカルのb1ブランチにさらに修正を行い、GitHubのb1ブランチにpushする
7. レビューが通ればPullRequestをマージする

コマンドラインで言うと以下。

1. ローカルでmasterから新しいブランチを作成する。例えばb1というブランチを作成したとする。
```
#現在どこのbranchにいるのか確認する
$git branch

#その後masterブランチに移動する
$git checkout master

#移動できない場合　コミットしてない場合が多い

#移動できているか確認する
$git branch

#新しいブランチを作成する
$git branch b1

#b1ブランチに移動する
$git checkout b1

##ブランチの新規作成と移動を同時に行うには以下のように-bオプションを付ける
$git checkout -b b1
```
修正  
修正  
修正  

2. ローカルのb1ブランチに修正をコミットする
```
#特定ファイルの修正を行いコミットする
$git add *****

#一度にすべてコミットする場合
$git add .

#修正したファイルのみコミットする場合(新規ファイルは含まれない)
$git add -u

$git commit

#コメントを一行で挿入する場合以下ののように-mオプションを利用できる
$git commit -m 'ここにコメントを入れる'

#直接　新規追加・変更ファイルをコミットするには-aオプションを利用できる
$git commit -a

#コメントを追加
$git commit -am 'ここにコメントを入れる'

#コミット完了
```

```
画像追加
imagesフォルダの中のファイルを表示させる
![title](images/sample.jpg)
```
![title](images/sample.jpg)