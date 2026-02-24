# WanLog（ワンログ）ランディングページ

「話せない分、あなたが記録してあげる。」愛犬の健康記録を一元管理するアプリ「WanLog」のランディングページです。

## 📋 プロジェクト概要

ペット飼い主の課題「動物病院に行ったら便のサンプルを忘れた」という経験から生まれたWanLog。愛犬の健康情報を簡単に記録・管理できるアプリの先行登録ランディングページです。

## 🎯 ページ構成

| セクション | 説明 |
|-----------|------|
| ① キャッチコピー | 「話せない分、あなたが記録してあげる。」 |
| ② ペインの共感 | ユーザーの課題を提示 |
| ③ 3つの主な機能 | 機能説明（画像付き） |
| ④ ターゲット明示 | 「犬を飼っているあなたへ」 |
| ⑤ 先行登録フォーム | Google Forms埋め込み |
| ⑥ フッター | コピーライト表示 |

## 🛠 技術構成

- **フレームワーク**: [Astro](https://astro.build/) - 高速な静的サイトジェネレータ
- **言語**: TypeScript + Astro
- **スタイル**: CSS（グローバルスタイル）
- **画像**: SVG（軽量で拡張性が高い）
- **フォーム**: Google Forms（埋め込みiframe）

## 📁 プロジェクト構造

```
src/
├── components/
│   ├── Hero.astro           # キャッチコピーセクション
│   ├── PainPoint.astro      # ペイン共感セクション
│   ├── Features.astro       # 3つの機能セクション
│   ├── Target.astro         # ターゲット明示セクション
│   ├── CTA.astro            # 先行登録フォーム
│   └── Footer.astro         # フッター
├── pages/
│   └── index.astro          # メインページ
└── styles/
    └── globals.css          # グローバルスタイル

public/
└── assets/
    ├── feature-1.png        # 健康記録の一元管理
    ├── feature-2.png        # 症状の詳細記録
    └── feature-3.png        # 診察の準備が簡単
```

## 🚀 クイックスタート

### 環境構築

```bash
# 依存パッケージをインストール
npm install
```

### 開発サーバーの起動

```bash
npm run dev
```

ブラウザで `http://localhost:3000` にアクセスしてください。

### 本番用ビルド

```bash
npm run build
```

生成されたファイルは `dist/` ディレクトリに出力されます。

### ビルド結果のプレビュー

```bash
npm run preview
```

## 🎨 デザイン

### カラースキーム
- **プライマリ**: #FF6B6B（赤）
- **セカンダリ**: #4ECDC4（青緑）
- **アクセント**: #FFE66D（黄色）
- **テキスト**: #2C3E50（濃紺）

### レスポンシブ対応
- モバイル: 480px以下
- タブレット: 481px〜768px
- デスクトップ: 769px以上

## 📝 カスタマイズガイド

### テキストの変更

各セクションのテキストは `src/components/` 内の `.astro` ファイルで編集できます。

### 画像の置き換え

`public/assets/` フォルダ内の画像を置き換えてください：
- `feature-1.png` → 健康記録画像
- `feature-2.png` → 症状記録画像
- `feature-3.png` → 診察準備画像

### カラーの変更

`src/styles/globals.css` の`:root`セクションでCSS変数を編集：

```css
:root {
    --primary-color: #FF6B6B;       /* プライマリ色 */
    --secondary-color: #4ECDC4;     /* セカンダリ色 */
    --accent-color: #FFE66D;        /* アクセント色 */
    /* ... その他のカラー ... */
}
```

### Google フォームの変更

`src/components/CTA.astro` の iframe `src` 属性を変更してください：

```astro
<iframe
  src="https://docs.google.com/forms/d/e/YOUR_FORM_ID/viewform?embedded=true"
  ...
/>
```

## 📊 ブラウザ互換性

- Chrome（最新版）
- Firefox（最新版）
- Safari（最新版）
- Edge（最新版）
- モバイルブラウザ

## 🌐 デプロイ

### Vercelへのデプロイ

```bash
npm install -g vercel
vercel
```

### Netlifyへのデプロイ

GitHub/GitLabアカウントと連携して自動デプロイが可能です。

詳細は[Astro公式ドキュメント](https://docs.astro.build/ja/guides/deploy/)を参照してください。

## 🔗 関連リンク

- [Astro 公式ドキュメント](https://docs.astro.build)
- [Astro Discord コミュニティ](https://astro.build/chat)

## 📅 更新履歴

- **2026-02-24**: Astro版ランディングページを完成
- **2026-02-24**: Google Forms統合

## 📄 ライセンス

このプロジェクトは自由に使用・修正・配布できます。

---

質問やサポートが必要な場合はお気軽にお問い合わせください。
