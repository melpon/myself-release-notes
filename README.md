# じぶんリリースノート

## 0.34.3-dev

### Wata 関連

- Windows で動きました → [Wata をWindows対応しました](https://medium.com/wandbox-org/wata-%E3%82%92windows%E5%AF%BE%E5%BF%9C%E3%81%97%E3%81%BE%E3%81%97%E3%81%9F-59a0259f436f)
- gRPC 1.20.0 にアップデートしました
- Wata をバーチャルライバー特化型の配信とするように方針を決めました
- Wata で RTMP のデータをブラウザに配信して表示するのを実装しました → https://twitter.com/melponn/status/1123135647840067584

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
