# 見積書作成アプリ (Quote Creator)

シンプルで使いやすい見積書作成専用のWindowsデスクトップアプリケーションです。直感的な操作で美しい見積書を素早く作成でき、EXEファイルとして配布されるため、誰でも簡単にインストール・実行できます。

## 🚀 特徴

- **簡単操作**: 直感的なユーザーインターフェースで誰でも簡単に見積書を作成
- **自動計算**: 税込み・税抜き価格、合計金額を自動で計算
- **PDF出力**: 作成した見積書をPDF形式で保存・印刷
- **データ保存**: 作成した見積書データを保存・再編集可能
- **EXE配布**: インストーラー不要、EXEファイルをダブルクリックで起動

## 🛠️ 技術スタック

### フロントエンド
- **Framework**: Next.js 14
- **Language**: TypeScript
- **UI Framework**: React 18
- **Styling**: Tailwind CSS
- **State Management**: React Context API
- **PDF生成**: jsPDF / React-PDF
- **Build Tool**: Next.js Build System
- **Deployment**: Electron Builder (EXE配布用)

## 📋 動作環境

### エンドユーザー（アプリ利用者）
- **最低**
    - **OS**: Windows 10 以上 (64bit)
    - **メモリ**: 4GB RAM 以上
    - **ストレージ**: 100MB の空き容量
    - **その他**: インターネット接続不要
- **推奨**
    - **OS**: Windows 10 以上 (64bit)
    - **メモリ**: 8GB RAM 以上
    - **ストレージ**: 100MB の空き容量
    - **その他**: インターネット接続不要

### 開発者
- **OS**: Windows / macOS / Linux
- **Node.js**: 18.0 以上
- **Next.js**: 14.0 以上
- **Git**: 最新版

## インストール・使用方法

### 開発者向けセットアップ

#### 1. リポジトリのクローン
```bash
git clone https://github.com/sakuraikanato/quote_request_app
cd quote_request_app
```

#### 2. 依存関係のインストール
```bash
npm install
```

#### 3. 開発環境での起動
```bash
# 開発モードで起動
npm run dev
```

## 使用方法

### 基本的な見積書作成フロー

#### 1. 新規見積書作成
- メイン画面の「新規見積書」ボタンをクリック
- 見積書番号が自動で生成されます

#### 2. 顧客情報の入力
- **新規顧客**: 会社名、担当者名、住所、電話番号等を入力
- **登録済み顧客**: ドロップダウンから選択して自動入力

#### 3. 見積内容の入力
- 「項目追加」ボタンで商品・サービスを追加
- 各項目に品名、数量、単価を入力
- 税込み・税抜きを選択（合計は自動計算）

#### 4. 見積書の調整
- 備考欄に特記事項を記入
- 有効期限を設定
- テンプレートを選択してデザイン変更

#### 5. 保存・出力
- **保存**: 作成中の見積書を保存（後で編集可能）
- **PDF出力**: 見積書をPDF形式で保存
- **印刷**: 直接プリンターに印刷

### 主な機能

#### 📋 見積書管理
- 作成済み見積書の一覧表示
- 検索・フィルター機能
- 見積書の複製・編集・削除

#### 👥 顧客管理
- 顧客情報の登録・編集
- よく使う顧客の管理
- 顧客別見積履歴

#### ⚙️ 設定機能
- 自社情報の登録
- ロゴ画像のアップロード
- デフォルト税率の設定
- 見積書テンプレートの選択

## 🧪 テスト

```bash
# 単体テストの実行
npm run test

# E2Eテストの実行
npm run test:e2e

# テストカバレッジの確認
npm run test:coverage
```

## 📝 開発

### 開発用コマンド

```bash
# Next.js開発サーバーの起動
npm run dev

# Next.jsアプリケーションのビルド
npm run build

# 本番環境での起動
npm start

# TypeScriptの型チェック
npm run type-check

# ESLintによるコード品質チェック
npm run lint

# Prettierによるコードフォーマット
npm run format

# テストの実行
npm run test
```

### ビルド・配布

```bash
# Next.jsアプリケーションのビルド
npm run build

# 静的エクスポート（必要に応じて）
npm run export

# ElectronでのWindows用EXEファイル作成
npm run electron:build:win

# 全プラットフォーム向けElectronビルド
npm run electron:build:all

# 配布用パッケージの作成
npm run dist
```

### プロジェクト構造

```
├── app/               # Next.js App Router
│   ├── components/    # UIコンポーネント
│   ├── api/           # API Routes
│   ├── quotes/        # 見積書関連ページ
│   ├── customers/     # 顧客管理ページ
│   └── settings/      # 設定ページ
├── components/        # 共有コンポーネント
├── hooks/             # カスタムフック
├── contexts/          # React Context状態管理
├── lib/               # ユーティリティ・設定
├── types/             # TypeScript型定義
├── public/            # 静的ファイル
└── electron/          # Electron関連ファイル（EXE配布用）
    ├── main.js        # Electronメインプロセス
    └── preload.js     # プリロードスクリプト
```

## 🤝 コントリビューション

1. このリポジトリをフォーク
2. フィーチャーブランチを作成 (`git checkout -b feature/amazing-feature`)
3. 変更をコミット (`git commit -m 'Add some amazing feature'`)
4. ブランチにプッシュ (`git push origin feature/amazing-feature`)
5. プルリクエストを作成

## 📄 ライセンス



## 👥 作者

### メインリーダー
- **Sakurai Kanato** - [@sakuraikanato](https://github.com/sakuraikanato)

### フロント/デザイナー
- **bannai enzo** - [@bannaienzo](https://github.com/bannaienzo)

## 🙏 謝辞

このプロジェクトの開発にあたり、以下のオープンソースプロジェクトを活用させていただきました：
- Electron
- React
- TypeScript
- Tailwind CSS
- SQLite
- jsPDF

## 📞 サポート

問題や質問がある場合は、以下の方法でお問い合わせください：
- GitHub Issues: [Issues ページ](https://github.com/sakuraikanato/quote_request_app/issues)
- Email: support@example.com

## 進行度

- [ ] 基本的な見積書作成機能
- [ ] excelエクスポート機能
- [ ] PDF出力機能
- [ ] 複数税率対応
- [ ] EXEファイル配布

## ⚠️ 注意事項

- このアプリケーションは現在開発段階です
- 重要なデータは定期的にバックアップを取ることをお勧めします
- 商用利用前に十分なテストを実施してください
- Windows Defender等のセキュリティソフトで警告が表示される場合がありますが、安全なアプリケーションです

---

**目標**: 見積書作成に特化したシンプルで使いやすいWindows デスクトップアプリケーション。  
**配布形式**: EXEファイルとして配布し、誰でも簡単にインストール・実行可能。

