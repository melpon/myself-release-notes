# じぶんリリースノート

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

["じぶんリリースノート" と称した月報を続けて3年が経った](https://blog.a-know.me/entry/2019/02/02/214612) のルールをほぼそのまま利用する。

- 毎月月初に "新しい自分" がリリースされた、ということにして月報代わりに書いていく
- バージョン番号は `0.年齢.月齢` にして、リリース前は後ろに `-dev` を付ける
- あの世へ行ったらメジャーバージョンを上げる
