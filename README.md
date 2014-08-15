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
```
#現在どこのbranchにいるのか確認する
$git branch

#その後masterブランチに移動する
$git checkout master

#移動できない場合　コミットしてない場合が多い

#移動できているか確認する
$git branch


```