# じぶんリリースノート

## 0.34.1-dev

### Wata 関連

- Medium を利用し始めて、[Wata の情報を公開](https://link.medium.com/UOpDBi2OqU) しました
- [RFC 3533](https://melpon.github.io/rfc/rfc3533.xml) と [RFC 7845](https://melpon.github.io/rfc/rfc7845.xml) を読んで、Opus を Ogg コンテナに詰めて Google の Cloud Speech-to-Text に送信する仕組みを Wata に実装しました。
- 下記の VAD フラグの知識を使って、無声区間をちゃんと検出するようにしました。

### Wandbox 関連

- gcc-8.3.0 を追加しました

### その他

- あるプログラミング教育系のサイトで C と C++ を扱うということで、そのコンサルティングを受けました
- [RFC 6716](https://melpon.github.io/rfc/rfc6716.xml) を軽く読んで、パケットやフレームのバイナリ構造や DTX や VAD フラグについて理解を深めました
- [resty-auth-serve](git@github.com:melpon/resty-auth-serve.git) で、認証付きの静的ファイル配信サーバを実装しました。OpenResty を使って Google 認証を掛けた上で S3 のファイルを取得してクライアントに返す、という実装を書き、それを AWS Fargate 上にデプロイする CloudFormation のスクリプトを書きました。

## ルール

["じぶんリリースノート" と称した月報を続けて3年が経った](https://blog.a-know.me/entry/2019/02/02/214612) のルールをほぼそのまま利用する。

- 毎月月初に "新しい自分" がリリースされた、ということにして月報代わりに書いていく
- バージョン番号は `0.年齢.月齢` にして、リリース前は後ろに `-dev` を付ける
- あの世へ行ったらメジャーバージョンを上げる
