# サービス概要書

### どんなアプリケーションか
YouTube動画に特化した料理レシピ保存サービス

### 開発動機
YouTubeで作り方を覚えても具材や調味料、分量などを料理のたびに動画を見返して確認するのが面倒なため。  
動画と一緒に簡単にレシピ登録できるサービスがほしいと思った。

### 特徴
- YouTube動画を各レシピページに埋め込み可能
- 外部検索リンク（「新しいタブでYouTubeを開く」ボタン）の設置でYouTubeアクセス & 動画URL取得を簡便に
- 具材、調味料、分量などを簡単に登録できる
- シンプルでわかりやすいUI & SPAによる優れたUX

### ターゲット
- YouTubeで料理レシピをリサーチする層
- 主に20 ~ 50代男女で幅広く分布。ボリューム層は20 ~ 30代女性。

### 競合と差別化ポイント
- クラシル、DELISH KITCHEN、クックパッドなどのレシピサービス
- 料理レシピ本
- 食品メーカーなどのWebサイト

上記競合群は活字ベースで静的なレシピ閲覧に特化している（YouTubeとの親和性はない）。  
また、分量などのカスタム管理は不可。

### 主な使用技術
- バックエンド
  - 言語: Ruby 3.3.7 / Ruby on Rails 7.2.2.1
  - テスト・開発支援: RSpec / RuboCop
  - 認証: Devise / Devise Token Auth
  - ページネーション: Pagy
- フロントエンド
  - 言語: TypeScript 5.8.2 / React 19.0.0 / Next.js 15.1.6
  - デザイン: Tailwind CSS / Shadcn UI
  - テスト・開発支援: Vitest / React Testing Library / MSW / Cypress / ESLint / Prettier
- インフラ
  - AWS: Route53 / ALB / ECS Fargate / ECR / RDS PostgreSQL / ACM / CloudWatch etc.
  - Nginx / Vercel
- CI/CD: GitHub Actions
- コンテナ技術: Docker / Docker Compose / Dev Containers
- 外部API: YouTube Data API

### 参考データ
- [マルハニチロ「料理レシピに関する調査 2020」](https://www.maruha-nichiro.co.jp/corporate/news_center/news_topics/20200818_research_recipe2020_1.pdf)