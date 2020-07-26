# 職務経歴書

## 基本情報

| 項目     | 内容                                                       |
| -------- | ---------------------------------------------------------- |
| 名前     | 沖村　光一郎(Koichiro Okimura)                             |
| Blog     | [https://okimurak.github.io/](https://okimurak.github.io/) |
| Twitter  | [@okky_eng](https://twitter.com/okky_eng)                  |
| Qiita    | [@okky_eng](https://qiita.com/okky_eng)                    |
| LinkedIn | [Koichiro Okimura](www.linkedin.com/in/okimurak)           |

## スキル

### 言語

- Python (v3 系)
  - バッチ開発で 2 年経験
- Java
  - フロントエンド(Java FX)、バックエンド開発のために 5 年経験
- PHP
  - バックエンドで 1 年経験。FW は FuelPHP を利用
- JavaScript
  　- フロントエンド開発、AWS Lambda のバッチ開発のために 計 1 年ほど経験。jQuery, Backbone.js を利用
- VB
  - SIer 時代に、業務改善のために半年ほど経験
- Shell
  - バッチ開発のために 5 年経験

### インフラ

- Docker
- Terraform
- Fluentd
- Mackerel
- datadog

#### データベース

- Oracle (11, 12c)
- MySQL(5.7)

#### AWS

以下のマネージドサービスを実務にて経験、Terraform などを用いてコード化

- EC2
- ECS(Fargate)
- ECR
- S3
- Lambda
  - Python3.7, JavaScript で実装
- CloudWatch
- SNS
- SES
- Route 53
- CodeDeploy
- RDS
- AWS Simple System Manager
  - パラメータストアを主に
- IAM

### その他

- Github, Gitlab
- CircleCI
- serverlessframework
  - AWS Lambda のデプロイに利用
- Coverity
  - SIer 時代に、Java の静的コード解析

## 自分の強み

- 面白そうと思ったことに対して、すぐに実践
  - メモ・ドキュメントを残す
- カイゼン活動。無理・強要はしない
- やったことがないもの（技術によらず）への興味

## 興味があるもの

- AWS を用いたシステム構築
- Kurbernetes を使った実務でのインフラ構築
- CI/CD
- マイクロサービスの開発・運用
- サーバレスアーキテクチャ

## 職務経歴

### 2019/04 - 現在 : インターネット広告系企業

#### 担当プロジェクトと業務

- SSP の商材管理システムの開発・運用

  - アプリケーションのバックエンドは PHP7.0(FuelPHP), フロントエンドは JavaScript(jQuery, Backbone.js), Shell を使用
  - インフラは AWS EC2 + CLB, RDS(MySQL), SES
  - 追加機能開発
    - 要件定義
    - ユースケース検討・定義
    - UI 設計
    - 基本設計・詳細設計
    - フロントエンド開発
    - データベース設計
    - バックエンド開発
    - 実装
    - オフショアとの開発調整(英語)
    - テストケース作成とテスト
  - CI/CD の導入
    - 手動シェル実行リリースから Github + CircleCI + Slack を用いた自動ビルド・デプロイ
    - 動かないテストコードの改修
  - 監視設計
    - アラートなしから Fluentd + CloudWatchLogs + Lambda + Slack を用いたアラート通知

- SSP の開発・運用
  - バックエンドは Java8, Python3.7, フロントエンドは JavaScript を使用
  - インフラは CentOS(VM) + MySQL(VM), AWS(S3, SES, Lambda)
  - AWS アカウントのスイッチロール対応
  - TLS 1.2 用リバースプロキシ構築
  - オンプレミスから AWS への移行
    - バッチの移行
      - 現行仕様調査
      - 技術選定
      - サービスアーキテクチャ検討
      - インフラストラクチャ設計
      - インフラストラクチャ構築
        - Terraform のコード化
      - CI/CD 設計
        - Github + CircleCI + Slack を用いた自動ビルド・デプロイ
      - 監視設計
        - CloudWatchLogs + Lambda + Slack を用いたアラート通知
        - datadog を用いたメトリクス取得とメトリクスダッシュボード作成
    - 既存 AWS リソースのコード化

### 2015/04 - 2019/03: メーカー系 SIer

職務: システムエンジニア

#### 担当プロジェクトと業務

- 官公庁向け大規模プロジェクトの開発・運用
  - 5 ヶ年のプロジェクト
  - アプリケーションは Java8, フロントエンドは Java FX を使用
  - バッチは Shell, Python3.2 を使用
  - インフラはサーバが RUEL, Windows Server 2012,2016, クライアントが Windows 10 Enterprise
  - 201507 - 201603
    - 基本設計
    - 要件定義
    - ユースケース検討・定義
    - 認証・ドメインサーバ (Window Server 2012 R2)構築
      - OS セットアップ、ネットワーク設定、ミドルウェア、Actice Directory 設定、業務アプリケーション設定
  - 201604 - 201703
    - PJ ルームの引っ越し
      - レイアウト
      - ネットワーク 設計
    - 詳細設計
    - UI 設計
      - 画面モックの作成・仕様調整 (Java8 + JavaFX)
    - Git + Jenkins + Coverity による継続的デプロイ環境の導入提案、構築
      - Subversion からの脱却
  - 201704 - 201803
    - 監視アプリケーション
      - フロントエンド、バックエンド開発 (Java8 + JavaFX)
      - データベース設計
      - テスト設計（テストケース、単体テスト、結合テスト）
    - 監視アプリケーションの工数・進捗管理
    - 開発拠点間 VPN 構築
  - 201804 - 201903
    - インフラ構築
    - デプロイ自動化バッチ構築
    - リリース前システムテスト
    - リリース

## 業務外活動

### 取得資格

| 名前                                        | 取得年月日 |
| ------------------------------------------- | ---------- |
| 応用情報技術者                              | 2010/06    |
| マイクロソフト認定プロフェッショナル 70-410 | 2015/08    |
| Oracle Master Bronze(11b)                   | 2015/10    |
| 情報処理安全確保支援士                      | 2016/07    |
| AWS 認定ソリューションアーキテクト          | 2020/06    |

### イベントへの参加

- JAWS-UG
- Terraform Meetup
- Infra Study Meetup
- CircleCI Meetup

## 参考

職務経歴書を作成するにあたり、参考にさせていただいた資料

- [職務経歴書 · kwappa on the net](https://kwappa.github.io/logs/resume/)
- [okohs/Curriculum-Vitae-template](https://github.com/okohs/Curriculum-Vitae-template)
