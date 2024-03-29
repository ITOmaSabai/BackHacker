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
- 過去の旅行を思い出したり、誰かにシェアしたいユーザー

## ■サービスの利用イメージ
### 利用方法
- 世界のどこかに訪問したいとき、ユーザーはトップページの地図からピンが打ってあるスポット(都市)を選択します。
- ピンをクリックすると国名、都市名、その都市のYouTube動画が埋め込みで表示されます。
- ユーザーは動画を見て楽しんだり、ピンされたスポットに対してコメントを残したり、コメント付きでXにシェアしたり、いいねボタンを押すことができます。
- スポットは、ユーザー自身で新規作成することができます。スポットを作成する際には、スポット名やスポット周辺の街歩き動画のほか、コメントやタグをつけてスポットを紹介することができます。
- ユーザーは何箇所でもスポットの動画を見ることができますが、スポットを新規投稿できる回数には限りがあります。

### 得られる価値・体験
このサービスを利用することで、知らない土地の雰囲気を詳細に知ることができ、ワクワクできます。
また旅行先として検討している国や都市の雰囲気を事前に把握することもできます。
単なる暇つぶしはもちろんですが、個人の趣味としてGoogle Map旅行をする人やYouTubeの街歩き動画を見る人が、お気に入りのスポットをシェアして共感を集めたり、他のユーザーとのつながりを持つことができます。

## ■ ユーザーの獲得について
以下の方法でユーザー獲得を目指します
- Xでの宣伝、シェア活動
- Qiitaでの紹介記事投稿

## ■ サービスの差別化ポイント・推しポイント
- 世界中の都市の「歩いてみた」動画をまとめているWebサイトやアプリは極少数存在していますが、以下のポイントで差別化をしています。
  - 地図から各都市の動画を探せる点（国名、都市名でいちいち検索しなくてもよい)
  - ユーザーがスポットを新規投稿できる点

## ■ 機能候補

### MVPリリース時
- ユーザー登録機能
- ユーザー削除(退会)機能
- ユーザー情報機能
- ユーザーの投稿したスポット一覧機能
- ユーザーのいいねしたスポット一覧機能
- ログイン機能
- ログアウト機能
- Google Map APIを用いた機能
  - スポット新規投稿機能
  - スポット削除機能
  - スポット編集機能
  - スポット一覧機能(地図上に表示)
  - いいね機能
  - いいねしたスポットの一覧機能(地図上に表示)
- YouTube Data APIを用いた機能
  - スポットを投稿する際、自動的に動画を取得する機能

### 本リリース時
- コメント投稿機能
- コメント削除機能
- タグから検索機能
- 通知機能
- 最新の投稿をトップ画面に表示する機能
- 利用規約
- プライバシーポリシー

## ■ 機能の実装方針予定
### 使用技術
フロントエンド: React 18.2.0
- UIコンポーネント: MaterialUI
- コード解析: ESLint
- フォーマッター: Prettier
バックエンド: Ruby 3.2.2 / Rails 7.1.3
- コード解析 / フォーマッター: Rubocop
- テストフレームワーク: RSpec
- データベース:　PostgreSQL
インフラ: Vercel(フロントエンド) / Render(バックエンド)
API: 
- Google Map API
  - 表示させた埋め込みマップ上をクリックして、スポット情報をピンとして投稿し、地図上に表示させる
- YouTube Data API
  - スポットを登録時に、ピンした都市の動画をYouTubeから検索し、埋め込み表示させる