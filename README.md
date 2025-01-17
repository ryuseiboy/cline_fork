# Cline – OpenRouterで1位

<p align="center">
  <img src="https://media.githubusercontent.com/media/cline/cline/main/assets/docs/demo.gif" width="100%" />
</p>

<div align="center">
<table>
<tbody>
<td align="center">
<a href="https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev" target="_blank"><strong>VS Marketplaceからダウンロード</strong></a>
</td>
<td align="center">
<a href="https://discord.gg/cline" target="_blank"><strong>Discord</strong></a>
</td>
<td align="center">
<a href="https://www.reddit.com/r/cline/" target="_blank"><strong>r/cline</strong></a>
</td>
<td align="center">
<a href="https://github.com/cline/cline/discussions/categories/feature-requests?discussions_q=is%3Aopen+category%3A%22Feature+Requests%22+sort%3Atop" target="_blank"><strong>機能リクエスト</strong></a>
</td>
<td align="center">
<a href="https://cline.bot/join-us" target="_blank"><strong>採用中！</strong></a>
</td>
</tbody>
</table>
</div>

CLIとエディタを使用できるAIアシスタント、Clineをご紹介します。

[Claude 3.5 Sonnetのエージェント的なコーディング機能](https://www-cdn.anthropic.com/fed9cc193a14b84131812372d8d5857f8f304c52/Model_Card_Claude_3_Addendum.pdf)により、Clineは複雑なソフトウェア開発タスクをステップバイステップで処理できます。ファイルの作成・編集、大規模プロジェクトの探索、ブラウザの使用、ターミナルコマンドの実行（許可後）を可能にするツールにより、コード補完やテクニカルサポート以上の支援が可能です。ClineはModel Context Protocol (MCP)を使用して、新しいツールを作成し、自身の機能を拡張することもできます。従来の自律型AIスクリプトは独立した環境で実行されますが、この拡張機能は、ファイルの変更とターミナルコマンドを承認するためのヒューマンインザループGUIを提供し、エージェント型AIの可能性を安全にアクセス可能な方法で探索できます。

1. タスクを入力し、モックアップを機能的なアプリに変換したり、スクリーンショットでバグを修正したりするための画像を追加します。
2. Clineは、既存のプロジェクトで作業するために、ファイル構造とソースコードASTの分析、正規表現検索、関連ファイルの読み取りから始めます。コンテキストに追加する情報を慎重に管理することで、コンテキストウィンドウを圧迫することなく、大規模で複雑なプロジェクトでも価値のある支援を提供できます。
3. 必要な情報を得たClineは以下のことができます：
    - ファイルの作成・編集とリンター/コンパイラーエラーの監視。これにより、不足しているインポートや構文エラーなどの問題を自主的に修正できます。
    - ターミナルで直接コマンドを実行し、作業中にその出力を監視。例えば、ファイル編集後の開発サーバーの問題に対応できます。
    - Web開発タスクでは、サイトをヘッドレスブラウザで起動し、クリック、入力、スクロール、スクリーンショットやコンソールログの取得が可能で、ランタイムエラーや視覚的なバグを修正できます。
4. タスクが完了すると、Clineは`open -a "Google Chrome" index.html`のようなターミナルコマンドで結果を表示し、ボタンをクリックするだけで実行できます。

> [!TIP]
> `CMD/CTRL + Shift + P`ショートカットを使用してコマンドパレットを開き、"Cline: Open In New Tab"と入力すると、エディタのタブとして拡張機能を開くことができます。これにより、ファイルエクスプローラーと並行してClineを使用し、ワークスペースの変更をより明確に確認できます。

---

<img align="right" width="340" src="https://github.com/user-attachments/assets/3cf21e04-7ce9-4d22-a7b9-ba2c595e88a4">

### あらゆるAPIとモデルを使用

ClineはOpenRouter、Anthropic、OpenAI、Google Gemini、AWS Bedrock、Azure、GCP VertexなどのAPIプロバイダーをサポートしています。OpenAI互換のAPIを設定したり、LM Studio/Ollamaを通じてローカルモデルを使用することもできます。OpenRouterを使用する場合、拡張機能は最新のモデルリストを取得し、新しいモデルが利用可能になり次第使用できます。

また、タスク全体と個々のリクエストのトークン総数とAPI使用コストを追跡し、支出状況を常に把握できます。

<!-- Transparent pixel to create line break after floating image -->

<img width="2000" height="0" src="https://github.com/user-attachments/assets/ee14e6f7-20b8-4391-9091-8e8e25561929"><br>

<img align="left" width="370" src="https://github.com/user-attachments/assets/81be79a8-1fdb-4028-9129-5fe055e01e76">

### ターミナルでコマンドを実行

新しい[VSCode v1.93のシェル統合アップデート](https://code.visualstudio.com/updates/v1_93#_terminal-shell-integration-api)のおかげで、Clineはターミナルで直接コマンドを実行し、その出力を受け取ることができます。これにより、パッケージのインストールやビルドスクリプトの実行からアプリケーションのデプロイ、データベースの管理、テストの実行まで、幅広いタスクを実行できます。Clineは開発環境とツールチェーンに適応し、仕事を正しく完了させます。

開発サーバーのような長時間実行されるプロセスの場合、「実行中に続行」ボタンを使用して、コマンドがバックグラウンドで実行されている間にClineがタスクを続行できるようにします。Clineが作業を進める中で、新しいターミナル出力が通知され、ファイル編集時のコンパイルエラーなどの問題に対応できます。

<!-- Transparent pixel to create line break after floating image -->

<img width="2000" height="0" src="https://github.com/user-attachments/assets/ee14e6f7-20b8-4391-9091-8e8e25561929"><br>

<img align="right" width="400" src="https://github.com/user-attachments/assets/c5977833-d9b8-491e-90f9-05f9cd38c588">

### ファイルの作成と編集

Clineはエディタ内でファイルを直接作成および編集し、変更の差分ビューを表示します。差分ビューエディタでClineの変更を編集または元に戻すことができ、チャットでフィードバックを提供して満足するまで結果を調整できます。Clineはリンター/コンパイラーエラー（不足しているインポート、構文エラーなど）も監視し、途中で発生する問題を自主的に修正できます。

Clineによるすべての変更はファイルのタイムラインに記録され、必要に応じて変更を追跡および元に戻す簡単な方法を提供します。

<!-- Transparent pixel to create line break after floating image -->

<img width="2000" height="0" src="https://github.com/user-attachments/assets/ee14e6f7-20b8-4391-9091-8e8e25561929"><br>

<img align="left" width="370" src="https://github.com/user-attachments/assets/bc2e85ba-dfeb-4fe6-9942-7cfc4703cbe5">

### ブラウザを使用

Claude 3.5 Sonnetの新しい[コンピュータ使用](https://www.anthropic.com/news/3-5-models-and-computer-use)機能により、Clineはブラウザを起動し、要素をクリックし、テキストを入力し、スクロールし、各ステップでスクリーンショットとコンソールログをキャプチャできます。これにより、インタラクティブなデバッグ、エンドツーエンドテスト、さらには一般的なWeb使用が可能になります。これにより、視覚的なバグやランタイムの問題を手取り足取りでエラーログをコピー＆ペーストすることなく修正できます。

Clineに「アプリをテストして」と頼んでみてください。彼は`npm run dev`のようなコマンドを実行し、ローカルで実行されている開発サーバーをブラウザで起動し、一連のテストを実行してすべてが正常に動作することを確認します。[デモはこちらをご覧ください。](https://x.com/sdrzn/status/1850880547825823989)

<!-- Transparent pixel to create line break after floating image -->

<img width="2000" height="0" src="https://github.com/user-attachments/assets/ee14e6f7-20b8-4391-9091-8e8e25561929"><br>

<img align="right" width="350" src="https://github.com/user-attachments/assets/ac0efa14-5c1f-4c26-a42d-9d7c56f5fadd">

### 「ツールを追加して...」

[Model Context Protocol](https://github.com/modelcontextprotocol)のおかげで、Clineはカスタムツールを通じて機能を拡張できます。[コミュニティ製のサーバー](https://github.com/modelcontextprotocol/servers)を使用することもできますが、Clineは代わりに特定のワークフローに合わせたツールを作成してインストールできます。Clineに「ツールを追加して」と頼むだけで、MCPサーバーの作成から拡張機能へのインストールまで、すべてを処理します。これらのカスタムツールはClineのツールキットの一部となり、将来のタスクで使用できるようになります。

-   「Jiraチケットを取得するツールを追加して」：チケットACを取得し、Clineに作業を依頼
-   「AWS EC2を管理するツールを追加して」：サーバーメトリクスを確認し、インスタンスをスケールアップまたはダウン
-   「最新のPagerDutyインシデントを取得するツールを追加して」：詳細を取得し、Clineにバグ修正を依頼

<!-- Transparent pixel to create line break after floating image -->

<img width="2000" height="0" src="https://github.com/user-attachments/assets/ee14e6f7-20b8-4391-9091-8e8e25561929"><br>

<img align="left" width="360" src="https://github.com/user-attachments/assets/7fdf41e6-281a-4b4b-ac19-020b838b6970">

### コンテキストを追加

**`@url`:** URLを貼り付けて拡張機能が取得し、Markdownに変換。最新のドキュメントをClineに提供したいときに便利

**`@problems`:** Clineが修正するためのワークスペースエラーと警告（「問題」パネル）を追加

**`@file`:** ファイルの内容を追加して、ファイルの読み取りを承認するAPIリクエストを節約（ファイルを検索して入力）

**`@folder`:** フォルダーのファイルを一度に追加して、ワークフローをさらにスピードアップ

<!-- Transparent pixel to create line break after floating image -->

<img width="2000" height="0" src="https://github.com/user-attachments/assets/ee14e6f7-20b8-4391-9091-8e8e25561929"><br>

<img align="right" width="350" src="https://github.com/user-attachments/assets/140c8606-d3bf-41b9-9a1f-4dbf0d4c90cb">

### チェックポイント：比較と復元

Clineがタスクを進める中で、拡張機能は各ステップでワークスペースのスナップショットを撮ります。「比較」ボタンを使用してスナップショットと現在のワークスペースの差分を確認し、「復元」ボタンを使用してその時点にロールバックできます。

たとえば、ローカルWebサーバーで作業する場合、「ワークスペースのみを復元」を使用してアプリの異なるバージョンを迅速にテストし、「タスクとワークスペースを復元」を使用して続行したいバージョンを見つけたときに使用します。これにより、進行状況を失うことなく異なるアプローチを安全に探索できます。

<!-- Transparent pixel to create line break after floating image -->

<img width="2000" height="0" src="https://github.com/user-attachments/assets/ee14e6f7-20b8-4391-9091-8e8e25561929"><br>

## 貢献

プロジェクトに貢献するには、[貢献ガイド](CONTRIBUTING.md)から基本を学び始めてください。また、[Discord](https://discord.gg/cline)に参加して、`#contributors`チャンネルで他の貢献者とチャットすることもできます。フルタイムの仕事を探している場合は、[採用ページ](https://cline.bot/join-us)で公開されているポジションを確認してください。

<details>
<summary>ローカル開発の手順</summary>

1. リポジトリをクローンします（[git-lfs](https://git-lfs.com/)が必要です）：
    ```bash
    git clone https://github.com/cline/cline.git
    ```
2. プロジェクトをVSCodeで開きます：
    ```bash
    code cline
    ```
3. 拡張機能とwebview-guiの必要な依存関係をインストールします：
    ```bash
    npm run install:all
    ```
4. `F5`を押して（または`Run`->`Start Debugging`）拡張機能が読み込まれた新しいVSCodeウィンドウを開きます。（プロジェクトのビルドに問題がある場合は、[esbuild problem matchers extension](https://marketplace.visualstudio.com/items?itemName=connor4312.esbuild-problem-matchers)をインストールする必要があるかもしれません。）

</details>

## ライセンス

[Apache 2.0 © 2024 Cline Bot Inc.](./LICENSE)
