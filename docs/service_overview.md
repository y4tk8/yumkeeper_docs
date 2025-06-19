# サービス概要書

### どんなアプリケーションか
YouTube動画に特化した料理レシピ保存サービス

### 開発動機
YouTubeで作り方を覚えても具材や調味料、分量などを料理のたびに動画を見返して確認するのが面倒なため。  
動画と一緒に簡単にレシピ登録できるサービスがほしいと思った。

### 特徴
- YouTube動画を各レシピページに埋め込み可能
- 外部検索リンク（「新しいタブでYouTubeを開く」ボタン）の設置でYouTubeアクセス & 動画URL取得を簡単に
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
- バックエンド: Ruby on Rails / RSpec
- フロントエンド: TypeScript / React / Next.js / Tailwind CSS / Vitest / React Testing Library / MSW / Cypress
- インフラ: AWS(Route53 / ALB / ECS on Fargate / ECR / RDS / ACM etc) / Nginx / Vercel
- CI/CD: GitHub Actions
- 環境構築: Docker / Docker Compose / Dev Containers
- 外部API: YouTube Data API

### 参考データ
- [マルハニチロ「料理レシピに関する調査 2020」](https://www.maruha-nichiro.co.jp/corporate/news_center/news_topics/20200818_research_recipe2020_1.pdf)