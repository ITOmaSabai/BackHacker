
フロントエンドのリポジトリは[こちら](https://github.com/ITOmaSabai/BackHacker-frontend)です。  
バックエンドのリポジトリは[こちら](https://github.com/ITOmaSabai/BackHacker-backend)です。
# BackHacker. / バーチャル旅行体験アプリ
![サムネイル](assets/images/BackHacker_thumbnail.png)
[![React](https://img.shields.io/badge/React-v18.2.0-61DAFB?logo=React&logoColor=61DAFB)](https://react.dev/blog/2022/03/29/react-v18#whats-new-in-react-18)
[![Ruby](https://img.shields.io/badge/Ruby-v3.2.2-CC342D?logo=Ruby&logoColor=CC342D)](https://www.ruby-lang.org/ja/news/2023/03/30/ruby-3-2-2-released)
[![Rails](https://img.shields.io/badge/Rails-v7.1.3-CC0000?logo=Ruby-on-Rails&logoColor=CC0000)](https://rubyonrails.org/2024/2/21/Rails-Versions-6-1-7-7-7-0-8-1-and-7-1-3-2-have-been-released)
[![Firebase](https://img.shields.io/badge/Firebase-gray?logo=Firebase&logoColor=FFCA28)](https://firebase.google.com/)
[![Maps JavaScript API](https://img.shields.io/badge/Maps_JavaScript_API-gray?logo=googlemaps&logoColor=%234285F4&color=gray
)](https://developers.google.com/maps/documentation/javascript/overview)
[![YouTube Data API](https://img.shields.io/badge/YouTube_Data_API-gray?logo=youtube&logoColor=%23FF0000
)](https://developers.google.com/youtube/v3)
[![Thanks](https://img.shields.io/badge/Thank%20you-for%20visiting-00aab9)](https://backhacker-frontend.vercel.app/)



## サービス概要
BackHackerは、**「自宅にいながらPC一台でバックパッカー」** をコンセプトとした、バーチャル旅行好きのためのエンタメアプリです。
地図を見ながら、世界中の国や都市を直感的に選んで、街並み動画で旅行気分を味わうことができます。
PC一台で、知らない土地に気軽にトリップしてみませんか？


## サービス作成の背景
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

### ▼サービスURL
https://backhacker-frontend.vercel.app/  
レスポンシブ対応済みのため、スマートフォン環境からでもご利用いただけます。

### ▼開発者Xアカウント
https://x.com/Ito_GeekHatch  
お気づきの点がございましたら、こちらまでお気軽にご連絡ください。

## 使い方
- 地図上のピンをクリックすると、投稿したユーザー、タイトル、そのスポットに関連する街歩き動画が埋め込みで表示されます。
- ユーザーは動画を見て楽しんだり、ピンされたスポットに対してコメントを残したり、Xにシェアしたり、いいねボタンを押すことができます。
- スポットは、ユーザー自身で新規作成することができます。スポットに関連する動画は、住所情報を元にYouTubeから自動で取得されます (スポットの住所を元にYouTubeを検索しています)。
- ユーザープロフィールページでは、各ユーザーの投稿したスポットといいねしたスポットを一覧で確認できます。

![使い方](assets/gifs/how_to_use.gif)

### メイン機能の使い方
| スポットを見る | スポットを投稿する |
| :--- | :--- |
| ![スポットを見る](assets/gifs/view_spots.gif) | ![スポットを投稿する](assets/gifs/post_spots.gif) |
| 地図上のピンをクリックします。モーダルが動画を見る場合は、開いたモーダルの動画サムネイルをクリックします。 | 地図上をクリック後、スポットを投稿ボタンを押下します。次に、スポット名と説明（任意）を入力してから投稿するボタンを押下します。 |

| いいねする | コメントする |
| :--- | :--- |
| ![いいねする](assets/gifs/likes.gif) | ![コメントする](assets/gifs/comments.gif) |
| スポット詳細画面のハートのボタンを押下します。いいねを解除するには、もう一度押下します。 | スポット詳細画面の吹き出しボタンを押下するとモーダルが開きます。コメントを入力後、投稿ボタンを押下します。コメントを削除するには、コメントの横のゴミ箱アイコンを押下します。 |


## 機能
- ユーザー登録機能
- ユーザー削除(退会)機能
- ユーザー情報機能
- ユーザーの投稿したスポット一覧機能
- ユーザーのいいねしたスポット一覧機能
- ログイン機能
- ログアウト機能
- スポット新規投稿機能
- スポット削除機能
- スポット編集機能
- スポット一覧機能(地図上に表示)
- いいね機能
- いいねしたスポットの一覧機能(地図上に表示)
- コメント投稿機能
- コメント削除機能


## 使用技術
| カテゴリ | 技術 |
| :---| :--- |
| フロントエンド | React 18.2.0 |
| UIコンポーネント | MaterialUI |
| コード解析 | ESLint |
| バックエンド | Ruby 3.2.2 / Rails 7.1.3 |
| データベース | PostgreSQL |
| 認証 | Firebase Authentication |
| インフラ | Vercel(フロントエンド) / Render(バックエンド) |
| API | Maps JavaScript API(Google Map) / YouTube Data API |

## 技術選定の理由
### フロントエンド: React
Reactを使ったアプリの開発経験はほとんどありませんでしたが、以下の2つの理由からReactを採用しました。

1. JavaScriptで描画するGoogle Mapの制御を容易にするため
2. 充実したUIライブラリを活用し、リッチなUIを構築してユーザー体験を向上させるため

ReactのフレームワークであるNext.jsの導入は、キャッチアップコストと得られるメリットを検討した結果、導入を見送りました。

### バックエンド: Ruby on Rails
フロントエンドのキャッチアップに時間を要すると判断したため、最速でバックエンドを構築したいと考え、学習経験のあったRuby on Railsを選定しました。

### 環境構築: ローカル
Dockerの使用も検討しましたが、最短時間で環境構築をし、フロントエンドの構築に時間を割きたかったため、ローカルでの環境構築を選択しました。

### 認証: Firebase Authentication
以下2点の理由から、Firebase Authenticationを使ったGoogleログインを選定しました。
1. 機密情報の漏洩を避けるため
2. ログインにおけるユーザーの工数を削減するため

1については、ユーザーのメールアドレスやパスワードなどの機密情報を、自分のデータベースに保存せず外部サービスに保存することで、情報漏洩のリスクを低下させる狙いです。

2については、Googleアカウントにログイン状態であればパスワードを入力する必要がなく、ユーザーの工数を削減できると考えました。普及率の高いGoogleアカウントであれば、ユーザーがログイン状態である可能性が高いと考えました。

### インフラ: Vercel / Render
以下の2点の理由から、VercelとRenderを選択しました。
1. ドキュメントが豊富に存在していて、設定が容易である点(フロントエンドの構築に時間を割くために、環境構築の時間を最小にしたかった)
2. 基本利用が無料である点(個人開発アプリを長く維持するためには、運用コストは最小限に抑える必要があると判断したため)

## 工夫した点
▼画面の全面に地図を表示することで、アプリへの没入感を演出しました。
| PC画面 |
| :--- |
| ![PC画面](assets/images/map_laptop_view.png) |

| スマートフォン画面 |
| :--- |
| ![スマートフォン画面](assets/images/map_smartphone_view.png) |


▼新規投稿完了後には次のアクションを促すモーダルを表示するなど、ユーザーの行動を先読みして誘導することで、ユーザーが次のアクションに迷わないようにしました。
| 新規投稿完了後のモーダル |
| :--- |
| ![スポットを投稿する](assets/gifs/post_spots.gif) |


▼ユーザーがアプリを操作する際ストレスを感じないように、利用者の多いアプリのボタン配置を参考に、UIを構築しました。

## 今後の展望
以下の機能を追加していきたいと考えています。
- 通知機能
- 最新の投稿をトップ画面に表示する機能

また、現状は自動で取得される動画の精度 (スポットとの関連度)が若干低いため、関連性の高い動画を取得できるように改善していきたいと思います。
