# 営業管理ダッシュボード

営業活動を効率化するためのWebベースの管理システムです。

## 概要

このシステムは営業チームのパフォーマンス管理と顧客管理を支援するダッシュボードアプリケーションです。

### 主な機能

- **ダッシュボード機能** (`index.html`)
  - 売上データの可視化
  - チーム別パフォーマンス表示
  - 目標達成率の監視
  - リアルタイム統計情報

- **リード管理機能** (`leads-management.html`)
  - 顧客リードの登録・編集
  - ステータス管理
  - 連絡履歴の記録
  - フォローアップ管理

### ユーザーロール

システムでは以下のユーザーロールをサポートしています：

| ユーザーID | 役割 | チーム |
|-----------|------|--------|
| admin | 管理者 | - |
| sales1 | 田中太郎 | Aチーム |
| sales2 | 佐藤花子 | Bチーム |
| manager1 | 山田次郎 | Aチーム |

## 技術スタック

- **フロントエンド**
  - HTML5
  - CSS3
  - JavaScript (Vanilla)
  - Tailwind CSS
  - Font Awesome
  - Chart.js
  
- **フォント**
  - Google Fonts (Inter)

## セットアップ

1. このリポジトリをクローンします：
   ```bash
   git clone <repository-url>
   cd sales-dashboard
   ```

2. Webサーバーでファイルを配信します：
   ```bash
   # 例: Python HTTP サーバー
   python -m http.server 8000
   
   # 例: Node.js HTTP サーバー
   npx http-server
   ```

3. ブラウザで `http://localhost:8000` にアクセスします。

## 使用方法

### ログイン

1. `index.html` にアクセス
2. ユーザー選択ドロップダウンから任意のユーザーを選択
3. 「ログイン」ボタンをクリック

※ パスワードは不要です（デモ用）

### ナビゲーション

- **ダッシュボード**: 売上データと統計情報の表示
- **リード管理**: 顧客情報の管理と編集

## ファイル構成

```
├── index.html              # メインダッシュボード
├── leads-management.html   # リード管理画面
└── README.md              # プロジェクト説明書
```

## 開発者向け情報

### 使用されている外部リソース

- [Tailwind CSS](https://tailwindcss.com/) - CSSフレームワーク
- [Chart.js](https://www.chartjs.org/) - グラフ描画ライブラリ
- [Font Awesome](https://fontawesome.com/) - アイコンフォント
- [Google Fonts](https://fonts.google.com/) - Webフォント

### カスタマイズ

- スタイルのカスタマイズは各HTMLファイル内の `<style>` セクションで行えます
- チャートの設定は `Chart.js` の設定オブジェクトを編集してください
- ユーザーデータは JavaScript の配列オブジェクトとして管理されています

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。

## サポート

質問や問題がある場合は、GitHubのIssuesでお知らせください。