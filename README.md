# 出荷指示管理システム

GitHub: https://github.com/TSUNOSHIN/Shipment-management-system

物流現場（花王ロジスティクス）での実務経験をもとに、使いにくかった既存システムの課題を解決するために開発した出荷指示管理アプリです。

## アプリ概要

拠点ごとにログインし、出荷指示（梱出荷・バラ出荷）の登録・編集・削除、店舗マスタ管理ができるBtoB向け業務支援アプリです。郵便番号APIによる住所自動入力にも対応しています。

## サイトURL

（Vercelデプロイ後にここへURLを記載）

## 使用技術

- フロントエンド：Next.js（App Router）、React、TailwindCSS
- バックエンド：Next.js API Routes
- データベース：Supabase（PostgreSQL）
- 認証：Supabase Auth
- 外部API：郵便番号API（zipcloud）
- デプロイ：Vercel
- バージョン管理：Git、GitHub
- 設計ツール：Figma、draw.io

## 設計ドキュメント

[要件定義・基本設計・詳細設計の一覧_Googleスプレッドシート]
(https://docs.google.com/spreadsheets/d/1_92QzNYiftUf_nFWfuMIKza6hmokr3Vur-28xKohQ0Y/edit?gid=1593576189#gid=1593576189)

ワイヤーフレーム、ER図、ワークフロー図の画像はdocsディレクトリに格納しています。（[こちらからアクセス](docsフォルダのURL)）

## 機能一覧

- ログイン・認証機能（Supabase Auth、拠点アカウント制）
- 出荷指示の新規作成・編集・削除
- 出荷指示一覧表示・種別（梱／バラ）フィルタリング
- 出荷ステータス管理（準備中・指示済み・完了）
- 店舗マスタ管理（登録・編集・削除）
- 郵便番号APIによる住所自動入力
- 出荷時間に基づく優先順位の自動表示

## 備考

- 活用した生成AIとその用途
  - Claude：要件定義の壁打ち、DB設計・ER図のレビュー、機能一覧の整理、ワークフロー図の作成相談
