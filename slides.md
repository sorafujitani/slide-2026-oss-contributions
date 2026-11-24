---
theme: default
colorSchema: light
background: false
class: text-center
drawings:
  persist: false
transition: slide-left
title: 2026年のOSS活動まとめ
fonts:
  provider: none
  sans: 'Noto Sans JP'
  mono: ui-monospace
---

<CoverSlide
  title="2026年 OSS contribution まとめ"
  author="fujitani sora"
/>

<!--
目安 20秒

今年作ったものと、ほかのOSSで取り組んだことを紹介します。
数字は2026年11月24日時点です。
-->

---

<ProfileSlide
  name="fujitani sora"
  x="sorafujitani"
  github="sorafujitani"
  website="https://sorafujitani.me/"
  avatar="https://raw.githubusercontent.com/fs0414/imgs/main/fs0414_dot_image.png"
  :items="[
    { icon: 'calendar', label: '2001 (25)' },
  ]"
/>

---

# rfmt

Rustの高速なRuby Code Formatter

- https://github.com/sorafujitani/rfmt
- RubyGemsで累計37,629ダウンロード
- [Short Ruby Newsletter #165](https://newsletter.shortruby.com/p/edition-165) で紹介
- [2.0.0.beta1](https://github.com/sorafujitani/rfmt/releases/tag/v2.0.0.beta1) を最新で公開

<!--
目安 1分

Rubyのコードを一定のスタイルに整えるツールです。
今年は2.0のベータ版を公開しました。1月にはShort Ruby Newsletterの新着gem欄で紹介され、RubyGemsの累計ダウンロードは約3.8万件になりました。

https://rubygems.org/api/v1/gems/rfmt.json
https://newsletter.shortruby.com/p/edition-165
-->

---

# ccsession

AIエージェントの過去の会話を探して再開するCLI

- https://github.com/sorafujitani/ccsession
- GitHub Releasesで配布バイナリが累計8,443ダウンロード
- Articles
  - [Claude Codeのセッション履歴をfzf検索 & previewする技術（ccsession）](https://zenn.dev/soramarjr/articles/4eb891ab20498e)
  - [CLI派歓喜！Claude Code履歴検索のccsessionが便利](https://eiji.page/blog/ccsession-intro/)

<!--
目安 1分10秒

前にどのプロジェクトで話したか忘れても、会話を横断して検索し、選んだセッションを元の作業場所から再開できます。
5月に公開しました。Claude Code向けに作り始めて、CodexやOpenCodeなどでも使えるようにしました。

https://github.com/sorafujitani/ccsession
https://eiji.page/blog/ccsession-intro/
https://api.github.com/repos/sorafujitani/ccsession/releases?per_page=100
-->

---

# その他に作ったOSS

2026年に、ccsession以外にも32件のOSSリポジトリを作成

[skills](https://github.com/sorafujitani/skills)、[panopticon](https://github.com/sorafujitani/panopticon)、[rt](https://github.com/sorafujitani/rt) など

<!--
目安 30秒

ほかにも普段の開発で使うツールを作りました。たとえばpanopticonは、エージェントが実行したツールや、エラーが起きた箇所を振り返るためのものです。
本人の公開・非forkリポジトリで、MITまたはApache-2.0のものを集計しています。

https://api.github.com/users/sorafujitani/repos?per_page=100&sort=created&direction=desc&page=1
-->

---

# 他のOSSへの貢献

公開PRは29件、うち19件がマージ（共同開発を含む）

- **Oxc**　OxlintにNode.js向けのルールを実装したり
- **Hono**　言語判定で ja-JP から ja を選べるようにしたりテストを最新化したり
- **Ruby**　Ruby PrismのBuildとRuboCopの自動修正を改善したり
- **その他**　Mago、Yamada UI、ccgateなど

[PR・Issue一覧](https://sorafujitani.me/pulls/)

<!--
目安 2分

OxcではOxlintにNode.js向けのルールを追加しました。Honoでは、たとえば日本向けの言語コードを受け取ったときに、日本語の設定を使えるようにしました。
Ruby Prismはrfmtでも使っているライブラリです。rfmtを別の環境向けにビルドする際に見つけた問題を報告し、修正PRを出しました。

Oxc
https://github.com/oxc-project/oxc/pull/23539
https://github.com/oxc-project/oxc/pull/23589

Hono
https://github.com/honojs/hono/pull/4717

Ruby
https://github.com/ruby/prism/pull/4179
https://github.com/rubocop/rubocop/pull/15101

PR・Issue一覧
https://sorafujitani.me/pulls/
-->
