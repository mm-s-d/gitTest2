# Gitコマンド学習メモ(初心者向け)

## Gtiコマンド

### 初期設定

- Gitの初期設定を確認  
  $ `git config --list`
- ユーザー名の登録  
  $ `git config --global user.name ...`
- メールアドレスの登録  
  $ `git config --global user.email ...`
- コミットコメント入力用エディタをvsCodeに指定  
  $ `git config --global core.editor "code --wait"`
- デフォルトブランチ名をmasterではなくmainに設定  
  $ `git config --global init.defaultBranch main`
- Git初期設定を削除する方法  
  $ `git config --global --unset ...`

### コミット操作

- ローカルリポジトリの初期化  
  $ `git init`

---

#### メモ

VSCodeでマークダウン表示をする場合、ctrl+shift+vでプレビュー表示可能。左右分割すると見やすい。

---

### 既存のGitローカルリポジトリを新規GitHubリモートリポジトリに登録

- GitHub に空の新規リポジトリを作成
- 既存のローカルリポジトリにGitHubの空のリモートリポジトリをエイリアス
  名「origin」として登録する。  
  $ `git remote add origin …`
- 登録したリモートリポジトリへ、ローカルリポジトリの内容を反映すると同時
  に、上流ブランチを設定する。  
  $ `git push -u origin main`
