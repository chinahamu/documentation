# Documentation Application

## 概要

このプロジェクトは、receiptアプリケーションと統一されたカラーパターンを使用するdocumentationアプリケーションです。

## カラーパレット

### プライマリカラー（Blue系）
信頼性と安定性を表現するブルー系カラーです。メインボタンやナビゲーション要素に使用されます。

- `--color-primary-500: #2563eb` （標準）
- `--color-primary-600: #1d4ed8` （ホバー状態）
- `--color-primary-700: #1e40af` （アクティブ状態）

### セカンダリカラー（Green系）
成功・完了状態を示すグリーン系カラーです。

- `--color-secondary-500: #059669`
- `--color-secondary-600: #047857`
- `--color-secondary-700: #065f46`

### アクセントカラー（Orange系）
警告・注意喚起用のオレンジ系カラーです。

- `--color-accent-500: #ea580c`
- `--color-accent-600: #c2410c`
- `--color-accent-700: #9a3412`

### エラーカラー（Red系）
エラー・削除アクション用のレッド系カラーです。

- `--color-error-500: #dc2626`
- `--color-error-600: #b91c1c`
- `--color-error-700: #991b1b`

### ニュートラルカラー（Gray系）
テキストと背景用のグレー系カラーです。

- `--color-neutral-50: #f9fafb` （背景）
- `--color-neutral-700: #374151` （テキスト）
- `--color-neutral-800: #1f2937` （見出し）

## 使用方法

### CSSファイルの読み込み

```html
<link rel="stylesheet" href="assets/css/theme.css">
```

### 定義済みクラスの使用

#### ボタン
```html
<button class="btn-primary">プライマリボタン</button>
<button class="btn-secondary">セカンダリボタン</button>
<button class="btn-success">成功ボタン</button>
<button class="btn-warning">警告ボタン</button>
<button class="btn-danger">危険ボタン</button>
```

#### アラート
```html
<div class="alert-info">情報メッセージ</div>
<div class="alert-success">成功メッセージ</div>
<div class="alert-warning">警告メッセージ</div>
<div class="alert-error">エラーメッセージ</div>
```

#### フォーム要素
```html
<label class="form-label" for="input">ラベル</label>
<input type="text" id="input" class="form-input" placeholder="入力フィールド">
```

#### カード
```html
<div class="card">
    <div class="card-header">
        <h3>カードタイトル</h3>
    </div>
    <div class="card-body">
        <p>カードの内容</p>
    </div>
</div>
```

### CSS変数の直接使用

```css
.custom-element {
    background-color: var(--color-primary-600);
    color: white;
    border: 1px solid var(--color-primary-700);
}

.custom-text {
    color: var(--color-neutral-700);
}
```

## ファイル構成

```
documentation/
├── assets/
│   └── css/
│       └── theme.css      # メインのテーマファイル
├── index.html             # サンプルページ
└── README.md             # このファイル
```

## receiptアプリケーションとの統一性

このプロジェクトのカラーパターンは、receiptアプリケーションの `resources/css/theme.css` と完全に同期されています。両プロジェクト間で一貫したブランディングとユーザーエクスペリエンスを提供します。

## デモ

`index.html` ファイルを開くことで、定義されたカラーパターンとコンポーネントの実際の表示を確認できます。