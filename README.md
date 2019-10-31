# じぶんリリースノート

## 0.34.9

### Wandbox 関連

- [Wandbox に CPython 3.8.0 他と PyPy 7.2.0–3 他を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-cpython-3-8-0-%E4%BB%96%E3%81%A8-pypy-7-2-0-3-%E4%BB%96%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-826bd973aba0)
- [Wandbox に Ruby 2.8.0-preview1 他と mruby 2.0.1 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-ruby-2-8-0-preview1-%E4%BB%96%E3%81%A8-mruby-2-0-1-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-a8de991e5d99)

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- [@tyottyoworks](https://twitter.com/tyottyoworks)
- [まろ](https://twitter.com/_marony)

Wandbox はスポンサーになってくれた皆のおかげで動いてるのでとても感謝しています。

### OSS 関連

- [Yacto](https://github.com/gumi/yacto) を大改修して、いくつか破壊的変更を入れつつ 2.0.0-pre.15 をリリースしました。
- WebRTC SFU Sora の Unity プラグインである [Sora Unity SDK](https://github.com/shiguredo/sora-unity-sdk) の実装をしました。
  - [Sora Unity SDK サンプル集](https://github.com/shiguredo/sora-unity-sdk-samples) も実装しました。
- Sora Unity SDK を作る過程で [Windows 向け WebRTC ライブラリ用ビルドツール](https://github.com/shiguredo/shiguredo-webrtc-windows) の整備を行いました。

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています（11月末で契約終了）
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- OSS である [Sora Unity SDK](https://github.com/shiguredo/sora-unity-sdk) を開発したりメンテナンスする仕事をやっています
- gRPC C++ や gRPC Go を使った開発をやっています(詳細は非公開)

### ブログ

書いてない

### その他

- Sora Unity SDK を使ってマルチストリームする動画を頑張って作った: https://twitter.com/melponn/status/1185869961811513346
- Wandbox の実行環境が HDD フルになってたので、何とか対応した

### 感想

- 10月は忙しいので外に見える成果はあまり無さそうだと思ってたけど、Sora Unity SDK を OSS で開発する仕事を時雨堂から貰えたので結構成果が出た
- Yacto の改修も割と頑張ってた
- 11月も10月と同じような感じになる予定

## 0.34.8

### Wata 関連

特に無し

### Wandbox 関連

- autoconf から CMake でのビルドに切り替えました: https://github.com/melpon/wandbox/pull/282
- [Wandbox に Go 1.13 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-go-1-13-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-a030c702d756)
- [Wandbox に Boost 1.71.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-boost-1-71-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-13fed38c0149)
- [Wandbox の PHP に mbstring 対応を入れました](https://medium.com/wandbox-org/wandbox-%E3%81%AE-php-%E3%81%AB-mbstring-%E5%AF%BE%E5%BF%9C%E3%82%92%E5%85%A5%E3%82%8C%E3%81%BE%E3%81%97%E3%81%9F-8c0f1722939a)
- [Wandbox に clang-9.0.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-clang-9-0-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-7f7f05dbf1df)
- [Wandbox に Nim 1.0.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-nim-1-0-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-5d0f58d21e7e)
- [Wandbox に Go 1.13.1 と Go 1.12.10 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-go-1-13-1-%E3%81%A8-go-1-12-10-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-80db2714d806)

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- [イズカワタカノブ](https://twitter.com/soundkitchen)

### momo 関連

- Jetson Nano 用のクロスビルドに対応しました: https://github.com/shiguredo/momo/pull/99
- オーディオフラグの無効化オプションを追加しました: https://github.com/shiguredo/momo/pull/97

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています（11月末で契約終了）
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- gRPC C++ を使って開発した仕事のメンテナンスをしています(詳細は非公開)

### ブログ

以下の記事を書きました。

- [gRPC C++ の環境を構築する](https://medium.com/@melpon/grpc-c-%E3%81%AE%E7%92%B0%E5%A2%83%E3%82%92%E6%A7%8B%E7%AF%89%E3%81%99%E3%82%8B-4f5f40fb10ec)
- [React Hooks でいい感じに fetch する](https://medium.com/@melpon/react-hooks-%E3%81%A7%E3%81%84%E3%81%84%E6%84%9F%E3%81%98%E3%81%AB-fetch-%E3%81%99%E3%82%8B-8a1101c776de)
- [Wandbox のビルドを CMake に移行した話](https://medium.com/wandbox-org/wandbox-%E3%81%AE%E3%83%93%E3%83%AB%E3%83%89%E3%82%92-cmake-%E3%81%AB%E7%A7%BB%E8%A1%8C%E3%81%97%E3%81%9F%E8%A9%B1-693956073d45)

### その他

- WebRTC のシグナリングサーバである [Ayame](https://github.com/OpenAyame/ayame) を C++ で再実装してみました: https://github.com/melpon/ayame_cpp
  - まだとりあえず動く程度しか実装してない
- 自分用のテンプレート置き場用のリポジトリ [mytemplates](https://github.com/melpon/mytemplates) を作りました
  - mytemplates に C++ + WebSocket のサーバを扱う場合のテンプレートを追加しました
  - mytemplates に TypeScript + React Hooks + Material UI を使う場合のテンプレートを追加しました
- gRPC の実験をいろいろやるリポジトリ [grpc_sandbox](https://github.com/melpon/grpc_sandbox) を作りました
- FLAC 1.3.3 が CMake 対応したと書いていたのに、パッケージに CMakeLists.txt が無かった問題を報告しました: https://github.com/xiph/flac/issues/140
- Boost.System が 1.69.0 からヘッダーオンリーになってるので、boostjp の [ヘッダオンリー or ビルドが必要なライブラリ](https://boostjp.github.io/tips/build_link.html) を修正しました: https://github.com/boostjp/site/commit/c0ea2bd7b86172847b510245f807729f0cf2a8cd

### 感想

- 今回はすごくいろいろやったので大変良かった
- けど相変わらず Wandbox の UI はリプレースできなかったので反省する
- しかし今月からは仕事が忙しくなる予定なので、外に見える進捗はあまり出なさそう
- 少なくとも Wata は gumi の契約終了までは諦めて、そっから考える

## 0.34.7

### Wata 関連

- ネイティブプラグインとのやり取りに、以前は組み込み型や配列ぐらいしか渡せなかったのを、C# 用の proto ファイルから生成したメッセージを使うようにして汎用的にしました。
- ネイティブプラグインのログを Unity 側で扱えるようにしました。

### Wandbox 関連

- Wandbox の新しい UI をプレビューで公開しました → https://canine.wandbox.org/
- Wandbox の UI を TypeScript+React+Hooks+MaterialUI で[作り直しています](https://github.com/melpon/wandbox/tree/canine/canine)。
- gcc-9.2.0 を [追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-gcc-9-2-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-8ccb795b16d0)
- Go 1.12.8 と 1.11.13 を [追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-go-1-12-8-%E3%81%A8-1-11-13-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-d2983e877f56)
- Go 1.12.9 を [追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-go-1-12-9-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-bfbd0e90dbb1)

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました:

- [@gnaggnoyil](https://twitter.com/gnaggnoyil)
- [@mandel59](https://twitter.com/mandel59)
- Tommy6

### momo 関連

- 細かいところを [いろいろ](https://github.com/shiguredo/momo/commits?author=melpon&since=2019-07-31&until=2019-08-31) やりました
  - `--video-device` オプションの追加
  - `./momo p2p` を `./momo test` に
  - nlohmann/json のバージョン更新
  - `--metadata` オプションの公開（以前は隠しオプションだった）

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- gRPC C++ を使って開発した仕事のメンテナンスをしています(詳細は非公開)

### その他

- Wandbox がディスクフルで止まっていたので直しました。
  - 実行ログが大分多かったので S3 にアップロードして削除しました。
- そのついでに実行ログから１日に何回 Wandbox が実行されてるかを [確認しました](https://twitter.com/melponn/status/1165162847975854080)
- [Kubernetes完全ガイド impress top gearシリーズ](https://www.amazon.co.jp/dp/B07HFS7TDT/) を読みました。

### 感想

- Wata と Wandbox の UI、どちらもそこそこ進められたので良かった。
- Wandbox の UI はリプレースまで行かなかったので反省する。
- これ書いてて気が付いたけど Boost 1.71.0 をビルドしたまま放置してたのでちゃんと追加する。
- ブログ書いてなさ過ぎなので反省する。

## 0.34.6

### Wata 関連

- Wata の公式 Web サイトを[株式会社Xemono](https://xemono.life/)に作ってもらいました。公開は実装が完了してからになります。

### Wandbox 関連

- [Wandbox に Go 1.12.7 と 1.11.12 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-go-1-12-7-%E3%81%A8-1-11-12-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-c4bc50801e9e)
- [Wandbox に Nim 0.20.2 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-nim-0-20-2-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-20f60aa62b0c)
- Wandbox の UI を TypeScript+React+Hooks+MaterialUI で[作り直しています](https://github.com/melpon/wandbox/tree/canine/canine)。

### Wandbox スポンサー関連

- 無し

### momo 関連

- Momo の [Windows 版](https://gist.github.com/voluntas/7af1596557121796123ac7dee9e3f5a4) のビルド周りを改善した

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- gRPC C++ を使って開発した仕事のメンテナンスをしています(詳細は非公開)
- Opus を扱う Unity プラグインを実装する仕事が完了しました（詳細は非公開）

### その他

- Yacto ライブラリの [TODO](https://github.com/gumi/yacto/issues/15) を書きました
- Yacto ライブラリを [MyXQL アダプターに対応](https://github.com/gumi/yacto/commit/88f4d8debdef21587600dcb0f3fbab05e778ad14) して [2.0.0-pre.13](https://github.com/gumi/yacto/releases/tag/2.0.0-pre.13) をリリースしました。
- [ecto_sql](https://github.com/elixir-ecto/ecto_sql/issues/129) の MyXQL アダプターが MySQL 5.6 で `:map` 型が使えないことを報告しました（仕様とのこと）。
- Credo ライブラリの実行で警告が出ていたので [修正PR](https://github.com/rrrene/credo/pull/677) を投げ、無事マージされました。
- simple_schema ライブラリの [1.1.9](https://github.com/gumi/simple_schema/releases/tag/1.1.9) をリリースしました。

### 感想

- Wata 関連の実装があまり進んでないのは反省したい。今月は何か進捗出したいところ。
- 仕事の関係もあって Elixir 周りで調べたり PR してることが多かったなーという感じ。
- Wandbox の UI は先月中には作っておきたかったけど、思ったより大変だったのでまだ完了してない。今月にはリプレースさせたい。

## 0.34.5

### Wata 関連

- C# 側とのインターフェース部分を書き換え
- バグ修正

### Wandbox 関連

- [Wandbox に Node.js 10.16.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-node-js-10-16-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%9F-76f571377453)
- [Wandbox に新しく TypeScript を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB%E6%96%B0%E3%81%97%E3%81%84%E8%A8%80%E8%AA%9E-typescript-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-3c24fd7fec5a)
- [Wandbox に Swift 5.0.1 を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-swift-5-0-1-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-f5b4fe17e2d0)
- [Wandbox に Nim 0.20.0 を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-nim-0-20-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-5395b23866cc)
- [Wandbox に Go 1.12.6 と 1.11.11 を追加しました](https://medium.com/@melpon/wandbox-%E3%81%AB-go-1-12-6-%E3%81%A8-1-11-11-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-e12885bf2a1)

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました。

- [黒澤　亮二](https://twitter.com/rjkuro)
- [@fukasawah](https://twitter.com/fukasawah)
- [暢気](https://twitter.com/f_akinobu)

### momo 関連

- Windows の Docker で momo.exe をビルドする機能を[実装しました](https://twitter.com/voluntas/status/1144944949445550081)
- [ubuntu-18.04_x86_64 のベースが Ubuntu 16.04 になってたのを修正](https://github.com/shiguredo/momo/commit/9570fe9d0a16ed10e899a167eb68ee6653fefa0f)
- [--video-codec や --audio-codec などを sora 専用オプションに移動](https://github.com/shiguredo/momo/commit/92d7f07215b277b02e3038fd7e273bcb1df8593a)
- [CLI 1.8.0 にバージョンを上げた](https://github.com/shiguredo/momo/commit/cc33d7b262cfbf69db9e4da7fb599c0f48cbe0f3)
- [NOTTY オプションを追加](https://github.com/shiguredo/momo/commit/08f15330010b78d43e6ef1f2cbf41c65a92b36d1)
- [ubuntu-16.04_armv8 のビルドを削除](https://github.com/shiguredo/momo/commit/93095c4ab2ca4530fbd9d8fe74e9d586f3993c58)

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- gRPC C++ を使って開発した仕事のメンテナンスをしています(詳細は非公開)
- Opus を扱う Unity プラグインを実装する仕事をしています(詳細は非公開)

### その他

## 0.34.4

### Wata 関連

- RTMP to ブラウザーを実装して[記事にしました](https://medium.com/wandbox-org/wata-%E3%82%92%E3%83%AA%E3%82%A2%E3%83%AB%E3%82%BF%E3%82%A4%E3%83%A0%E6%98%A0%E5%83%8F%E9%85%8D%E4%BF%A1%E3%81%AB%E5%AF%BE%E5%BF%9C%E3%81%97%E3%81%9F-569300f47b8e)

### Wandbox 関連

- [gcc-9.1.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-gcc-9-1-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%9F-aea46f4cba01)
- [perl-5.28.2 と perl-5.30.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-perl-5-28-2-%E3%81%A8-5-30-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-50064e87a87a)

### Wandbox スポンサー関連

以下の企業スポンサーを追加/更新しました。

- [セオライド・テクノロジー㈱](http://theolizer.com/)
- [株式会社gumi](https://gu3.co.jp/)
- [BASSDRUM株式会社](https://bassdrum.org/)

以下の個人スポンサーを追加/更新しました。

- [I (@wx257osn2)](https://twitter.com/wx257osn2)
- [@jj1bdx](https://twitter.com/jj1bdx)
- [@yuushimizup](https://twitter.com/yuushimizup)
- 安藤敏彦

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- あるプログラミング教育系のサイトで C と C++ を扱うということで、そのコンサルティングをやっています
- gRPC C++ を使って開発する仕事をやっています(詳細は非公開)

## 0.34.3

### Wata 関連

- Windows で動きました → [Wata をWindows対応しました](https://medium.com/wandbox-org/wata-%E3%82%92windows%E5%AF%BE%E5%BF%9C%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-59a0259f436f)
- gRPC 1.20.0 にアップデートしました
- Wata をバーチャルライバー特化型の配信とするように方針を決めました
- Wata で RTMP をブラウザに配信して表示するのを実装しました → https://twitter.com/melponn/status/1123135647840067584

### Wandbox 関連

- [boost-1.70.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-boost-1-70-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%9F-94f99ca4a6e1)
- Wandbox で日本語で書いた文字列が permlink 経由で表示した時に文字化けしていたバグを修正しました。

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました。

- [Freezer](https://mastodon.social/@Freezer)
- [mtera](https://twitter.com/tonakou)
- [@m_akihiro](https://twitter.com/m_akihiro)
- 松崎啓治

### momo 関連

- Boost 1.70 へのアップデートをしました
- ubuntu-18.04_armv8 のビルドを追加しました

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- あるプログラミング教育系のサイトで C と C++ を扱うということで、そのコンサルティングをやっています
- gRPC C++ を使って開発する仕事をやっています(詳細は非公開)

### その他

- [FLAC の仕様](https://xiph.org/flac/format.html#format_overview) を読んで、FLAC が任意の位置（バイト単位）から再生しても正しくデコードできるようになっていることを知りました
- 借りてた自作キーボードにゲームを入れて遊んでました → [自作キーボードにゲームを作って入れた話](https://medium.com/@melpon/%E8%87%AA%E4%BD%9C%E3%82%AD%E3%83%BC%E3%83%9C%E3%83%BC%E3%83%89%E3%81%AB%E3%82%B2%E3%83%BC%E3%83%A0%E3%82%92%E4%BD%9C%E3%81%A3%E3%81%A6%E5%85%A5%E3%82%8C%E3%81%9F%E8%A9%B1-a4840a83518e)
- [動画を送ろう!!RTMP](https://www.kumaryu.net/books/douga-rtmp.html) を読んで RTMP を一から作ったので、RTMP にとても詳しくなりました
- [Coinhive事件裁判費用の寄付のお願い](https://www.hacker.or.jp/coinhive_innocent/) に合同会社 Wandbox として 5 万円寄付しました

## 0.34.2

### Wata 関連

- １万接続で試験して動作しました → [Wataが1万接続で動いた – wandbox.org – Medium](https://medium.com/wandbox-org/wata%E3%81%8C1%E4%B8%87%E6%8E%A5%E7%B6%9A%E3%81%A7%E5%8B%95%E3%81%84%E3%81%9F-7d9eab20a144)
- Wata プロジェクトの紹介ページを用意しました → [Wata プロジェクト](https://gist.github.com/melpon/8ba5197d71ece3b034abfcd0f7cb10db)
- １万接続で大変だったのをまとめました → [gRPC を使って1万接続を達成するまでの話 – wandbox.org – Medium](https://medium.com/wandbox-org/grpc-%E3%82%92%E4%BD%BF%E3%81%A3%E3%81%A61%E4%B8%87%E6%8E%A5%E7%B6%9A%E3%82%92%E9%81%94%E6%88%90%E3%81%99%E3%82%8B%E3%81%BE%E3%81%A7%E3%81%AE%E8%A9%B1-cf5cd310a71d)

### Wandbox 関連

- [clang-8.0.0 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-clang-8-0-0-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-9edf4cb7cec2)
- クライアントのブラウザ上で任意の JavaScript コードが実行できる脆弱性を修正しました → [melpon/wandbox#262](https://github.com/melpon/wandbox/issues/262)
- [php-7.3.3 を追加しました](https://medium.com/wandbox-org/wandbox-%E3%81%AB-php-7-3-3-%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-1b5d9f32c569)

### Wandbox スポンサー関連

以下の企業スポンサーを追加/更新しました。

- [株式会社フィックスターズ](http://www.fixstars.com/)
- [株式会社Preferred Networks](https://www.preferred-networks.jp/)

以下の個人スポンサーを追加/更新しました。

- [@char8_t](https://twitter.com/char8_t)
- [@ignis_fatuus](https://twitter.com/ignis_fatuus)
- [sublimer](https://twitter.com/lz650sss)
- 沖　観行
- [Usagi Ito](https://twitter.com/USAGI_WRP)
- [@cpp_akira](https://twitter.com/cpp_akira)
- [@take_cheeze](https://github.com/take-cheeze)
- [@tzik_tack](https://twitter.com/tzik_tack)
- [@wraith13](https://twitter.com/wraith13)
- [@srz_zumix](https://twitter.com/srz_zumix)
- [@nobu_k](https://twitter.com/nobu_k)
- [tai2](https://blog.tai2.net/pages/about.html)

### momo 関連

- M73 対応版で macOS だとセグフォする問題について [調査しました](https://github.com/shiguredo/momo/pull/59#issuecomment-469357182)

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- あるプログラミング教育系のサイトで C と C++ を扱うということで、そのコンサルティングをやっています
- gRPC C++ を使って開発する仕事を受けました(詳細は非公開)

### その他

- Yacto にマイグレーションファイルの検証機能を実装して 2.0.0-pre.8 をリリースしました。[CHANGELOG](https://github.com/gumi/yacto/blob/master/CHANGELOG.md#200-pre8)
- Yacto のマイグレーション時に存在しないモデルがあった場合に drop table するマイグレーションファイルを吐き出す機能を追加して 2.0.0-pre.9 をリリースしました。 [CHANGELOG](https://github.com/gumi/yacto/blob/master/CHANGELOG.md#200-pre9)

## 0.34.1

### Wata 関連

- Medium を利用し始めて、[Wata の情報を公開](https://link.medium.com/UOpDBi2OqU) しました
- [RFC 3533](https://melpon.github.io/rfc/rfc3533.xml) と [RFC 7845](https://melpon.github.io/rfc/rfc7845.xml) を読んで、Opus を Ogg コンテナに詰めて Google の Cloud Speech-to-Text に送信する仕組みを Wata に実装しました。
- 下記の VAD フラグの知識を使って、無声区間をちゃんと検出するようにしました。

### Wandbox 関連

- gcc-8.3.0 を追加しました

### Wandbox スポンサー関連

以下の個人スポンサーを追加/更新しました

- [堀尾典孝](https://twitter.com/holyshared)

### その他

- あるプログラミング教育系のサイトで C と C++ を扱うということで、そのコンサルティングを受けました
- [RFC 6716](https://melpon.github.io/rfc/rfc6716.xml) を軽く読んで、パケットやフレームのバイナリ構造や DTX や VAD フラグについて理解を深めました
- [resty-auth-serve](https://github.com/melpon/resty-auth-serve) で、認証付きの静的ファイル配信サーバを実装しました。OpenResty を使って Google 認証を掛けた上で S3 のファイルを取得してクライアントに返す、という実装を書き、それを AWS Fargate 上にデプロイする CloudFormation のスクリプトを書きました。

## ルール

["じぶんリリースノート" と称した月報を続けて3年が経った](https://blog.a-know.me/entry/2019/02/02/214612) のルールをほぼそのまま利用する。

- 毎月月初に "新しい自分" がリリースされた、ということにして月報代わりに書いていく
- バージョン番号は `0.年齢.月齢` にして、リリース前は後ろに `-dev` を付ける
- あの世へ行ったらメジャーバージョンを上げる
