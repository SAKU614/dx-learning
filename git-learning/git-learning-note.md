# Git / GitHub 学習ログ

## 学習日

2026年8月1日

---

# 1. Gitとは

## 概要

Gitは、ファイルの変更履歴を管理するためのツール。

例えばプログラムを修正した場合、

- いつ変更したか
- 何を変更したか
- 以前の状態へ戻せるか

を管理できる。

## イメージ
ファイル編集
↓
Gitが変更履歴を記録
↓
必要なら過去の状態へ戻せる

---

# 2. GitHubとは

## 概要

GitHubは、Gitで管理しているデータを保存・共有するクラウドサービス。

## GitとGitHubの違い

| 項目 | 役割 |
|---|---|
| Git | パソコン内で変更履歴を管理する |
| GitHub | Gitのデータをインターネット上で保存・共有する |

## 関係性
VS Code
↓
Git
↓
GitHub

---

# 3. GitHubアカウント作成

## 手順

1. GitHubへアクセス

https://github.com/

2. Sign upを選択

3. メールアドレス登録

4. パスワード設定

5. ユーザー名設定

6. メール認証

---

# 4. Gitの初期設定確認

## 確認コマンド

ターミナルで実行。

### ユーザー名確認

```
bash
git config --global user.name
```

### メールアドレス確認

```
bash
git config --global user.email
```

### メールアドレス確認結果例

```
user.name=sato-dx
user.email=xxxxx@gmail.com
```

---

# 5. VS CodeとGitHubを連携

## 確認手順：

1. VS Codeを起動
2. 左下のアカウントアイコンをクリック
3. GitHubへサインイン
4. ブラウザで

「Authorize Visual Studio Code」

を許可

5. VS Codeへ戻る

## 確認：

左下にGitHubユーザー名が表示されれば完了。


---


# ６. GitHubリポジトリ作成

リポジトリとは

プロジェクトを保存する場所。


## 例：

```
GitHub

dx-learning

```

## 作成手順：

1. GitHubへログイン
2. 「New repository」を選択
3. Repository nameを入力

例：
```
dx-learning
```
4. Descriptionを入力
例：
```
Learning repository for DX, Git, GitHub, kintone, Tableau, and JavaScript.
```
5. Publicを選択
6. README作成にチェック
7. Create repository

---

# 7. Clone（複製）

Cloneとは

GitHub上のリポジトリを自分のパソコンへコピーすること。

## 手順：

1. VS Codeを開く
2. Command Paletteを開く

```
⌘ + Shift + P
```

3. 以下を選択

```
Git: Clone
```
※日本語表示では「複製」

4. GitHubリポジトリを選択

```
dx-learning
```

5. 保存場所を指定
6. Open Repositoryを選択

---

# 8. Workspace Trust（制限モード解除）

制限モードとは

安全確認のためVS Codeが機能を制限している状態。

## 対応：

1. 上部の「制限モードになっています」をクリック
2. 「ワークスペースを信頼する」を選択

---

# 9. Commit（コミット）

Commitとは、変更履歴を保存する操作。

## 流れ：
ファイル編集

↓

Gitが変更を検知

↓

Commit

↓

変更履歴として保存


Commitメッセージ例

```
Add Git learning notes
```

---

# 10.Push（プッシュ）

Pushとは
Mac内のGitの変更履歴をGitHubへ送信する操作。

## 流れ：
Mac

Commit済み

↓

Push

↓

GitHubへ反映

Commitメッセージ例：
```
Add Git learning notes
```

---

# 11. Git学習ログの管理方法

## 推奨フォルダ構成：

```
dx-learning

├── git-learning
│   └── git-learning-note.md
│
├── kintone-learning
│   └── 学習記録
│
├── tableau-learning
│   └── 学習記録
│
└── ai-learning
    └── 学習記録

```

---

# 12.Gitを使った基本サイクル 

  今後の開発では以下を繰り返す。

  ① ファイル作成・編集

↓

② Gitで変更確認

git status

↓

③ Commit

変更履歴を保存

↓

④ Push

GitHubへ反映

---

# 13. 今回学んだGitコマンド

状態保存：現在の変更状態を確認します

```Bash
git status
```

Git設定確認：ユーザー情報を確認します

```
Bash
git config --global user.name
git config --global user.email
```

---

# 14. 今回の学習ポイント

* Gitは変更履歴管理ツール
* GitHubはGitデータの保存場所
* Repositoryはプロジェクト単位の保存場所
* CloneでGitHubからPCへコピーする
* Commitで変更履歴を保存する
* PushでGitHubへ反映する
* GitHubは将来のポートフォリオになる