# じぶんリリースノート

## master

## 0.35.9 (2020/9)

### Wandbox 関連

特になし

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- [三重野賢人](https://twitter.com/djann9071)
- Tommy6

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- [melpon/wandbox](https://github.com/melpon/wandbox)
  - Wandbox の Issue を閉じました
  - README.md を日本語にして FAQ を追加しました
  - 実行時に作成できるファイル数とファイルサイズに制限を入れました
  - 詳細は[こちら](https://github.com/melpon/wandbox/commits?author=melpon&since=2020-08-31&until=2020-09-30)
- [shiguredo/zakuro](https://github.com/shiguredo/zakuro)
  - 作りました
  - 詳細は[こちら](https://github.com/shiguredo/zakuro/commits?author=melpon&since=2020-08-31&until=2020-09-30)
- [shiguredo/momo](https://github.com/shiguredo/momo)
  - ROS ビルドを削除しました ([#173](https://github.com/shiguredo/momo/pull/173))
  - NVIDIA VIDEO CODEC SDK 10 に対応して、Linux で H264 が動作しない問題を修正しました ([#174](https://github.com/shiguredo/momo/pull/174))
  - Windows スクリーンキャプチャが動かなくなっていたのを修正しました
  - その他いくつかの変更や修正をしました
  - 詳細は[こちら](https://github.com/shiguredo/momo/commits?author=melpon&since=2020-08-31&until=2020-09-30)
- [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk)
  - M86 対応でコンパイルが通らなくなっていた部分を修正しました
  - 詳細は[こちら](https://github.com/shiguredo/sora-unity-sdk/commits?author=melpon&since=2020-08-31&until=2020-09-30)
- [shiguredo-webrtc-build/webrtc-build](https://github.com/shiguredo-webrtc-build/webrtc-build)
  - ubuntu-16.04_x86_64 と ubuntu-16.04_armv7 ビルドを削除しました
  - 詳細は[こちら](https://github.com/shiguredo-webrtc-build/webrtc-build/commits?author=melpon&since=2020-08-31&until=2020-09-30)

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています。
- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Load Testing Tool Zakuro](https://github.com/shiguredo/zakuro) を開発する仕事を請けています。
- [時雨堂](https://shiguredo.jp/) から gRPC C++ や gRPC Go を使った開発を請けていました（終了）。
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。
- とある会社から gRPC を使ったライブラリの開発を請けています。(詳細は非公開)

### ブログ

- [WebRTC Load Testing Tool Zakuro を作った話](https://dev.to/wandbox/webrtc-load-testing-tool-zakuro-p61)

### その他

- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を妻に作ってもらってます。
- 歯医者に行きました。

### 感想

- ９月は大体 Zakuro だった。
- Zakuro に [ちょっとしたゲーム](https://twitter.com/melponn/status/1309881464180232193) も追加できたので割と満足している。
- 来月は別件の gRPC の仕事を頑張ることになりそう。

## 0.35.8 (2020/8)

### Wandbox 関連

特になし

### Wandbox スポンサー関連

特になし

### OSS 関連

- [melpon/wandbox](https://github.com/melpon/wandbox)
  - Runtime Options が機能しなくなっていたのを修正しました ([#312](https://github.com/melpon/wandbox/issues/312))
  - 詳細は[こちら](https://github.com/melpon/wandbox/commits?author=melpon&since=2020-07-31&until=2020-08-31)
- [melpon/libxml](https://github.com/melpon/libxml)
  - [#5](https://github.com/melpon/libxml/pull/5), [#7](https://github.com/melpon/libxml/pull/7), [#9](https://github.com/melpon/libxml/pull/9) をマージして、依存ライブラリを更新して libxml-1.1.6 をリリースしました
  - 詳細は[こちら](https://github.com/melpon/libxml/commits?author=melpon&since=2020-07-31&until=2020-08-31)
- [shiguredo/momo](https://github.com/shiguredo/momo)
  - 設定は全部 ConnectionSettings に纏めて全体で利用していたけれども、モジュール性が悪いのでクラスごとに必要な最低限の設定に分けました ([#169](https://github.com/shiguredo/momo/pull/169))
  - `--multistream` と `--simulcast` に引数 true/false の指定を必要にしました
  - 詳細は[こちら](https://github.com/shiguredo/momo/commits?author=melpon&since=2020-07-31&until=2020-08-31)
- [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk)
  - Unity カメラのスクリーンキャプチャが動かいことがあった問題を、深度バッファを設定することで解消しました
  - Sora Unity SDK のダウンロードしたバイナリにライセンスファイルを含めました
  - iOS に対応しました ([#9](https://github.com/shiguredo/sora-unity-sdk/pull/9))
  - 詳細は[こちら](https://github.com/shiguredo/sora-unity-sdk/commits?author=melpon&since=2020-07-31&until=2020-08-31)
- [shiguredo/sora-unity-sdk-samples](https://github.com/shiguredo/sora-unity-sdk-samples)
  - サンプルが利用する Sora Unity SDK を 2020.8 にアップデートしました
  - 詳細は[こちら](https://github.com/shiguredo/sora-unity-sdk-samples/commits?author=melpon&since=2020-07-31&until=2020-08-31)
- [shiguredo-webrtc-build/webrtc-build](https://github.com/shiguredo-webrtc-build/webrtc-build)
  - iOS ビルドに対応しました ([#6](https://github.com/shiguredo-webrtc-build/webrtc-build/pull/6))
  - CentOS 8 ビルドに対応しました ([#8](https://github.com/shiguredo-webrtc-build/webrtc-build/pull/8))
  - デイリービルドのブランチを master から daily に変更して、今後は HEAD ビルドの修正をこのブランチで行うようにしました
  - HEAD ビルドが通らなくなっていたいくつかの問題を修正しました
  - その他いくつかのバグを修正しました
  - 詳細は[こちら](https://github.com/shiguredo-webrtc-build/webrtc-build/commits?author=melpon&since=2020-07-31&until=2020-08-31)

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています
- [時雨堂](https://shiguredo.jp/) から OSS で公開予定の [WebRTC Load Testing Tool Zakuro](https://medium.com/shiguredo/webrtc-load-testing-tool-zakuro-%E9%96%8B%E7%99%BA%E4%B8%AD-8d225a0654d) を開発する仕事を請けています
- [時雨堂](https://shiguredo.jp/) から gRPC C++ や gRPC Go を使った開発を請けています。(詳細は非公開)
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。

### ブログ

- [Sora Unity SDK を iOS 対応した話](https://dev.to/wandbox/sora-unity-sdk-ios-356m)

### その他

- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を妻に作ってもらってます。
- 歯医者にまた行き始めました。

### 感想

- ８月の前半は Sora Unity SDK の iOS 対応、後半は Zakuro に力を入れて頑張ってた。
- 種類は少ないけど、この２つをかなり頑張ってやってたと思うので今月は割と満足。
- 来月は Zakuro の公開に向けての対応と、あとは別件の仕事をちょっとするかも。

## 0.35.7 (2020/7)

### Wandbox 関連

特になし

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- むてら
- [@Linda_pp](https://twitter.com/Linda_pp)
- ガチKGB

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- [melpon/wandbox](https://github.com/melpon/wandbox)
  - IP 毎に送信できるソースコードのサイズを制限しました。
    - めちゃめちゃでかいコードを何度も送られてきて、実行ログが酷いことになってしまったので
  - /api/list.json の select スイッチに name が無かったのを修正
    - 内部の通信を gRPC に入れ替える前にはあった
  - 詳細は[こちら](https://github.com/melpon/wandbox/commits?author=melpon&since=2020-06-30&until=2020-07-31)
- [gumi/yacto](https://github.com/gumi/yacto)
  - `mix yacto.migrate` のリポジトリ一覧を `:ecto_repos` から取得する ([#21](https://github.com/gumi/yacto/issues/21))
  - 上記の対応を入れて [yacto-2.0.0-rc.1](https://hex.pm/packages/yacto/2.0.0-rc.1) をリリースしました
  - 詳細は[こちら](https://github.com/gumi/yacto/commits?author=melpon&since=2020-06-30&until=2020-07-31)
- [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk)
  - [GetStats を実装](https://github.com/shiguredo/sora-unity-sdk/pull/7) しました
  - 詳細は[こちら](https://github.com/shiguredo/sora-unity-sdk/commits?author=melpon&since=2020-06-30&until=2020-07-31)
- [shiguredo/sora-unity-sdk-samples](https://github.com/shiguredo/sora-unity-sdk-samples)
  - GetStats を利用する処理を追加
  - 詳細は[こちら](https://github.com/shiguredo/sora-unity-sdk-samples/commits?author=melpon&since=2020-06-30&until=2020-07-31)
- [shiguredo/momo](https://github.com/shiguredo/momo)
  - Jetson Xavier での VP9 のビットレートを調整しました
  - [VP8/H264 のサイマルキャストを実装](https://github.com/shiguredo/momo/pull/165) しました
  - [リファクタリング](https://github.com/shiguredo/momo/pull/166) しました
  - [SDL のビルド周りを修正](https://github.com/shiguredo/momo/pull/167) しました
  - 詳細は[こちら](https://github.com/shiguredo/momo/commits?author=melpon&since=2020-06-30&until=2020-07-31)

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています
- [時雨堂](https://shiguredo.jp/) から gRPC C++ や gRPC Go を使った開発を請けています。(詳細は非公開)
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。

### ブログ

なし

### その他

- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を妻に作ってもらってます。
- 歯医者に行ってたんだけど、一度予約すっぽかしてから再度予約するのは敷居が高くて治療が止まってる状態です。

### 感想

- 何もしてないのに７月が終わってたみたいな気分。
- VP9 の調査に半月ぐらい掛かってしまったとはいえ、それを考慮してもやってることが少なすぎなので反省したい。

## 0.35.6 (2020/6)

### Wandbox 関連

- [Wandbox に gcc-10.1.0を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-gcc-10-1-0%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-1cf8ca1ad4f5)
- [Wandbox に TypeScript 3.9.5 などを追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-typescript-3-9-5-%E3%81%AA%E3%81%A9%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-b561f0542636)
- [Wandbox に Lua 5.4.0 を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-lua-5-4-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-b99d95c84137)

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- [I (@wx257osn2)](https://twitter.com/wx257osn2)
- 安藤敏彦
- [長谷川一輝](https://twitter.com/_NANASI880)

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- [melpon/wandbox](https://github.com/melpon/wandbox)
  - Boost.SML と Boost.DI の URL が間違ってると[報告](https://github.com/melpon/wandbox/issues/308)を受けたので修正しました
  - ggrpc のバージョンを 0.4.0 に更新しました
  - ndjson の API が正しく動いてなかったのを修正しました
  - stdout と stderr が同時に閉じるとセグフォする問題を修正しました
  - 全体的に許容する nproc の数を増やしました
  - 詳細は[こちら](https://github.com/melpon/wandbox/commits?author=melpon&since=2020-05-31&until=2020-06-30)
- [melpon/ggrpc](https://github.com/melpon/ggrpc)
  - サーバストリーミングを実装しました
  - クライアントストリーミングを実装しました
  - 関数名を全体的に統一した名前に変更しました
  - ドキュメントを整理しました
  - 上記の変更を反映した ggrpc 0.4.0 をリリースしました
  - 詳細は[こちら](https://github.com/melpon/ggrpc/commits?author=melpon&since=2020-05-31&until=2020-06-30)
- [melpon/grpc-over-ayame](https://github.com/melpon/grpc-over-ayame)
  - 作りました。C++ 版の gRPC over WebRTC です
  - [Ayame](https://github.com/OpenAyame/ayame) でシグナリングしてます
- [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk)
  - [Androidに対応](https://github.com/shiguredo/sora-unity-sdk/pull/4) しました
  - GitHub Actions のキャッシュを cache@v2 にアップデート
- [shiguredo/sora-unity-sdk-samples](https://github.com/shiguredo/sora-unity-sdk-samples)
  - pub, sub, pubsub という名前を recvonly, sendonly, sendrecv に変更
  - Android対応に合わせてメタデータを変更
  - 詳細は[こちら](https://github.com/shiguredo/sora-unity-sdk-samples/commits?author=melpon&since=2020-05-31&until=2020-06-30)
- [shiguredo-webrtc-build/webrtc-build](https://github.com/shiguredo-webrtc-build/webrtc-build)
  - Windows 版のディレクトリ削除でエラーになっていたのを修正しました
  - `raspbian-buster` を `raspberry-pi-os` に変更しました
  - `raspberry-pi-os_armv8` を追加しました
  - macOS 版の .a 内のファイル名が15文字で切られていたのを修正しました
  - 詳細は[こちら](https://github.com/shiguredo-webrtc-build/webrtc-build/commits?author=melpon&since=2020-05-31&until=2020-06-30)
- [shiguredo/momo](https://github.com/shiguredo/momo)
  - [Windows / Linux の全画面スクリーンキャプチャを実装](https://github.com/shiguredo/momo/pull/155) しました
  - [利用できるエンコーダ/デコーダの一覧を表示する機能を実装](https://github.com/shiguredo/momo/pull/156) しました
  - [Boost のアーカイブをキャッシュ](https://github.com/shiguredo/momo/pull/159) しました
  - [ビデオコーデックのエンジン名を指定できる機能を実装](https://github.com/shiguredo/momo/pull/161) しました
  - `raspberry-pi-os_armv8` を追加しました
  - パッケージ名 `ubuntu-18.04_armv8_jetson_nano` を `ubuntu-18.04_armv8_jetson` に変更しました
  - パッケージ名 `raspbian-buster_armv6` と `raspbian-buster_armv7` を `raspberry-pi-os_armv6` と `raspberry-pi-os_armv7` に変更しました
  - 詳細は[こちら](https://github.com/shiguredo/momo/commits?author=melpon&since=2020-05-31&until=2020-06-30)
- [cpprefjp/crsearch](https://github.com/cpprefjp/crsearch)
  - [#41 add cpo category](https://github.com/cpprefjp/crsearch/pull/41) をマージ
  - deps更新
- [cpprefjp/kunai](https://github.com/cpprefjp/kunai)
  - deps更新
- [DreamExposure/DisCal-Discord-Bot](https://github.com/DreamExposure/DisCal-Discord-Bot)
  - 日本語化するのを[手伝いました](https://github.com/DreamExposure/DisCal-Discord-Bot/pull/32)。

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています
- [時雨堂](https://shiguredo.jp/) から gRPC C++ や gRPC Go を使った開発を請けています。(詳細は非公開)
- [時雨堂](https://shiguredo.jp/) から Sora Unity SDK の Android 対応を優先実装する仕事を請けています。
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。

### ブログ

- [Sora Unity SDK を Android 対応した話 - DEV Community 👩‍💻👨‍💻](https://dev.to/wandbox/sora-unity-sdk-android-1638)
- [Sora Unity SDK を NVDEC に対応した話 - DEV Community 👩‍💻👨‍💻](https://dev.to/wandbox/sora-unity-sdk-nvdec-2ieg)

### その他

- [std::めるぽんさんはTwitterを使っています 「C++ で gRPC over WebRTC できた！HTTP/2 の代わりに WebRTC DataChannel を使って gRPC をやり取りできるようになったぞ https://t.co/c87T0Hs6ZU」 / Twitter](https://twitter.com/melponn/status/1277183741010444288) が大量に Fav されてて謎だった。
  - 相当ニッチな内容だと思うんですけどこれ…。
- [std::めるぽんさんはTwitterを使っています 「Wandbox がちょこちょこ落ちる問題直ったかもしれない。しばらくこれで様子見かな」 / Twitter](https://twitter.com/melponn/status/1274517939291451393) で無事 Wandbox が落ちる問題が直ってたので安心しました。
  - 修正は[このコミット](https://github.com/melpon/wandbox/commit/ec5cf9211415838f31cba1eddcb05b39d06e42a9)です。何が間違ってたのか考えてみると面白いかも。
- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を作るのを継続してやっています。
  - もう最近は妻に作ってもらうのが殆どになりましたが
- 歯医者に通い始めました。
  - 今までの人生で歯医者にはほぼ無縁だったので、麻酔されたり親知らず抜かれたりゴリゴリされたりキュイーンされたり詰め物されたりでなかなかつらい…。
- 生活リズムは崩れ気味だった
  - けどなんかもう体調さえ崩れなければ別にいいんじゃないかってあまり気にしなくなってきた

### 感想

- メインの仕事が大分落ち着いてたので OSS 系に精を出してました。
  - 振り返るとかなりの量になってて面白い
- ブログ記事を２本も（？）書けた。
  - 自分のやったことを記事にするだけならそんなに大変でもないので、誰需要という感じでこの辺をちょこちょこ書いていきたいところ。
- 6月は一瞬で終わってしまった気がする。もうちょい人生を長く感じるようにしていきたいところ。

## 0.35.5 (2020/5)

### Wandbox 関連

- [Wandbox に Boost 1.73.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-boost-1-73-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-288e885700e2)

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- LouiS0616
- [@volanja](https://twitter.com/volanja)
- 大鎌広
- 他1名

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- [melpon/wandbox](https://github.com/melpon/wandbox)
  - 内部通信を gRPC 化した影響で、うまく動いてない部分がまだあったのでいろいろ直しました。
- [melpon/wandbox-builder](https://github.com/melpon/wandbox-builder)
  - Go が動いていなかったのを修正しました
- [melpon/ggrpc](https://github.com/melpon/ggrpc)
  - 実装をいい感じにして 0.1.0 リリースしました
  - そのままいろいろバグ修正や機能追加して 0.2.3 までバージョンアップしました
- [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk)
  - Sora.Role.Upstream, Sora.Role.Downstream を削除しました
  - 接続確立中に Sora.Dispose するとセグフォすることがあったのを修正しました
  - 接続が確立する前に ping を受け取ると通信が切断されてしまっていたのを修正しました
  - Windows 版の H.264 デコードでリサイズが発生した際にエラーになるのを修正しました
  - [Android 対応](https://github.com/shiguredo/sora-unity-sdk/tree/feature/android) を始めました
- [shiguredo/sora-unity-sdk-samples](https://github.com/shiguredo/sora-unity-sdk-samples)
  - Sora 切断時にトラックをクリアしてなかったのを修正しました
- [shiguredo-webrtc-build/webrtc-build](https://github.com/shiguredo-webrtc-build/webrtc-build)
  - [Android 用パッケージを追加](https://github.com/shiguredo-webrtc-build/webrtc-build/pull/1) しました
- [shiguredo/momo](https://github.com/shiguredo/momo)
  - EncodedImage::set_buffer() が消えてたので、毎フレーム EncodedImage を作り直すようにしました
  - Windows で音が鳴らなくなっていたので、Windows の ADM に専用の関数を使うようにしました
  - ビルド時に利用する Jetson Nano の L4T を 32.4.2 に更新しました

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています
- [時雨堂](https://shiguredo.jp/) から gRPC C++ や gRPC Go を使った開発を請けています。(詳細は非公開)
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。

### ブログ

なし

### その他

- Twitter にちょっとずつ復帰してきました。安心な発言しかしない人をリストに入れて（現在8人）、そこしか見ない運用してます。
- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を作るのを継続してやっています。
  - iPhone の Twitter クライアントを消しちゃったのでアップロードできてないですが。
- 5月の後半にまたギックリ腰をやってしまった。
  - そこまで酷くはないけど、1〜2日は立ち上がるだけで痛すぎて脂汗が出てた

### 感想

- 5月はメインの仕事が忙しいから OSS 活動はあまり進まなさそうって思ってたけど、振り返ると意外と結構やってたっぽい
  - メインの仕事のコードも、眺めるとかなりの量書いてて、一ヶ月って結構いろいろ出来るんだなって思った
- Wandbox がバグってて急いで修正したり、Sora Unity SDK がバグってて急いで修正したりで、バグは進捗を産むということが分かった

## 0.35.4 (2020/4)

（これからは月をパッチバージョンを一致させるようにした）

### Wandbox 関連

- Wandbox の内部通信を gRPC 化しました
  - PR はこれ: [kennel と cattleshed 間の通信を gRPC 化した](https://github.com/melpon/wandbox/pull/298)
- cattleshed のログにリモートアドレスとかの情報を追加しました
  - PR はこれ: [cattleshed のログにリモートアドレスとかの情報を追加した](https://github.com/melpon/wandbox/pull/302)
  - これで問題のあるコードを大量に投げてくる人を IP でブロックするみたいなのが出来るようになる
  - 早速 gRPC 化の恩恵が現れてる
    - 元のプロトコルだと、プロトコルを拡張してパーサを書き換えてってやらないといけなくて面倒だったのでやってなかった
- [@kikairoya](https://github.com/kikairoya) さんの PR [uidの分離を実装](https://github.com/melpon/wandbox/pull/304) をマージしました
  - おかげで酷いコードが投げられても他のユーザに影響することが少なくなりました。ありがとうございます。
- ちょっとだけ Issue の整理をしました
  - インストールができないみたいな Issue をどうしようかと思ってたんだけど、ある程度自分の中で方針が決まったので、[こういう](https://github.com/melpon/wandbox/issues/293) フォーマットも何も考えずペーストしただけの Issue は何も言わずクローズすることにした。再度同じようなの立てたらブロックする
  - どっかに方針書いておきたいところ
- [Wandbox に clang-10.0.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-clang-10-0-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-35cd9984e04c)
- [Wandbox に go-1.14.2 や go-1.13.10 などを追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-go-1-14-2-%E3%82%84-go-1-13-10-%E3%81%AA%E3%81%A9%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-92f166d2fea6)
- [Wandbox に nim-1.2.0 を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-nim-1-2-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-d3955f09ccdd)
- [Wandbox に nodejs-14.0.0 や nodejs-13.13.0 などを追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-nodejs-14-0-0-%E3%82%84-nodejs-13-13-0-%E3%81%AA%E3%81%A9%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-9993329389a2)

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- [@jj1bdx](https://twitter.com/jj1bdx)
- [TAKEI Yuya](https://github.com/takei-yuya)
- [nekketsuuu](https://twitter.com/nekketsuuu)
- [@cpp_maid_bot](https://twitter.com/cpp_maid_bot)
- [@ishidakei](https://twitter.com/ishidakei)
- [@hnokx](https://twitter.com/hnokx)

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- [gumi/yacto](https://github.com/gumi/yacto)
  - マイグレーションファイルをスキーマ毎に分けて生成するようにしました。
    PR はこれ: [マイグレーションファイルをスキーマ毎に分けるようにした](https://github.com/gumi/yacto/pull/20)
  - 上記の対応を入れて [yacto-2.0.0-rc.0](https://hex.pm/packages/yacto/2.0.0-rc.0) をリリースしました
- [shiguredo-webrtc-build/webrtc-build](https://github.com/shiguredo-webrtc-build/webrtc-build)
  - VERSIONS ファイルにはコミット情報だけじゃなくてリモートの URL も追加しました
    - WebRTC が参照しているリポジトリの URL が変わってしまうということが起きたため
  - ubuntu-16.04_armv7 ビルドから nolibcxx バージョンを削除しました
    - GCC が古くてビルドが通らなくなったので
- [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk)
  - Windows 版で NVIDIA VIDEO CODEC SDK が入っている場合に、ハードウェアデコードが出来るようにしました。
    - PR はこれ: [Windows の NvDec に対応](https://github.com/shiguredo/sora-unity-sdk/pull/3)
    - GitHub Actions には CUDA 環境が無いんだけど、その状態でビルドさせるのにすごく苦労した
- [shiguredo/momo](https://github.com/shiguredo/momo)
  - Jetson Nano では ALSA ではなく PulseAudio を利用する
    - [sora-laboでマルチストリームを実行中にjetsonでmomo配信を行うとmomoの映像がsora-laboに出ない](https://gist.github.com/torikizi/a9171ba1f6b9627a301c1e4100ea9349) の問題を解決するため
  - ubuntu-16.04_armv7_ros のビルドを削除
  - macOS で、バージョンが変わったら deps も自動的に取得し直すようにした
  - --version に WebRTC のバージョンや Environment の情報を出力する
- [shiguredo/sora-unity-sdk-samples](https://github.com/shiguredo/sora-unity-sdk-samples)
  - 利用する Sora Unity SDK のバージョンを 2020.2 にアップデートしました

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。

### ブログ

- [Wandbox の内部通信を gRPC 化した](https://medium.com/wandbox-org/wandbox-%E3%81%AE%E5%86%85%E9%83%A8%E9%80%9A%E4%BF%A1%E3%82%92-grpc-%E5%8C%96%E3%81%97%E3%81%9F-d0e8c8bf8717)

### その他

- コロナとか香川とかで Twitter 疲れを起こしたので、Twitter を見るのを一時的にやめてみました。会話はちょっとしたけど基本的に TL は見てない。
- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を作るのを継続してやっています。
- [リングフィットアドベンチャー](https://www.nintendo.co.jp/ring/) も継続してちょこちょこやってます。
  - 今月は大体音ゲーやってた。
  - でもこれ、上級と超上級に難易度の差がありすぎだし、曲ごとに同じような難易度ばっかりで飽きてくるし、レベルデザイン失敗してると思う
  - センサーみたいなアナログなのでやってるせいか、うまく動かしたつもりで失敗してるのはなかなかフラストレーションが溜まる
  - 音ゲー的な面白さもイマイチな感じ。腹筋のやつとか開発者ほんとに遊んだのかこれ
  - でも運動になるのでやる

### 感想

- 今月は仕事がほぼ無い状態だったのでいろいろできた。
  - 結構サボってる日もあるんだけど、一ヶ月あると意外と結構いろいろ進んで面白かった
- Twitter から離れた感想としては、割と平和で時間も無駄にせずに良かった気がする。
  - ただいくつかつぶやきたいことがある時に、それをつぶやくのも出来なくなってるのは微妙だった
  - あとランダムに良さげな情報を手に入れる手段が無くなってしまうので、自分に Twitter 疲れを起こさない人のリスト（プログラミング関係のことばっかりツイートしている人とか可愛い絵ばっかりリツイートしている人とか）みたいなの作って、頑張ってそこしか見ないみたいな運用でもいいと思うので、来月はそうしてみる
  - あと携帯からだと無限に時間を吸い取られるので、引き続き Twitter クライアントをアンインストールしたままにしておこうと思う

## 0.35.2 (2020/3)

### Wandbox 関連

- [Wandbox に Go 1.14.1 と Go 1.14 と Go 1.13.9 を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-go-1-14-1-%E3%81%A8-go-1-14-%E3%81%A8-go-1-13-9-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-f976a1ea8f4)
- [Wandbox に gcc-9.3.0を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-gcc-9-3-0%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-9a72f76b4375)
- [Wandbox に perl-5.30.1 を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-perl-5-30-1-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-e0ebedcea19c)

### Wandbox スポンサー関連

以下の法人スポンサーを追加/更新しました:

- [株式会社フィックスターズ](http://www.fixstars.com/)

以下の個人スポンサーを追加/更新しました:

- [@ignis_fatuus](https://twitter.com/ignis_fatuus)
- ブン
- [@tzik_tack](https://twitter.com/tzik_tack)
- [wraith13](https://twitter.com/wraith13)
- [@cpp_akira](https://twitter.com/cpp_akira)
- [@take_cheeze](https://github.com/take-cheeze)
- [@srz_zumix](https://twitter.com/srz_zumix)
- [@okdshin](https://twitter.com/okdshin)
- [@mumumu](https://twitter.com/mumumu)
- [@kariya_mitsuru](https://twitter.com/kariya_mitsuru)
- [@ciniml](https://twitter.com/ciniml)
- [@beam2d](https://twitter.com/beam2d)
- [@grafi_tt](https://twitter.com/grafi_tt)

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- cpprefjp / boostjp 関連
  - 久々に大掛かりなメンテナンスをしました。
  - cpprefjp/kunai, cpprefjp/crsearch の、メジャーバージョンアップを含む依存ライブラリの更新や deprecated なライブラリの切り替えを行い、3.0.3 をリリースしました。
  - cpprefjp/site_generator の [Python3 化の PR](https://github.com/cpprefjp/site_generator/pull/64) をマージして、cpprefjp/markdown_to_html も Python 3 に対応し、依存ライブラリを更新しました。
  - cpprefjp/site, boostjp/site のサイトへの反映を、今までは自分が借りているさくら VPS のサーバでやっていたのを、GitHub Actions で変換するようにしました。[cpprefjp/site への PR](https://github.com/cpprefjp/site/pull/739), [boostjp/site への PR](https://github.com/boostjp/site/pull/427)
  - [cpprefjp/kunai のコミット](https://github.com/cpprefjp/kunai/commits?author=melpon&since=2020-02-29&until=2020-03-31)
  - [cpprefjp/crsearch のコミット](https://github.com/cpprefjp/crsearch/commits?author=melpon&since=2020-02-29&until=2020-03-31)
  - [cpprefjp/site_generator のコミット](https://github.com/cpprefjp/site_generator/commits?author=melpon&since=2020-02-29&until=2020-03-31)
  - [cpprefjp/markdown_to_html のコミット](https://github.com/cpprefjp/markdown_to_html/commits?author=melpon&since=2020-02-29&until=2020-03-31)
  - [cpprefjp/site のコミット](https://github.com/cpprefjp/site/commits?author=melpon&since=2020-02-29&until=2020-03-31)
  - [boostjp/site のコミット](https://github.com/boostjp/site/commits?author=melpon&since=2020-02-29&until=2020-03-31)
- 時雨堂周辺の OSS 関連
  - [shiguredo/momo](https://github.com/shiguredo/momo)
    - WSS や TURN-TLS で接続する際にサーバの証明書をクライアント側で検証するようにしました。
    - 証明書を検証しないオプション `--insecure` を追加しました。
    - NvEnc に対応してない場合はビデオエンコーダを生成しないようにしました。
    - [Issue #138](https://github.com/shiguredo/momo/issues/138) Jetson Nano のデコーダの終了処理で Device or resource busy になってしまうことがあったのを修正しました。
    - 新しい MSVC だと JSON ライブラリの暗黙変換でエラーになっていたのを修正しました。
    - [Issue #143](https://github.com/shiguredo/momo/issues/143) Ubuntu 18.04 x86_64 の環境で libcuda.so/libnvcuvid.so がイントールされていないと起動できないのを修正しました。
    - [PR #147](https://github.com/shiguredo/momo/pull/147) ルートでの --port 引数を削除し、test と sora モードに --port を追加しました
    - `--daemon` 引数を削除しました
    - `--no-video` と `--no-audio` 引数を `--no-video-device` と `--no-audio-device` に変更しました
    - PCMU オーディオコーデックを削除しました
    - sora モードの引数に `--video`, `--audio` を追加しました
    - あと [Intel Media SDK](https://github.com/Intel-Media-SDK/MediaSDK) を使ったハードウェアエンコーダ/デコーダを試して、とりあえず Ubuntu で動きました。
    - [shiguredo/momo のコミット](https://github.com/shiguredo/momo/commits?author=melpon&since=2020-02-29&until=2020-03-31)
  - [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk)
    - CMakeLists.txt をモダンな書き方に修正しました
    - あと [Windows の NvDec 対応](https://github.com/shiguredo/sora-unity-sdk/tree/feature/nvdec) を始めました
    - [shiguredo/sora-unity-sdk のコミット](https://github.com/shiguredo/sora-unity-sdk/commits?author=melpon&since=2020-02-29&until=2020-03-31)
  - [shiguredo-webrtc-build/webrtc-build](https://github.com/shiguredo-webrtc-build/webrtc-build)
    - GitHub Actions 周りでエラーが起きてたのを修正しました
    - libaom 周りでエラーが起きるようになっていたのを修正しました
    - generate_licenses.py を使ってライセンスを生成するようにしました
    - あと [Android 対応](https://github.com/shiguredo-webrtc-build/webrtc-build/tree/feature/android) も始めてます。
    - [shiguredo-webrtc-build/webrtc-build のコミット](https://github.com/shiguredo-webrtc-build/webrtc-build/commits?author=melpon&since=2020-02-29&until=2020-03-31)
- その他 OSS 関連
  - melpon/memoize に[ドキュメント修正の PR](https://github.com/melpon/memoize/pull/9) が来ていたのでマージしました。
  - gumi/simple_schema に [`:meta` を許可する PR](https://github.com/gumi/simple_schema/pull/8) が来ていたのでマージしました。

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています
- [時雨堂](https://shiguredo.jp/) から gRPC C++ や gRPC Go を使った開発を請けています。(詳細は非公開)
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。

### ブログ

なし

### その他

- Qiita を退会しました。バックアップは [melpon/qiita](https://github.com/melpon/qiita) に置いてます。
- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を作るのを継続してやっています。
  - 作った料理は [Twitter に上げています](https://twitter.com/melponn/media)。
- [リングフィットアドベンチャー](https://www.nintendo.co.jp/ring/) も継続してちょこちょこやってます。

### 感想

- 前半は cpprefjp / boostjp 周りすごい頑張ってた
- 後半は Momo のハードウェアエンコーダ/デコーダ周りすごい頑張ってた
- 4月（0.35.3）は大きい仕事が無いので、いろいろ止まってたあれこれをやっていきたいところ

## 0.35.1 (2020/2)

### Wandbox 関連

- Wandbox の SSL 証明書を更新して[さくらの SSL から Let's Encrypt に乗り換えました](https://twitter.com/melponn/status/1233249685021679616)

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- わたやん
- [@KorekaraSEDB](https://twitter.com/KorekaraSEDB)

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- [shiguredo-webrtc-build/webrtc-build](https://github.com/shiguredo-webrtc-build/webrtc-build)
  - Windows で 4K パッチを適用するようにしました
  - WebRTC のバージョンを更新して何度かリリースしました（現時点で 81.4044.7.0 が最新）
- [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk)
  - Windows 版では H.264 エンコードに NVIDIA VIDEO CODEC SDK を使うようにしました
  - macOS 版では H.264 エンコード/デコードに VideoToolbox を使うようにしました
  - role の指定に sendonly, recvonly, sendrecv を使えるようにしました
  - pong 時に Sora に stats 情報を送るようにしました
  - 上記の変更を入れて 2020.1 をリリースしました
  - 詳細は [コミットログ](https://github.com/shiguredo/sora-unity-sdk/commits?author=melpon&since=2020-01-31&until=2020-02-29) を参照
- [shiguredo/sora-unity-sdk-samples](https://github.com/shiguredo/sora-unity-sdk-samples)
  - multi_pub のサンプルを追加しました
  - [Video Codecを選択可能にする](https://github.com/shiguredo/sora-unity-sdk-samples/pull/2) をマージしました
  - サンプルは Sora Unity SDK 2020.1 を使うようにしました
- [shiguredo/momo](https://github.com/shiguredo/momo)
  - ビルドを CMake 化して Windows 対応するのを [やりました](https://github.com/shiguredo/momo/pull/132)
  - デイリービルドの GitHub Actions を matrix を使って短くしました
  - macOS で --use-sdl オプションを利用すると落ちていたのを修正しました
  - WebRTC をカスタムしつつローカルに構築するためのドキュメントを追加
  - [Sora に stats の取得を実装](https://github.com/shiguredo/momo/pull/134) しました
  - 詳細は [コミットログ](https://github.com/shiguredo/momo/commits?author=melpon&since=2020-01-31&until=2020-02-29) を参照

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています
- [時雨堂](https://shiguredo.jp/) から Momo の Windows 対応、Momo と Sora Unity SDK の NVIDIA VIDEO CODEC SDK 対応などの仕事を請けています
  - [スロースネットワークス株式会社](http://www.sloth-networks.co.jp/) からの優先実装依頼です
- [時雨堂](https://shiguredo.jp/) から gRPC C++ や gRPC Go を使った開発を請けています。(詳細は非公開)
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。

### ブログ

なし

### その他

- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を作るのを継続してやっています。
  - 作った料理は [Twitter に上げています](https://twitter.com/melponn/media)。
- [リングフィットアドベンチャー](https://www.nintendo.co.jp/ring/) も継続してちょこちょこやってます。
- （1月のリリース忘れ）1月に [mini Regulus AR5](https://www.dospara.co.jp/5shopping/detail_prime.php?mc=8843&sn=0) を購入してました。
  - Ryzen5 3400G (3.7GHz-4.2GHz/4コア/8スレッド)、16GB メモリ、SSD 512GB+1TB
- [Dell XPS 15](https://www.dell.com/ja-jp/shop/%E3%83%87%E3%83%AB%E3%81%AE%E3%83%8E%E3%83%BC%E3%83%88%E3%83%91%E3%82%BD%E3%82%B3%E3%83%B3/xps-15-%E3%83%8E%E3%83%BC%E3%83%88%E3%83%91%E3%82%BD%E3%82%B3%E3%83%B3/spd/xps-15-7590-laptop) を購入しました。
  - Intel Core i7-9750H (最大4.5GHz/6コア/12スレッド)、16GB メモリ、SSD 1TB、NVIDIA GeForce GTX 1650
- SDL2 のビルド周りで [酷いバグ](https://twitter.com/melponn/status/1225083116559032320) に遭遇してました
- あまり書いてないけど、数日に１回ぐらいのペースで [Uber Eats](https://www.ubereats.com/ja-JP/) を利用してます

### 感想

- 完全に時雨堂中心の生活になってた
- Wandbox 周りもちょこちょこ弄ってたんだけど、外に出せるほどは進んでない
- 月の後半は割と遊んでる時間が多かった気がするので、もうちょいプログラム周りに割り当てたい
- 睡眠はまた夜型になってきた
  - 昼に連携取りながら進める仕事がほとんど無くなったので油断し始めた
- ヨシケイと Uber Eats で順調に引きこもりが加速してる

## 0.34.12 (2020/1)

### Wandbox 関連

- [Wandbox に Go 1.13.6 と Go 1.12.15 を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-go-1-13-6-%E3%81%A8-go-1-12-15-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-dfa3a19ea79b)
- [Wandbox に Nim 1.0.6 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-nim-1-0-6-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-351cf3173967)

### Wandbox スポンサー関連

以下の法人スポンサーを追加/更新しました:

- [株式会社ドットインストール](https://dotinstall.com/)

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- gRPC C++ でグレースフルシャットダウンが安全に出来るライブラリ [melpon/ggrpc](https://github.com/melpon/ggrpc) を作りました。
- [melpon/wandbox-builder](https://github.com/melpon/wandbox-builder) に GitHub Actions を導入して、HEAD ビルドの一部を行うようにしました。
  - これによって、週に１回になってた HEAD ビルドがデイリーでビルド出来るようになりました。
- [shiguredo/momo](https://github.com/shiguredo/momo)
  - ビルドを CMake 化して Windows 対応するのを [始めました](https://github.com/shiguredo/momo/tree/feature/cmake)。
  - タグを push したら GitHub Actions によるパッケージングとリリースが自動的に行われるようにしました。
  - --no-video で起動時に一瞬カメラデバイスを掴んでしまうのを修正しました。
  - jaist が落ちてる時のフォールバック先として tsukuba.wide を追加しました。
  - 詳細は [コミットログ](https://github.com/shiguredo/momo/commits?author=melpon&since=2019-12-31&until=2020-01-31) を参照。
- [shiguredo-webrtc-build/webrtc-build](https://github.com/shiguredo-webrtc-build/webrtc-build)
  - WebRTC のバージョンを上げて [m80.3987.2.1](https://github.com/shiguredo-webrtc-build/webrtc-build/releases/tag/m80.3987.2.1) をリリースしました
  - GitHub Actions を使って毎日 [HEAD ビルド](https://github.com/shiguredo-webrtc-build/webrtc-build/releases/tag/heads) を行うようにしました
- [shiguredo/sora-unity-sdk](https://github.com/shiguredo/sora-unity-sdk) の WebRTC と Boost のバージョンを上げて [v1.0.3](https://github.com/shiguredo/sora-unity-sdk/releases/tag/v1.0.3) をリリースしました。
- [shiguredo/sora-unity-sdk-samples](https://github.com/shiguredo/sora-unity-sdk-samples) を新しい Sora Unity SDK に追従しました。
- [gumi/connex](https://github.com/gumi/connex) と [gumi/simple_schema](https://github.com/gumi/simple_schema) の deps を更新して新しいバージョンをリリースしました。

### 仕事状況

- [時雨堂](https://shiguredo.jp/) から OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) やその周辺ライブラリのアップデートや機能追加する仕事を請けています
- [時雨堂](https://shiguredo.jp/) から gRPC C++ や gRPC Go を使った開発を請けています。1月(0.34.12) は WASM とブラウザ仕様を相手に戦ってました。(詳細は非公開)
- [株式会社アカツキ](https://aktsk.jp/) から Elixir 関連の OSS のメンテナンスや技術コンサルティングを行う仕事を請けています。

### ブログ

- [GitHub Actions でデイリービルドしてリリースする](https://medium.com/@melpon/github-actions-%E3%81%A7%E3%83%87%E3%82%A4%E3%83%AA%E3%83%BC%E3%83%93%E3%83%AB%E3%83%89%E3%81%97%E3%81%A6%E3%83%AA%E3%83%AA%E3%83%BC%E3%82%B9%E3%81%99%E3%82%8B-5211e7dc4b86)

### その他

- [ヨシケイ](http://yoshikei-dvlp.co.jp/) を利用してご飯を作るのを継続してやっています。
  - 作った料理は [Twitter に上げています](https://twitter.com/melponn/media)。
- [リングフィットアドベンチャー](https://www.nintendo.co.jp/ring/) も継続してちょこちょこやってます。
- [MSVC の謎の挙動](https://twitter.com/melponn/status/1222822322689597440) に苦しめられました（結局引数で # を渡すのは諦めた）。
- ちょっとだけ [WASM と戯れました](https://twitter.com/voluntas/status/1220184386655490048)
- [アジャイル開発で失敗した話が出ると「それはアジャイルじゃなかったね」って多方向から言われてアジャイルが問題ないことにされるの、無敵戦法すぎて面白い](https://twitter.com/melponn/status/1217631481528373248) という発言が結構 RT/Fav されました。
  - これに対して大量の [引用リプ](https://twitter.com/search?q=https%3A%2F%2Ftwitter.com%2Fmelponn%2Fstatus%2F1217631481528373248&src=typed_query&f=live) を貰いました。うんそうだね、アジャイルだね。

### 感想

- Wandbox の HEAD ビルドを少しだけ近代化できて良かった
- 睡眠は生活に慣れてちょっとマシになってきた気がする
  - けどやっぱり１日２回とか寝ることがあり、なかなか安定が難しい
- 時雨堂からまた新しい仕事を貰ったので、順調に時雨堂に囲い込まれてる
  - 囲い込まれるというか、むしろ囲いに自分から飛び込んでいく感じ。
  - コード書いてるだけでお金が貰えるし、やれることの範囲も徐々に広がってる感じがあるし、家に引きこもったままでいられるし、メリット多すぎて囲いの外に出たくない。
  - 囲い込みってこうやるんだなって勉強になる（使うことは無さそう）。

## ルール

["じぶんリリースノート" と称した月報を続けて3年が経った](https://blog.a-know.me/entry/2019/02/02/214612) のルールをそのまま利用する。

- 毎月月初に "新しい自分" がリリースされた、ということにして月報代わりに書いていく
- バージョン番号は `0.年齢.月齢` にする
- あの世へ行ったらメジャーバージョンを上げる
