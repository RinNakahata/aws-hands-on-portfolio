 # AWS Hands-on Portfolio

このリポジトリは、教本 **「みんなのAWS」(技術評論社)** のハンズオンに基づいて構築した3つの環境と、その際に出力された **CloudTrail / Config のログ** を記録したものです。  
構築作業は、教本の手順を忠実に実施し、環境ごとに開始時間・終了時間をレポート化しています。  



##  リポジトリ構成
```
aws-hands-on-portfolio/
├─ env1/ # 第2章　AWSで作るWebサービス
│ ├─ logs/ # CloudTrail/Configログを日付ごとに保存
│ └─ report.md # 作業時間や概要を記録
├─ env2/ # 第3章　サーバーレスプラットフォームで作る モバイル向けアプリケーション
│ ├─ logs/
│ └─ report.md
├─ env3/ # 第4章　AWSで作るデータの収集・可視化基盤
│ ├─ logs/
│ └─ report.md
└─ README.md # 本ドキュメント
```




##  環境概要

### 第2章　AWSで作るWebサービス
- **概要**: VPC内にPHPアプリと管理画面（phpMyAdmin）をデプロイし、RDS(MySQL)と連携
- **構成**: VPC, ECS(Fargate), RDS, ALB, CodeCommit, CodePipeline


### 第3章　サーバーレスプラットフォームで作る モバイル向けアプリケーション
- **概要**: API + フロントエンドを組み合わせたモバイル対応アプリの提供
- **構成**: API Gateway, Lambda(Go), DynamoDB, CloudFront, S3, Vue.js(PWA), AWS CDK


### 第4章　AWSで作るデータの収集・可視化基盤
- **概要**: 仮想ETCゲートからのデータを収集・分析・可視化
- **構成**: IoT Core, Kinesis Firehose, Lambda(Python), DynamoDB, S3, Glue, Athena, Redshift, QuickSight



##  ログとレポート
- 各環境の作業ログ（CloudTrail / Config）は `logs/` 以下に日付フォルダごとに保存  
- 各環境の作業レポート（所要時間やポイント）は `report.md` に記録  

---

##  License
This repository is licensed under the MIT License.
