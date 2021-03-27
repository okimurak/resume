# 職務経歴書

## 基本情報

| 項目   | 内容                                                                                                             |
| ------ | ---------------------------------------------------------------------------------------------------------------- |
| 名前   | 沖村　光一郎(Koichiro Okimura)                                                                                   |
| Email  | [okimurak0901@gmail.com](mailto:okimurak0901@gmail.com)                                                          |
| Blog   | [https://okimurak.github.io/](https://okimurak.github.io/), Qiita : [@okky_eng](https://qiita.com/okky_eng)      |
| Github | [okimurak](https://github.com/okimurak)                                                                          |
| SNS    | Twitter : [@okky_eng](https://twitter.com/okky_eng), LinkedIn : [okimurak](https://www.linkedin.com/in/okimurak) |

## 職務経歴

### 2019/04 - 現在 : インターネット広告系企業

- 職位 : Web エンジニア

#### SSP のクラウド移行

SSP とは、媒体の広告枠販売や広告収益の最大化を支援するためのツールです。オンプレミスで構築されたシステムをクラウドへ移行する必要があり、移行プロジェクトが発足しました。クラウドインフラへの面白さと魅力を実感し、より深くクラウドインフラと関わるために AWS へ移行するプロジェクトを参画させていただいています。移行はシステム構成をクラウドネイティブに再設計する形で進めています。

##### 役割

- クラウド移行後の技術選定・設計・構築
- CI/CD パイプラインの構築
- プロジェクトのドキュメント整備
- スケジュール・タスク管理

##### 環境

- バックエンド : Java 8, Python3.7
- フロントエンド : JavaScript
- インフラ
  - オンプレミス : CentOS(VM) + MySQL(VM), Mackerel
  - クラウド : ECS, EFS, Aurora, DynamoDB, Lambda, Stepfunctions, S3, API Gateway, Route53, SES, CloudWatch, EventBridge, SSM Parameter Store, Fastly, datadog
- 開発規模は 14 名

##### 実績・ポイント

- 業務アプリケーションはコンテナ化して ECS へ移行しています。
- DB 接続が不要な Web アプリケーションは API Gateway + Lambda、バッチアプリケーションは Lambda に移行しています。
- 移行先のインフラ環境は再現性を持たせるために Terraform や serverless framework を使ってコード化を行い、設定の見える化をしました。
- プロジェクトの開発プロセスを分析して、Github + CircleCI を用いた CI/CD パイプラインを作成し、GitOps のビルド・デプロイフローを構築しました。

#### SSP の商材管理システムの開発・運用

PMP(Private Marcket Place) で用いる商材情報を管理するためのシステムの追加開発・保守を担当しました。

##### 役割

- 要件定義、設計、開発、テスト、レビュー、リリース
- スケジュール・タスク管理・オフショアとの調整

##### 環境

- バックエンド : PHP 7.0(FuelPHP)
- フロントエンド : JavaScript(jQuery, Backbone.js), Shell
- インフラ : EC2 + CLB, RDS(MySQL), Lambda, SES, CloudWatch, Mackerel
- 開発規模は 3 名

##### 実績・ポイント

- 追加機能開発に要件定義からリリースまで一気通貫で担当しました。
- オフショア（ベトナム）を利用し、英語でコミュニケーションを取っていました。
- 手動手順だったデプロイを Github + CircleCI + CodeDeploy を用いた CI/CD パイプラインを作成し、GitOps のビルド・デプロイフローを構築しました。
- アプリケーションログを監視しておらず、クリティカルなエラーに気づけなかったため Fluentd + CloudWatch Logs + Lambda + Slack を用いたアプリケーションログ監視を設計・構築しました。

### 2015/04 - 2019/03: メーカー系 SIer

- 職務: システムエンジニア

#### 担当プロジェクトと業務

#### 2016/04 - 2019/03 : 官公庁向けプロジェクトのリプレイス

システムエンジニアとして通信指令システムのリプレイスプロジェクトに参画し、外部設計からリリースまでを担当しました。画面設計、テスト、リリースについては全システムを担当しました。また、詳細設計、実装については他システムで発生した障害情報を収集する監視機能や、リモートで各サーバや端末を操作する運用管理機能を持った運用監視システムのリーダーを担当しました。

##### 役割

- システム全体の画面設計
- 運用監視システムリーダー
  - 詳細設計、 開発、テスト、レビュー、リリース
  - スケジュール・タスク管理

##### 環境

- バックエンド : Java 8
- フロントエンド : Java FX, バッチは Shell, Python3.2
- インフラ
  - サーバ : RHEL7, Windows Server 2016
  - クライアント : Windows 10 Enterprise
  - ミドルウェア は Oracle 12c, WebLogic
- 開発規模は 100 名 (チーム規模 3 名, 10 チーム)


##### 実績・ポイント

- お客様との要件齟齬を防ぐため、プロトタイプを開発しながら要件・機能確認を繰り返し行う形で進めました。
  - Java FX による UI のモックを作成して画面設計を行い、お客様と調整を行いました。またその後に、内部ロジックを追加してお客様にデモを行いながら機能確認と追加改修を行いました。
- 開発業務の効率化のため、ソースコードについては Subversion から Git + Jenkins + Coverity による継続的デプロイ環境の提案、導入、構築をしました。
- 運用監視システムのリーダーとしてメンバーの工数管理をしつつ、開発実装も担当しました。
- プロジェクトの新人オンボーディング資料が無かったため 1 ヶ月程度掛かっていましたが、独自に新人教育用の資料を作成することで、2 週間程度に抑えることができました。資料は、サンプルコードや実装例を含めたプログラミング課題（電卓作成）を作成しました。

#### 2015/07 - 2016/03 : 官公庁向けプロジェクトのサーバ更改

通信指令システムのサーバ更改において、認証・ドメインサーバの構築を担当しました。

##### 役割

- サーバ設定における詳細設計、構築、テスト、リリース

##### 実績・ポイント

- サーバ構築について、OS セットアップ(Windows Server 2012R2)、ネットワーク設定、ミドルウェアインストール、Active Directory 設定、業務アプリケーション設定、サーバリリースを担当しました。

## スキル

### 言語

| 言語       | 経験                                                                                            |
| ---------- | ----------------------------------------------------------------------------------------------- |
| Python3    | バッチ開発で 2 年経験                                                                           |
| Java       | フロントエンド(Java FX)、バックエンド開発のために 5 年経験                                      |
| PHP        | バックエンドで 1 年経験。FW は FuelPHP を利用                                                   |
| JavaScript | フロントエンド開発、AWS Lambda のバッチ開発のために 計 1 年ほど経験。jQuery, Backbone.js を利用 |
| Shell      | バッチ開発のために 5 年経験                                                                     |

### インフラ

- OS ... Windows, Linux (CentOS, RHEL7), Mac OS
- ツール ... Docker, Terraform, Fluentd, Mackerel, datadog

### データベース

6 年経験

- Oracle (11, 12c), MySQL(5.6)

### AWS

2 年経験

- EC2, ECS(Fargate), ECR, S3, Lambda, Stepfunctions, CloudWatch, SNS, SES, EventBridge, Route53, ALB, API Gateway, CodeDeploy, DynamoDB, RDS, SSM Parameter Store, IAM

### その他ツール

- Github, Gitlab, CircleCI, Jenkins, serverless framework, Coverity, JIRA, Redmine

## 自分の強み

- 面白そうと思ったことに対して、すぐに実践
  - メモ・ドキュメントを残す
- 定形作業の自動化
- 未経験の技術分野への興味

## 興味があるもの

- AWS を用いたシステム構築
- コンテナ
- Kurbernetes を使った実務でのインフラ構築
- CI/CD パイプラインの構築
- マイクロサービスの開発・運用
- イベントドリブンのアーキテクチャ

## 業務外活動

### 取得資格

| 名前                                              | 取得年月日 |
| ------------------------------------------------- | ---------- |
| 応用情報技術者                                    | 2010/06    |
| マイクロソフト認定プロフェッショナル 70-410       | 2015/08    |
| Oracle Master Bronze(11b)                         | 2015/10    |
| 情報処理安全確保支援士                            | 2016/07    |
| AWS 認定ソリューションアーキテクト - アソシエイト | 2020/06    |

## 参考

職務経歴書を作成するにあたり、参考にさせていただいた資料。

- [職務経歴書 · kwappa on the net](https://kwappa.github.io/logs/resume/)
- [okohs/Curriculum-Vitae-template](https://github.com/okohs/Curriculum-Vitae-template)
