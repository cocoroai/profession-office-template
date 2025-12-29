# 士業事務所ホームページテンプレート

行政書士・税理士・司法書士などの士業事務所向けのレスポンシブWebサイトテンプレートです。

## デモサイト

[GitHub Pagesでデモを見る](https://cocoroai.github.io/profession-office-template/)

## 特徴

- 📱 **モバイルファースト設計** - スマートフォンでも見やすく操作しやすい
- 🎨 **プロフェッショナルなデザイン** - 青と白を基調とした信頼感のあるデザイン
- 📅 **予約システム** - カレンダーベースの予約機能（第3希望まで選択可能）
- 💼 **充実のページ構成** - TOP、業務内容、料金案内、プロフィール、FAQ、お問い合わせ、予約
- 🚀 **軽量・高速** - JavaScript最小限でパフォーマンス重視
- 🔧 **カスタマイズ容易** - シンプルなHTML/CSSで構成

## ページ構成

1. **TOPページ** (`index.html`)
   - ヒーローセクション
   - 事務所紹介
   - 業務内容概要（展開可能なカード）
   - お客様の声

2. **業務内容** (`services.html`)
   - 法人設立・会社設立
   - 許認可申請
   - 税務相談・申告
   - 相続・遺言
   - 不動産登記
   - 契約書作成

3. **料金案内** (`pricing.html`)
   - 各サービスの基本料金
   - オプション料金
   - 顧問契約プラン

4. **代表プロフィール** (`profile.html`)
   - 代表者紹介
   - 経歴・実績
   - 保有資格

5. **よくある質問** (`faq.html`)
   - アコーディオン形式のFAQ

6. **お問い合わせ** (`contact.html`)
   - お問い合わせフォーム
   - アクセス情報
   - Google Maps連携

7. **予約ページ** (`reservation.html`)
   - カレンダー形式の日付選択
   - 時間帯選択
   - 第3希望まで選択可能

## 使い方

### 1. ダウンロード

```bash
git clone https://github.com/cocoroai/profession-office-template.git
cd profession-office-template
```

### 2. カスタマイズ

#### 事務所情報の変更
すべてのHTMLファイルで以下の情報を変更してください：
- 事務所名
- 住所
- 電話番号
- メールアドレス
- 営業時間

#### 画像の差し替え
`images/README.md` を参照して、必要な画像を配置してください：
- `hero-background.jpg` - ヒーロー背景画像
- `office-exterior.jpg` - 事務所外観
- `profile-photo.jpg` - 代表者写真
- `access-map.jpg` - アクセスマップ

#### 色の変更
`style.css` で以下の色を変更できます：
```css
/* メインカラー（青） */
color: #1e3a8a;
background-color: #1e3a8a;
```

### 3. 公開

#### 方法1: GitHub Pages（推奨）
1. GitHubにリポジトリを作成
2. Settings → Pages → Source を "Deploy from a branch" に設定
3. Branch を "main" に設定
4. 数分後に `https://[username].github.io/[repository-name]/` でアクセス可能

#### 方法2: 通常のWebサーバー
すべてのファイルをWebサーバーにアップロードしてください。

## 技術仕様

- **HTML5** - セマンティックなマークアップ
- **CSS3** - Flexbox/Grid によるレイアウト
- **JavaScript** - 最小限の使用（メニュー、予約システムのみ）
- **レスポンシブ** - モバイル/タブレット/デスクトップ対応
- **パフォーマンス** - 画像の遅延読み込み、フォールバック機能

## ブラウザ対応

- Chrome（最新版）
- Firefox（最新版）
- Safari（最新版）
- Edge（最新版）
- iOS Safari（iOS 14以上）
- Android Chrome（最新版）

## カスタマイズのヒント

### サービスカードの追加
`index.html` や `services.html` で以下の構造をコピーして追加：
```html
<div class="service-card" onclick="toggleServiceDetail(this)">
    <div class="service-card-header">
        <h3>新しいサービス</h3>
        <span class="service-card-icon">▼</span>
    </div>
    <p>サービスの説明</p>
    <p class="highlight">特徴やポイント</p>
    <div class="service-card-detail">
        <h4>詳細サービス内容</h4>
        <ul>
            <li>詳細項目1</li>
            <li>詳細項目2</li>
        </ul>
    </div>
</div>
```

### 新しいページの追加
1. 既存のHTMLファイルをコピー
2. ヘッダーとフッターはそのまま利用
3. メインコンテンツ部分を編集
4. ナビゲーションメニューにリンクを追加

## ライセンス

MIT License - 自由に使用、改変、再配布可能です。

## 作者

Created with Claude Code

## 貢献

プルリクエストやイシューは歓迎します。

## 更新履歴

- 2024-07-23 - 初版リリース
  - 基本的なページ構成
  - レスポンシブデザイン
  - 予約システム実装