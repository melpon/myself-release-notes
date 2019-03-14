# じぶんリリースノート

## 0.34.2-dev

### Wata 関連

- （負荷テストの件について書く）

### Wandbox 関連

- （多分 Boost 1.70.0 あたりが来そう）

### Wandbox スポンサー関連

以下の企業スポンサーを追加/更新しました。

- [株式会社フィックスターズ](http://www.fixstars.com/)

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

### momo 関連

- M73 対応版で macOS だとセグフォする問題について [調査しました](https://github.com/shiguredo/momo/pull/59#issuecomment-469357182)

### 仕事状況

- [株式会社gumi](https://gu3.co.jp/) で開発支援をやっています
- OSS である [WebRTC Native Client Momo](https://github.com/shiguredo/momo) のアップデートや機能追加する仕事をやっています
- あるプログラミング教育系のサイトで C と C++ を扱うということで、そのコンサルティングをやっています
- gRPC C++ を使って開発する仕事を受けました(詳細は非公開)

### その他

- Yacto にマイグレーションファイルの検証機能を実装して 2.0.0-pre.8 をリリースしました。[CHANGELOG](https://github.com/gumi/yacto/blob/master/CHANGELOG.md#200-pre8)

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
