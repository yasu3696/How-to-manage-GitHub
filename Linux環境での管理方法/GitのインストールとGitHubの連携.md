# GitのインストールとGitHubの連携
<br>
<br>
<br>

 ## 1. Gitのインストール

| git --version |
|--|
| Gitがインストールされているか確認 |

### インストールさていなければ以下でインストール

 - レッドハット/CentOS:

| sudo yum install git |
|--|

 - Debian/Ubuntu系:
 
| sudo apt update |
|--|--|
| **sudo apt install git** |

<br>
-------------------
<br>

 ## 2.Gitの初期設定 
| git config --global user.name "あなたの名前" |
|--|
| **git config --global user.email "あなたのメールアドレス"** |
これでコミットに使われる名前とメールが設定されます。

<br>
---------------------------------
<br>

## 3. GitHubと連携（SSH鍵の設定）

 1. 鍵を生成：
 
| ssh-keygen -t ed25519 -C "あなたのメールアドレス" |
|--|
| （途中の質問はEnter連打でOK） |
 2. 公開鍵をコピー：
 
 
| cat ~/.ssh/id_ed25519.pub |
|--|--|
|  |
 3.  GitHubの[SSH設定ページ](https://github.com/settings/keys)にアクセスして、コピーした公開鍵を登録。
