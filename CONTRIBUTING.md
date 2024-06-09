# 貢献者ガイドライン

## 始めに

まず初めに、VOICEVOXプロジェクトに関心を寄せて頂きありがとうございます。
私たちは、あなたが積極的に参加してくれることを歓迎します。

実際に参加しようとすると、どんなコミュニティにもルールが存在し、そこを理解しないとハードルを高く感じてしまうことがあります。

このガイドラインは、その部分を出来るだけ分かりやすく文章として残し、コミュニティへ参画しやすい環境を提供するために執筆されました。なお、新たな貢献者が参入しやすくするよう細かく解説しているため、慣れている方には不要な説明も含まれます。プロジェクトは意志ある貢献者を歓迎しておりますので、ドキュメントを読んで参画してみてください。

## 担当

|役割             | 担当                  |
|-----------------|-----------------------|
|プロダクトオーナー |@Hiroshiba             |
|メンテナー       |@Hiroshiba、@y-chan、@qryxip    |

## 参加の心得

VOICEVOXプロジェクトは、いわゆる集団開発型のオープンソースソフトウェアにあたります。参加を望む方は、下記のことに注意して参加する必要があります。

* [VOICEVOXの目標](docs/ミッション・バリュー・ビジョン.md)に照らし合わせて提案を行うと会話がスムーズです。

* 実施する中身については、コミュニティ内で会話をしながら合意を取っていく必要があります。また、プロジェクト方針により採用が拒絶されるケースがあります。

* 集団開発では、会話をしながら物を作っていくことが１つの醍醐味でもあります。一人で作品を作る時に比べて丁寧なコミュニケーションが必要です。会話相手に対して常に敬意を払ってください。

* プロジェクトへの参画に当たっては、年齢、国籍、境遇、性別などは関係ありません。これらの差別を行うことをプロジェクトは容認しません。

* プロジェクトは著作者や著作物を尊重します。常に他者の権利やライセンスを順守するように意識しています。プロジェクトへの貢献にあたっては、盗用したプログラムの提出は行わないでください。

* コントリビューターとして提供したプログラムは、プロジェクトが定義するライセンスで取り扱われる事に注意してください。

* プライバシーに関わる実装や、コンピュータに危害を与える可能性がある実装に関しては慎重な議論が必要です。実装を先におこなうのではなく、必ず合意形成をしてください。

## 貢献の仕方

このドキュメントでは、主にプログラムの改良を手伝ってくださる方に向けた、「参加の仕方」をガイドします。

VOICEVOXには、下記のような貢献の仕方があります。

* ユーザとして使う
* 記事や動画を公開して広める
* プログラムの改良を手伝う
* ドキュメントなどを書く

プログラムは３部構成に分かれているので、該当する部分に該当するプロジェクトに参加しましょう。

