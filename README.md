# CalculateWithoutWaste(2024/9/29)

https://eztas.github.io/CalculateWithoutWaste/

ゲームのポイントをできるだけ無駄なく使いきるための計算をするアプリ

# ver1 2024/09/29
入力機能、計算機能, 入力項目追加機能、計算結果表示機能の実装

# ver2 2024/11/24
固定消費ポイント計算の追加(必ずこのポイントをこの数だけ使いたい、というものに対応)

個々のインプットを削除できるボタンを実装

課題

固定消費したいもの可変消費でいいものをより分かりやすく分割。固定消費の入力枠を1つだけから複数対応にするのが課題

計算中などの、計算状態を可視化させたい

## 背景
自分が遊んでいるゲームにて、試合に勝つともらえるアイテム交換に利用できるポイントがある
個人的にポイントをできるだけ余すことなく使い切りたいが、アイテムの種類が約6種類あるため、その6元1次方程式を解くのが毎度大変だった
そこで、「所持しているポイント」、「各アイテムごとの消費ポイント」、「各アイテムの交換数の上限」を入力して、計算ボタンを押すだけで
この方程式を解くことができるアプリケーションを開発した
## 開発手法
perplexityにて実行したい内容を与えて作成
早く利用したかったので自分自身は開発に携わっていない
## 今後の展望
Reactを組み合わせてより使いやすいUIにしていきたい

## Git Commands

### 1. リモートリポジトリのクローン

まず、リモートリポジトリをローカルにクローンする。リポジトリのURLを使用して次のコマンドを実行する。

```
git clone git@github.com:~.git
```

### 2. 現在のリポジトリを確認
*のところが現在のブランチ

```
git branch
```

```
  demo
* develop
  main
```

### 3. 新しいブランチを切りだし

```
git checkout -b {your-feature-branch}
```

### 4. 変更をリモートに反映

```
git add .
git commit -m "メッセージを書いて下さい！"
git push
```

### 5. リモートのブランチの変更をローカルに反映

```
git fetch origin
git pull
```

### 6. リモートのブランチをローカルへ落とし込む(ローカルにbranch1がない)
```
git fetch origin
git checkout -b branch1 origin/branch1
```
### 7. リモートのブランチをローカルのブランチに反映(ローカルにbranch1がある)
```
git fetch origin
git checkout branch1
git merge origin/branch1
```
