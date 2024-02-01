# BackHacker

## ■サービス概要
BackHackerは、「自宅にいながらPC一台でバックパッカー」をコンセプトとした、バーチャル旅行好きのためのエンタメアプリです。  
地図を見ながら、世界中の国や都市を直感的に選んで、街並み動画で旅行気分を味わうことができます。
PC一台で、知らない土地に気軽にトリップしてみませんか？


## ■ このサービスへの思い・作りたい理由
私は暇さえあればGoogle Mapで「旅」をしています。
Google Mapを用いて、実際に行ってみたい場所のリサーチをすることもあれば、過去に訪れた場所を再訪し、旅を思い出して楽しんだりしています。
それ以外にも、知らない土地を無作為に訪問しては、観光名所やお店の情報を見て旅行気分を味わっています。
Google Mapで知らない土地を訪問したとき、実際の旅行に負けない高揚感を味わうことができます。

同様に、YouTubeで街歩き動画を見るのも好きです。
Google Mapと同じで、街並みや現地の雰囲気を知ることでワクワクするからです。
街歩き動画には、Google Mapの写真で現地を確認するよりもリアリティがあります。

もちろん実際に訪問できれば最高なのですが、時間や距離の制約から、なかなか訪問できない場所もあると思います。
そんな遠隔地の街並みや空気感を知る手段として、Google MapやYouTubeの街歩き動画は非常に有益です。

そのような中で、地図から気になった都市や街に訪問し、さらにその土地の動画が見られるアプリがあれば、
「地図から知らない土地に降り立つ高揚感」を得ることができ、また現地の街並みをよりリアルに知ることができて楽しそうだと思い、このアプリを制作することとしました。


## ■ ユーザー層について
- 地図を眺めるのが好きなユーザー
- Google Mapを利用して知らない土地のストリートビューを訪問したりするユーザー
- YouTubeで街歩きの動画を見て楽しんでいるユーザー
- 世界一周旅行に憧れがあるユーザー
- 海外に興味はあるが、実際に旅行するのはハードルが高いと感じているユーザー

## ■サービスの利用イメージ
### 利用方法
- 世界のどこかに訪問したいとき、ユーザーはトップページの地図からピンが打ってあるスポット(都市)を選択します。
- ピンをクリックすると国名、都市名、その都市のYouTube動画が埋め込みで表示されます。
- ユーザーは動画を見て楽しんだり、ピンされたスポットに対してコメントを残したり、コメント付きでXにシェアしたり、「訪問した(いいね)ボタン」を押すことができます。
- スポットは、世界の主要都市が登録されていますが、ユーザー自身で新規作成することができます。

- ユーザーは1日に何回でもスポットの動画を見ることができますが、「訪問した(いいね)ボタン」を押せる回数には限りがあります。
- 訪問した国の数によって、バックハッカーLv.が上がっていきます。
- 上位レベルのバックハッカーは特別な権利を得ることができます。
訪問した国はリストとして残り、すべての国を訪問すると「世界一周バックパッカー」のバッジが獲得できます。
それ以外にも、「アジア制覇」「ヨーロッパ制覇」など複数のバッジを用意します。

### 得られる価値・体験
このサービスを利用することで、知らない土地の雰囲気を詳細に知ることができ、ワクワクできます。
また旅行先として検討している国や都市の雰囲気を事前に把握することもできます。
単なる暇つぶしはもちろんですが、趣味としてGoogle Map旅行をする人やYouTubeの街歩き動画を見る人が
「コレクション」や「成果物」として目に見える形で訪問記録を残すことができます。
また友人にシェアしたり、訪問した国の数を自慢することも可能です。


## ■ ユーザーの獲得について
以下の方法でユーザー獲得を目指します
- Xでの宣伝、シェア活動
- Qiitaでの紹介記事投稿

## ■ サービスの差別化ポイント・推しポイント

- 世界中の都市の「歩いてみた」動画をまとめているWebサイトやアプリは存在していないと思われます。
- 差別化ポイント
  - 地図から各都市の動画を探せる点（国名、都市名でいちいち検索しなくてもよい)
  - ランキング形式でゲーム感覚で遊べる点

## ■ 機能候補

### MVPリリース時
- ユーザー登録機能
- ユーザー削除(退会)機能
- ログイン機能
- ログアウト機能
- Google Map表示機能
- スポット投稿機能(マップにピンを作成する)
- スポット削除機能
- スポット編集機能
- スポット一覧機能(地図上に表示)
- スポット一覧機能(国、地域別に一覧表示)
- コメント投稿機能
- コメント削除機能
- 訪問した(いいね)機能
- 訪問した(いいね)スポットの一覧機能
- ランキング機能
- 検索機能
- スポットを投稿する際、自動的に動画を取得する機能

### 本リリース時
- 通知機能
- 最新の「訪問した」をトップ画面に表示する機能
- オートコンプリート機能


## ■ 機能の実装方針予定
### 使用技術
バックエンド: Ruby 3.2.2 / Rails 7.1.3
- コード解析 / フォーマッター: Rubocop
- テストフレームワーク: RSpec
- データベース:　PostgreSQL
フロントエンド: Hotwire
- CSSフレームワーク: Tailwind CSS
- コード解析: ESLint
- フォーマッター: Prettier
インフラ: render
API: 
- Google Map API
  - 表示させた埋め込みマップ上をクリックして、スポット情報をピンとして投稿し、地図上に表示させる(大島てるのイメージ)
- YouTube Data API
  - スポットを登録時に、ピンした都市の動画をYouTubeから検索し、埋め込み表示させる

### 画面遷移図
[Figma](https://www.figma.com/file/ZUt2MHugqFmcQhiSp3hiJ1/BackHacker?type=design&node-id=0%3A1&mode=design&t=MUbmc5Gov3iGYJCF-1)
