# 2026年のOSS活動まとめ

5分発表の素材。集計は2026年11月24日時点。

## 1. rfmt

- Rust製のRubyフォーマッタ。2026年に `2.0.0.beta1` を公開。<https://github.com/sorafujitani/rfmt/releases/tag/v2.0.0.beta1>
- **RubyGemsで累計約3.8万ダウンロード**（37,629件）。<https://rubygems.org/api/v1/gems/rfmt.json>
- **Short Ruby Newsletter #165** の新着gem欄で紹介（1月26日）。<https://newsletter.shortruby.com/p/edition-165>

## 2. ccsession

- AIコーディングエージェントの過去の会話を探し、元の作業場所で再開できるCLI。2026年5月に公開。<https://github.com/sorafujitani/ccsession>
- **GitHub Releasesの配布バイナリは累計約8,400ダウンロード**（8,443件）。<https://api.github.com/repos/sorafujitani/ccsession/releases?per_page=100>
- 7月6日にeiji.pageで紹介。<https://eiji.page/blog/ccsession-intro/>

## 3. 自作OSSの傾向

- **2026年に、ccsession以外にも32のOSSリポジトリを作成。** 例は `skills`、`panopticon`、`rt`。<https://github.com/sorafujitani?tab=repositories>
- 集計はGitHubの本人アカウントで、2026年作成・公開・非fork・ライセンスがMITまたはApache-2.0と確認できたもの。計33件からccsessionを除いた。2025年に始めたrfmtは年次集計の範囲外。<https://api.github.com/users/sorafujitani/repos?per_page=100&sort=created&direction=desc&page=1>
- GitHubの主言語で判定なしの8件をRustに加えて集計。Rust 13件（40.6%）、TypeScript 8件（25%）、Go 6件（18.8%）、その他5件（15.6%）。その他はHTML、JavaScript、MoonBit、Python、Swiftが各1件。
- 本人所有の公開・非forkの161リポジトリで、2026年1月1日〜11月24日（日本時間）に**164件のPRがマージ**され、**コミットは1,385件**。ライセンスの有無を問わず、PRはマージ日で、コミットは各デフォルトブランチの履歴で集計した。<https://api.github.com/users/sorafujitani/repos?per_page=100> · <https://docs.github.com/en/graphql/reference/commits>

## 4. 他のOSSへの貢献

外部リポジトリに **公開PR 29件、うち19件がマージ**。共同開発のPRも含む。<https://github.com/search?q=author%3Asorafujitani+is%3Apr+is%3Apublic+created%3A2026-01-01..2026-11-24+-user%3Asorafujitani&type=pullrequests>

- **Oxc** — OxlintにNode.js向けのlintルールを2つ追加。<https://github.com/oxc-project/oxc/pull/23539> · <https://github.com/oxc-project/oxc/pull/23589>
- **Hono** — 言語判定を改善。 `ja-JP` から `ja` にフォールバックできるようにした。<https://github.com/honojs/hono/pull/4717>
- **Ruby** — rfmtの配布で直面したビルドの問題をRuby Prismで修正。RuboCopの自動修正も改善。<https://github.com/ruby/prism/pull/4179> · <https://github.com/rubocop/rubocop/pull/15101>
- **その他** — Mago、Yamada UI、ccgateなど。<https://sorafujitani.me/pulls/>
