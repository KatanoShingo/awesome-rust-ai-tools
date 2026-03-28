# 🛑 クラウドAIへの課金はもうやめよう。究極のローカルRust AI開発者スタック。

\!([https://img.shields.io/badge/build-passing-brightgreen?style=for-the-badge](https://www.google.com/search?q=https://img.shields.io/badge/build-passing-brightgreen%3Fstyle%3Dfor-the-badge))
\!([https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge](https://www.google.com/search?q=https://img.shields.io/badge/License-MIT-blue.svg%3Fstyle%3Dfor-the-badge))
\!([https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge](https://www.google.com/search?q=https://img.shields.io/badge/PRs-welcome-brightgreen.svg%3Fstyle%3Dfor-the-badge))
\!([https://img.shields.io/badge/Rust-100%25-orange?style=for-the-badge\&logo=rust](https://www.google.com/search?q=https://img.shields.io/badge/Rust-100%2525-orange%3Fstyle%3Dfor-the-badge%26logo%3Drust))

_まだ社外秘のコードベースをOpenAIに送信していますか？ ローカルでシンプルなLLMを動かすためだけに、500MBものPython環境の悪夢と格闘していますか？ それも今日で終わりにしましょう。_

ここは、完全に **Rust 🦀** で構築された、現代のAI開発者向けツールの決定版かつ、綿密にキュレーションされたリストです。これらのツールは爆速で、メモリ安全であり、CLIネイティブ、そしてローカルファーストで動作するように設計されています。Pythonのグローバルインタプリタロック（GIL）に別れを告げ、未来の開発者体験（DX）を手に入れましょう。

#### 🧠 Local LLM Runners (推論エンジン)

基盤となるレイヤーです。PythonのラッパーやCUDAの互換性問題に悩まされるのはやめましょう。これらのRustネイティブな推論エンジンは、最適化されたモデルをベアメタル上で直接実行します。

| リポジトリ URL                                                              | 🚀 一行でわかる魅力的な説明                                                                                | ⭐ Stars |
| :-------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------- | :------- |
| [huggingface/candle](https://github.com/huggingface/candle)                 | Rust向けのミニマリストMLフレームワーク。圧倒的なGPUサポートとWASMコンパイルを標準搭載。                    | 19.8k    |
| [tracel-ai/burn](https://github.com/tracel-ai/burn)                         | WebGPUをサポートし、学習とエッジデプロイメントをシームレスに繋ぐ次世代のディープラーニングフレームワーク。 | 14.7k    |
| (https://github.com/EricLBuehler/mistral.rs)                                | In-Situ量子化(ISQ)と連続バッチングを備えた、ゼロコンフィグで超最適化されたLLMエンジン。                    | 6.7k     |
| [m0at/rvllm](https://www.google.com/search?q=https://github.com/m0at/rvllm) | vLLMを代替する16MBの静的バイナリ。メモリ消費を1/3に抑えつつ8,300+トークン/秒を実現。                       | 79       |

#### 💻 CLI / Terminal Tools

ターミナルから離れる必要はありません。AIをシェルに直接統合し、複雑なコマンドの生成、ローカルドキュメントの検索、システム管理の自動化を行います。

| リポジトリ URL                                                        | 🚀 一行でわかる魅力的な説明                                                                                | ⭐ Stars |
| :-------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------- | :------- |
| [sigoden/aichat](https://github.com/sigoden/aichat)                   | Chat-REPL、ローカルRAG、シェルアシスタント機能を備えたパワーユーザー向けの究極のAll-in-One CLIツール。     | 9.6k     |
| [lasantosr/intelli-shell](https://github.com/lasantosr/intelli-shell) | ターミナル版IntelliSense。AIで拡張されたコマンドマネージャーが、あなたのタイポを学習して動的に修正を提案。 | 1.2k     |
| (https://github.com/Dicklesworthstone/pi\_agent\_rust)                | Electronの肥大化を避けるため、Rustでゼロから構築されたメモリ効率が高く爆速なターミナルエージェント。       | \>500    |

#### ⚡ Code Assistants & IDEs

Post-Electron時代の到来です。AIをGPUレンダリングパイプラインに直接組み込み、遅延ゼロのエージェント的コーディングを実現するRust製テキストエディタ。

| リポジトリ URL                                              | 🚀 一行でわかる魅力的な説明                                                                                       | ⭐ Stars |
| :---------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------- | :------- |
| [zed-industries/zed](https://github.com/zed-industries/zed) | 120fpsでレンダリングされる高性能マルチプレイヤーコードエディタ。ネイティブなエージェント編集とZeta2予測機能搭載。 | 78k      |

#### 🤖 Agents & Auto-coding Frameworks

厳格なメモリ安全の境界内で、推論、計画、およびコード実行を行う自律型ソフトウェアエンジニアを構築するためのライブラリとランタイム。

| リポジトリ URL                                                      | 🚀 一行でわかる魅力的な説明                                                                                                 | ⭐ Stars |
| :------------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------------------------------- | :------- |
| [zeroclaw-labs/zeroclaw](https://github.com/zeroclaw-labs/zeroclaw) | 5MBのRAMで動くマイクロエージェントランタイム。10ドルのエッジハードウェアで稼働する、OpenClawの99%軽量な代替品。             | 29k      |
| [0xPlaygrounds/rig](https://github.com/0xPlaygrounds/rig)           | 20以上のプロバイダに統一APIを提供し、スケーラブルなAIアプリケーションを構築するための極めてエルゴノミックなRustライブラリ。 | 6.7k     |
| [sobelio/llm-chain](https://github.com/sobelio/llm-chain)           | LLMプロンプトの連鎖、複数ステップのロジックの連携、Bash/Pythonの安全な実行を行うための高度なクレート。                      | 1.6k     |

**🤝 コントリビューション（PR歓迎）**
プルリクエストを熱烈に歓迎します！ 開発者体験（DX）とローカル実行を重視した素晴らしいRust製AIツールをご存知でしたら、ぜひPRを送信してください。最速かつ最も安全なAIエコシステムを一緒に構築しましょう。