|種類           |ページ                                                      |役割                                    |
|---------------|------------------------------------------------------------|----------------------------------------|
|VOICEVOX       |[プロジェクト](https://github.com/VOICEVOX/voicevox/)       |主にユーザインタフェイス(エディタ)部分  |
|VOICEVOX_ENGINE|[プロジェクト](https://github.com/VOICEVOX/voicevox_engine/)|主にAPI実装や音声合成を行う部分         |
|VOICEVOX_CORE  |[プロジェクト](https://github.com/VOICEVOX/voicevox_core/)  |主に推論する部分                        |

なお、全体構成を学びたい場合は、[こちら](docs/全体構成.md)が参考になることでしょう。

## 初心者歓迎タスク

あなたがプログラム開発を学んだり、オープンソース開発コミュニティで活動することを実践したい場合は、既にコミュニティのIssuesで提案されている「初心者歓迎タスク」に参加することをお勧めします。

「初心者歓迎タスク」は、VOICEVOXプロジェクトとしては「難易度が比較的低い案件であるが、必要とされているもの」となっており、比較的一通りの工程をスマートに学びながら貢献することができます。

|種類           |ページ            |
|---------------|------------------|
|VOICEVOX       |[初心者歓迎タスク](https://github.com/VOICEVOX/voicevox/issues?q=is%3Aissue+is%3Aopen+label%3A%E5%88%9D%E5%BF%83%E8%80%85%E6%AD%93%E8%BF%8E%E3%82%BF%E3%82%B9%E3%82%AF)|
|VOICEVOX_ENGINE|[初心者歓迎タスク](https://github.com/VOICEVOX/voicevox_engine/issues?q=is%3Aissue+is%3Aopen+label%3A%E5%88%9D%E5%BF%83%E8%80%85%E6%AD%93%E8%BF%8E%E3%82%BF%E3%82%B9%E3%82%AF)|
|VOICEVOX_CORE  |[初心者歓迎タスク](https://github.com/VOICEVOX/voicevox_core/issues?q=is%3Aissue+is%3Aopen+label%3A%E5%88%9D%E5%BF%83%E8%80%85%E6%AD%93%E8%BF%8E%E3%82%BF%E3%82%B9%E3%82%AF)|

## 事前準備

ここからはWindowsをお使いの方が、VOICEVOX(エディタ)の環境を作るケースを想定し、話を進めます。まず、テスト版VOICEVOXの環境を構築しましょう。

### 1. 製品版VOICEVOXを導入する

* まず[VOICEVOXの製品版](https://voicevox.hiroshiba.jp/)を導入します。これによりすぐ使えるVOIECVOXエンジンを手に入れることができます。

### 2. 開発環境の構築

* 必須ツール
  * [Node.js](https://nodejs.org/en/download/releases/)
    [こちら](https://github.com/VOICEVOX/voicevox/blob/main/.node-version)に記載されているバージョンのインストーラを入手し、インストールします。

* 必要に応じて
  * [Git](https://git-scm.com/downloads)
  * [Visual Studio Code](https://code.visualstudio.com/)
  * [GitHub CLI](https://github.com/cli/cli#installation)
  * [typos](https://github.com/crate-ci/typos#install) (誤字チェックする場合)
  * [Tortoise Git](https://tortoisegit.org/download/) (エクスプローラ上で操作したい場合)

### 3. フォークする

* プロジェクトの複製をつくって自分のGitHubリポジトリにもってくる作業をフォークと言います。[こちら](https://github.com/VOICEVOX/voicevox/fork)を押して、フォークを実施します。

### 4. ソースコードを手に入れる（クローン）

* 自分のGitHubリポジトリにあるソースコードをGitHubから作業用パソコンに持ってきます。

#### 4.1 コマンドラインで行う場合
  
* GitHub コマンド(GitHub CLI)を使う場合

```bash
gh repo clone https://github.com/(個人のGitHubアカウント名)/voicevox.git
```

* Git コマンド(Git CLI)を使う場合

```bash
git clone git@github.com:(個人のGitHubアカウント名)/voicevox.git
```

#### 4.2 GUIで行う場合

* Visual Studio CodeやTortoise Gitなどのツールを用いて入手します。
* 指定するURLはツールによって異なりますが、`git@github.com:(個人のGitHubアカウント名)/voicevox.git`や`https://github.com/(個人のGitHubアカウント名)/voicevox.git`となります。

### 5. 必要なプログラムをダウンロードする

* 手順４で手に入れたフォルダを開いて、コマンドプロンプトを開きます。
* 環境を準備するコマンド ``npm ci`` を実行してください。自動的にダウンロードされます。
* ツールの組み合わせや実装に関する警告が表示されますが、開発環境を作るうえでは無視して差し支えありません。

### 6. エンジンを指定する

* `.env.production`というファイルがありますので、コピーして、名前を`.env`にします。
* ファイルをエディタでひらいて、`VITE_DEFAULT_ENGINE_INFOS`内の`executionFilePath`に手順１のフォルダ名をいれます。たとえば製品版をインストーラで導入し、インストール先を変更していない場合は、下記のように書き換えて保存します。

```ini
VITE_APP_NAME=voicevox
VITE_DEFAULT_ENGINE_INFOS=`[
    {
        "uuid": "074fc39e-678b-4c13-8916-ffca8d505d1d",
        "name": "VOICEVOX Engine",
        "executionEnabled": true,
        "executionFilePath": "vv-engine/run.exe",
        "executionArgs": [],
        "host": "http://127.0.0.1:50021"
    }
]`
```

* あなたがVOICEVOX製品版のインストール先を変更している場合は個別で指定します。たとえば、`D:\VOICEVOX0.14.1`に製品版をインストールしている場合は、下記のように書き換えて保存します。

```text
"executionFilePath": "D:/VOICEVOX0.14.1/vv-engine/run.exe",   
```

### 7. 始動してみる

* `npm run electron:serve`を実行します。
* 設定が正しければ、開発環境が起動するはずです。

## プロジェクトへの貢献手順

### 1. 提案と調整

まず、下記のことがあれば、Issueとして登録をしましょう。

* プログラムの仕様を変更したい
* 新機能を追加したい
* バグを確認した

#### 1.1 提案

その際、VOICEVOXのどの部分に関して提案をしたいのかを考えて提案しましょう。また、個人がわかる範囲で問題ないので、「改良されることで良くなる点」や「悪くなる点・影響を受ける点」を書いて登録します。

#### 1.2 相談

この段階では、関係者と実装に関しての制約や影響範囲、プロジェクト方針として優先度や実施してよいかをすり合わせます。
  
コミュニティには様々な技術領域・技量の方が混在しています。会話の途中で分からないことが出てくることも多いかとおもいます。不明点は質問し、理解を深めていきましょう。

#### 1.3 着手宣言
  
既にIssueとして登録されている課題に着手したい場合は、他の貢献者と作業が重複しないように、当該Issueのページで「私が着手する」旨の宣言を行ってください。

なお、着手宣言をした後は下記手順で作業をすることになります。定期的に相談や進捗をレポートしましょう。また、作業時間や技量などにより、コードを書き終えられないケースはあります。その場合は、抱え込まずにIssueページで相談をしてください。

### 2. ブランチを作る

* 自分の作業フォルダ内に、今回加工するために作業エリアを作ります。
* いくつかの案件を並走するなら、この手順でブランチをいくつか作ります。
* ブランチ名は、自分のわかりやすいもので構いません。

### 3. プログラムを加工する

実際にプログラムを書きます。プログラムを書くにあたっては、いくつかの流儀があります。

* 関数名や変数名は極力キャメルケースで命名する必要があります。何かしらの制約上キャメルケースで命名出来ない場合は、コメントを残します。

```python
// FIXME: ●●のため、キャメルケースが採用できない
```

* 今回コーディングするが、構造制約などで「本来ありたい構造と異なる」場合にも、コメントを残します。

```python
// TODO: ●●を使わずに、●●となる実装にしたい
```

* 変数名や型名の命名にあたっては、その仕組みで一般的に使われる命名則があれば、それらを優先して採用します。
* 関数名は、動詞＋役割となるように設定をします。
  |命名例      |役割                          |
  |------------|------------------------------|
  |setVolume() |音量を設定                    |
  |getVolume() |音量を取得                    |
  |isMuted     |ミュート状態の取得(boolean)   |

* 変数や関数名につける英語は極力省略しないようにします。
* コードは分かりやすさや単純さを保つようにしてください。
* 不必要な定義や、作業中のコードは、コード提出までに除去しましょう。

### 4. 事前テスト

* 提出前にコードをテストします。テストにはいくつかのツールを使います。このガイドラインの手順で進んでいれば既に必要なものはそろっている

* 記述コードがコーディングルールに沿っていることを確認します。（特に今回の作業によって警告やエラーが増えていないかどうかに注目してください）

  ```bash
  npm run lint
  npm run fmt
  ```

* TypeScriptの型チェックを行います。

  ```bash
  npm run typecheck
  ```

* Markdownの記述が正しいことを確認します。
  
  ```bash
  npm run markdownlint ./*/*.md
  ```

* 命名に使っている英語が誤っていないことを確認します。

  ```bash
  typos
  ```

* 個人環境でVOICEVOXを実行し、提出前に、一通り動くことを確認します。

  ```bash
  npm run electron:serve
  ```

* 使用するライブラリのライセンスに使用出来ないものが使われていないことを確認します。

  ```bash
  npm run license:generate -- -o voicevox_licenses.json
  ```

* e2eテストの内容を確認します。

  ```bash
  npm run test:unit
  npm run test:browser-e2e
  npm run test:electron-e2e
  ```

  * e2eテストは実際には自分が提出する範囲外の指摘をしたり、完全に警告が消えないことがあります。
  * 確認の目安としては、加工前後で e2eテスト結果による指摘が増えていないことを確認してください。（チェックアウト時点でe2eテストの指摘が残っていることがあるため、前後の差分で判断するのが良いでしょう）
  * 提出する範囲で指摘されているようであれば提出前に訂正しましょう。
  * e2eテスト結果を修正出来ない事情がある場合や判断に迷う場合は、レビュー時に相談をしましょう。

### 5. コードの提出

* 先に個人のリポジトリにコミットします。この時、詳細欄に変更に関する具体内容を確実に記入しましょう。タイトルは簡素で分かりやすいものが好まれます。

* コミットが終わったら、コードをコミュニティに提案しましょう。作成したコードをコミュニティへ提案する作業の事を「Pull Request（プルリクエスト）」といいます。

* Pull Requestには2つの種類があります。

  * Draft Pull Request
  * Pull Request

* Draft Pull Requestは、進捗状況を共有するために使います。検討の歩みがわかるため、議論が必要な項目では特に有効な手段です。

* Draft Pull Requestの場合は、タイトルの先頭に `WIP:` をつけると見た目に分かりやすいです。

* 凡そ問題ないと判断できたら、Pull Requestを提出します。
この先は共同作業になるので、今一度作業忘れや問題がないか確認をしてください。

* Pull Requestを出すときには、関連するIssueのナンバーを記載しておきます。

  記入例：

  ```text
    タイトル：起動時の待ち時間を低減する
    内容：初期化を並列処理することで待ち時間を短縮させる
    関連Issue：ref #0000
  ```

* 議論する場所が分散する事を防ぐため、Pull Requestするタイミングで問題提起した方の番号を閉じましょう。コメントに下記のような表記をすることでIssue側の議論を閉じることができます。

  ```text
     close #0000
  ```

### 6. コードレビュー

* レビュー担当やコミュニティメンバーによってソースの査読が行われます。課題が発見された場合には、記述修正の提案がおこなわれます。

* 納得できれば「提案通りに直す」方法もありますが、課題があると感じていれば、議論を行い最良点を探してください。

* この段階では、既にPull Requestが出されていますので、自分のリポジトリに修正分をプッシュするだけで自動的に追跡されます。

* 現在のVOICEVOXのマージルールでは、基本的に1名以上の査読が必要となっています。

### 7. コンフリクト対応

* レビューが終わると、マージ(取り込み)準備が始まります。

* 作業中に他の修正が取り込まれている場合には、修正箇所が重なる「コンフリクト」という現象が発生することがあります。

* コンフリクトが発生した場合には、Pull Requestのページに「コンフリクトが発生している」と表示されるので、次の手順で修正を行います。

  1. 自分の作業リポジトリにプルします。プル元は、自分のGitHubリポジトリではなく、[VOICEVOXのリポジトリ](https://github.com/VOICEVOX/voicevox.git)を指定します。

  2. 変更差分をみながら、コンフリクトしている部分を正しい実装に修正します。

  3. 変更がすべて終わったら、手順４にあった「事前テスト」を改めて実施します。

  4. 問題なければ、コミットします。

  5. VOICEVOXのPull Requestページで自動検査処理が走ります。この画面で「コンフリクトが発生した」という表示が消えたことを確認してください。

* お疲れさまでした。この工程までいけば、貢献者の仕事はおわりです。
* マージ担当者が確認後、マージ処理をします。
* マージが終われば、個人のブランチは削除できます。

### その他

* VOICEVOXプロジェクトメンバーは、貢献者が活動しやすいようサポートや相談に応じています。
* こまったり、わからないことが発生したら、プロジェクトメンバーに相談しましょう。
* [Discordコミュニティ](https://discord.gg/gJamMrqFHg)もあります。議論しながら考えをまとめたい場合など、コミュニティをうまく活用するとよいでしょう。
* 諸事情で処理が継続できなくなった場合や、技術的ハードルが高かったりして心が折れたときは、ギブアップを宣言することも可能です。調整が可能な場合もあるので、宣言する前に相談をすることをお勧めします。

## 参考情報

* 実装時のデザインに関しては、[UX・UIデザインの方針](docs/UX・UIデザインの方針.md)を参考に実装してください。

* 設計詳細については、[細かい設計方針](docs/細かい設計方針.md)を参考にしてください。

* VOICEVOXは、様々な技術を使って実装しており、技術の理解が無いと読みづらい部分があります。全体の構造については、[コードの歩き方](docs/コードの歩き方.md)を参考にしてみてください。

* 色については、[色の実装](docs/色について.md)についてのドキュメントを参考にしてみてください。

* VOICEVOXで使用するフォントは、[フォントについて](docs/フォントについて.md)に生成方法などが書いてあります。