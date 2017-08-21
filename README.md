# 東方Projectアレンジ曲管理ソフト（仮）
このソフトウェアは、東方Projectのアレンジ楽曲を管理するためのソフトウェアです。

**なお、開発中につき、このドキュメントには未実装の機能の説明が含まれています。また、大幅な仕様変更が行われる場合があります。**

## 何をするためのソフトですか？
このソフトウェアは、「東方旧作のアレンジを聴きたい」「霧雨魔理沙のテーマ曲のアレンジが聴きたい」「蓮台野夜行の収録曲順にプレイリストを作りたい」「誰それさんがボーカルの曲だけのプレイリストを作りたい」「どこそこのサークルの楽曲のプレイリストを作りたい」といった、通常の音楽再生プレイヤーでは難しいようなプレイリストを作ることを目的としたソフトウェアです。

従来の音楽プレイヤーではその曲が何のアレンジであるかを指定するような項目が無いため、例えば曲名に原曲名を入れるとか、アーティスト名にサークル名を含めるといった必要がありました。

このソフトウェアでアレンジ楽曲に原曲の情報を指定したり、アルバムに頒布サークルの情報を指定したりすることで、管理が容易になります。

また、サークルやアーティストにTwitter IDやWebサイトのURL情報を指定して、イベント前にリストを作成して情報を確認したりすることも可能（予定）です。

## 使い方
1. サークル情報を入力します。
1. 頒布イベント情報を入力します。
1. アーティスト情報を入力します。
1. アルバム情報を入力します。
1. 楽曲情報を入力します。（←ここまで実装）
1. 指定した条件に基づいてプレイリストを作成します。
1. プレイリストをお好みの音楽プレイヤーに取り込みます。
1. (ﾟдﾟ)ｳﾏｰ

## 使い方メモ
- 原曲やアーティスト名の削除ってどうやるの？
  - 右クリックメニュー
- 編集フォームで他の項目の編集ってできない？
  - IDの値を変えると項目が変わります。変える前のデータは保存されません。

## インストール
[Release](https://github.com/shiosyakeyakini/TohoMusicManager/releases)より最新版をダウンロードできます。

なお、実行には[Microsoft .NET Framework Version 2.0 Runtime](https://www.microsoft.com/ja-jp/download/details.aspx?id=6523)が必要となります。たぶんVistaとか7とかには標準でついています。98/98SE/Me/XPあたりは標準でついてないかもしれないので、適当にインストールしてください。

Monoとかは確認してないですが対応したいですね。普段はUbuntu使いなので。

## 天空璋ネタバレ回避・アレンジ登録したいんですけど
現在のデータベースには3面までの曲のデータが入力されています。そのうち対応します。

## その他
ソースコードも公開します。このプログラムは東方Projectのアレンジ楽曲にのみ絞っていますが、たぶんもっと汎用的なプログラムにもできる気がします。

なおはじめてVB使いました（ぇ

【ゆるぼ】このソフトウェアの名前をゆるぼしてます。

## ライセンス
このソフトウェアは、以下のライブラリに依存しています。

- [System.Data.SQLite（パブリックドメイン）](https://system.data.sqlite.org/index.html/doc/trunk/www/copyright.wiki)

このソフトウェアのソースコード、バイナリ、初期登録されたデータベースについてはフリー（自由な）ソフトウエアです。 

あらゆる改変の有無に関わらず、また商業的な利用であっても、自由にご利用、複製、再配布することができますが、全て無保証とさせていただきます。

These source code, binary, databases are free software. 

Unlimited permission is granted to use, copy, and distribute them, with or without modification, either commercially or noncommercially. 

THESE SOFTWEARS ARE PROVIDED "AS IS" WITHOUT WARRANTY.

## 何かありましたら
[Twitter](https://twitter.com/shiosyakeyakini)までどうぞ

## 予定
- 原曲関連情報の編集機能
- データの削除機能
- 仮名フォームの自動入力機能
- MP3タグの読み込み機能、再生時間読み込み機能
- SQL例外の日本語化（部分的に実装）
- 指定したフォーマットでのMP3タグ/ファイル名変更機能
- 音楽再生機能
- 楽曲データ検索・抽出機能
- プレイリスト出力機能
 - プレイリストのフォルダ置換機能
 - UNIX/Windowsのパス表現切り替え機能
- 日付フォームのNull値許容
- コンボボックスのNull値指定時の値改善
 - 指定しない、という選択肢がいま無いのでその辺ちゃんとしたい
- SQLiteの外部キー指定
- Twitterアカウントリスト表示機能
- WebサイトURLリスト表示機能
- UI/設定パラメータ等の設定機能
 - 原曲情報並び替え順とか
 - フォント変更
- SQLクエリの外部ファイル化
- アルバム新規追加時にフォルダ指定したら楽曲自動追加するとか
- 値編集可能なコンボボックスのDataSource指定
- データベースのCSVインポート・エクスポート機能


他にこういう機能欲しい！みたいなのがあれば教えてもらえれば追加するかもしれません。
