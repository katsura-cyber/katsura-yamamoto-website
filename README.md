# サイトの使い方・公開手順

## サイト構成(更新後)

- `index.html` … ホーム(彫刻作品の写真ギャラリー。以前あった文章は削除しました)
- `profile.html` … 略歴
- `blog.html` … ブログ一覧
- `blog/` フォルダの中の6ページ … ブログの各記事
  - `kibori.html`(木彫に挑戦)
  - `fuchineko.html`(ふちねこ の作り方)
  - `nendo.html`(粘土は手が荒れる？)
  - `dougu.html`(どんな道具で石を彫る？)
  - `takashimaya.html`(高島屋の展示)
  - `azarashi.html`(アザラシを設置しました)

## 1. 写真を差し替える

`images` フォルダの中に、まだ仮の画像(グレーの四角に文字が入ったもの)が入っています。
今のWordPressサイトの各記事から、対応する写真をダウンロードして、同じファイル名で置き換えてください。

**写真のダウンロード方法**: 各写真の上で右クリック →「名前を付けて画像を保存」

### ホーム(彫刻ギャラリー)・略歴の写真

- `images/profile.jpg` … 略歴ページの顔写真
- `images/work-01.jpg` 〜 `work-09.jpg` … ホームの彫刻ギャラリー(9枚)

### ブログ記事の写真(下の対応表の通りに保存してください)

**木彫に挑戦**
| 差し替えるファイル | 内容 |
|---|---|
| images/blog/kibori-01.jpg | 最初に彫ったネコ |
| images/blog/kibori-02.jpg | 写真の角度が難しい(2枚目のネコ) |
| images/blog/kibori-03.jpg | ふたつめのネコの彫りかけ |

**ふちねこ の作り方**
| ファイル | 内容 |
|---|---|
| fuchineko-01.jpg | 引き出しに入れてます(トップ画像) |
| fuchineko-02.jpg | 机に置くタイプのネコ |
| fuchineko-03.jpg | 茶トラ系ネコ |
| fuchineko-04.jpg | 黒系ネコ |
| fuchineko-05.jpg | 白系ネコ |
| fuchineko-06.jpg | 乾燥させたところ |
| fuchineko-07.jpg | 釉薬を掛けたところ |
| fuchineko-08.jpg | 焼き上がったところ |
| fuchineko-09.jpg | ネコと小さなアザラシ |

**粘土は手が荒れる？**
| ファイル | 内容 |
|---|---|
| nendo-01.jpg | 園芸用の土(トップ画像) |
| nendo-02.jpg | 陶芸の釉薬 |
| nendo-03.jpg | 石の粉まみれの様子 |

**どんな道具で石を彫る？**
| ファイル | 内容 |
|---|---|
| dougu-01.jpg | 石を手で彫る道具(トップ画像) |
| dougu-02.jpg | タンガロイが付いていないノミ |
| dougu-03.jpg | 小松石(ノミ跡) |
| dougu-04.jpg | 刃とんぼ・石頭 |
| dougu-05.jpg | 刃とんぼでノミ跡を細かくする様子 |
| dougu-06.jpg | 手磨き用の砥石 |
| dougu-07.jpg | 刃とんぼの跡と砥石の跡 |
| dougu-08.jpg | 表面の仕上がり |

**高島屋の展示**
| ファイル | 内容 |
|---|---|
| takashimaya-01.jpg | 展示会場(トップ画像) |
| takashimaya-02.jpg | 展示風景 |
| takashimaya-03.jpg | 白いアザラシ |
| takashimaya-04.jpg | 丸い小さいアザラシ |
| takashimaya-05.jpg | ペンギンの子供 |
| takashimaya-06.jpg | くり |
| takashimaya-07.jpg | ねむり猫 |
| takashimaya-08.jpg | 平たい小さいアザラシ |
| takashimaya-09.jpg | 古井さんとのコラボ展示 |
| takashimaya-10.jpg | カエル |

**アザラシを設置しました**
| ファイル | 内容 |
|---|---|
| azarashi-01.jpg | 設置したアザラシ(トップ画像) |
| azarashi-02.jpg | アザラシの様子 |
| azarashi-03.jpg | アザラシの様子 |
| azarashi-04.jpg | アザラシの様子(ポケストップ) |

## 2. 文章を直したい場合

各 `.html` ファイルをメモ帳などのテキストエディタで開くと、日本語の文章の部分だけをそのまま書き換えられます。
タグ(`<` `>` で囲まれた部分)は触らないようにしてください。

新しいブログ記事を追加したいときは、`blog` フォルダの中の似た記事のファイルをコピーして、タイトル・日付・本文・画像ファイル名を書き換え、`blog.html` の一覧にもリンクを追加してください。

## 3. GitHubに公開する(無料)

1. https://github.com で無料アカウントを作る
2. 右上の「+」→「New repository」をクリック
3. Repository name に `katsura-yamamoto-sculpture` など好きな名前を入力し、Public を選んで「Create repository」
4. できたページの「uploading an existing file」のリンクをクリック
5. このフォルダの中身(`index.html`, `profile.html`, `blog.html`, `style.css`, `images` フォルダ, `blog` フォルダ)をすべてドラッグ&ドロップ
6. 「Commit changes」をクリック

## 4. GitHub Pagesを有効にする

1. リポジトリの「Settings」タブを開く
2. 左メニューの「Pages」を選ぶ
3. 「Branch」を `main` に設定して「Save」
4. 数分後、`https://ユーザー名.github.io/リポジトリ名` でサイトが見られるようになります

## 5. 独自ドメイン(katsurayamamoto.com)をつなげる

1. 同じ「Settings → Pages」の画面で「Custom domain」に `katsurayamamoto.com` と入力して保存
2. ドメインを購入・管理しているサービス(お名前.comなど)の管理画面にログインし、DNS設定で以下を追加:
   - Aレコード(4つ、すべて追加):
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - もしくは CNAME で `ユーザー名.github.io` を指定(サブドメインの場合)
3. 反映まで数時間〜1日程度かかります

## 6. WordPressのサーバー(wing)を解約する

新しいサイトが正しく表示されることを確認できたら、wingの契約を解約して問題ありません。
**解約は、GitHub Pagesでサイトが正常に表示されることを確認してから**にしてください。
