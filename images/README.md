# 画像ファイルの配置について

このフォルダに以下の画像ファイルを配置してください：

## 必要な画像ファイル

### ヒーロー背景画像（NEW!）
- **ファイル名**: `hero-background.jpg` または `hero-background.png`
- **推奨サイズ**: 1920×1080px以上（横長）
- **用途**: トップページのメインビジュアル背景
- **内容例**: オフィスビル、法律書、スーツ姿のビジネスマンなど

### 事務所外観
- **ファイル名**: `office-exterior.jpg` または `office-exterior.png`
- **推奨サイズ**: 500×300px以上
- **用途**: トップページの事務所紹介セクション

### 代表者写真
- **ファイル名**: `profile-photo.jpg` または `profile-photo.png`
- **推奨サイズ**: 400×500px以上（縦長）
- **用途**: 代表プロフィールページ

### アクセスマップ
- **ファイル名**: `access-map.jpg` または `access-map.png`
- **推奨サイズ**: 600×450px以上
- **用途**: お問い合わせページのアクセス情報

## 画像を配置した後の設定

画像ファイルを配置したら、以下のHTMLファイルを編集してください：

### index.html（事務所外観）
```html
<!-- 現在 -->
<img src="https://picsum.photos/500/300?random=1" alt="事務所外観">

<!-- 変更後 -->
<img src="images/office-exterior.jpg" alt="事務所外観">
```

### profile.html（代表者写真）
```html
<!-- 現在 -->
<img src="https://via.placeholder.com/400x500?text=代表写真" alt="代表 山田太郎">

<!-- 変更後 -->
<img src="images/profile-photo.jpg" alt="代表 山田太郎">
```

### contact.html（アクセスマップ）
```html
<!-- 現在 -->
<img src="https://via.placeholder.com/600x450?text=アクセスマップ" alt="アクセスマップ">

<!-- 変更後 -->
<img src="images/access-map.jpg" alt="アクセスマップ">
```

## 注意事項

- 画像ファイルのサイズは適切に圧縮してください（1MB以下推奨）
- ファイル名は英数字のみを使用してください
- WebP形式もサポートしています（.webp）