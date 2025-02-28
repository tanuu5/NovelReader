# ScriptedScrollReader

ScriptedScrollReaderは、ブラウザで動作する縦書きと横書きをサポートする日本語電子書籍ビューアです。モバイルデバイスとデスクトップの両方で最適化されています。

![Sample](https://github.com/tanuu5/NovelReader/assets/134081795/55c1fe98-2a5b-4aaa-8d8e-83cd9c78cefd)

## 概要

このプロジェクトは、縦書きおよび横書きのテキスト表示に対応した電子書籍ビューアを提供します。日本語のコンテンツを閲覧するために最適化されており、下記の特徴があります：

- 縦書き/横書きの切り替え機能
- フォント選択（Noto Sans JP、Sawarabi Mincho、Kosugi Maru、游ゴシック）
- しおり機能（読んでいる位置を保存）
- 行間調整
- 複数のカラーテーマ（標準、ダーク、薄黄色背景）
- レスポンシブデザイン（スマートフォンやタブレットに対応）
- キーボードショートカット

## デモ

デモは[こちら](https://your-demo-url.com)で試すことができます。（※実際のURLに更新してください）

## セットアップ

1. リポジトリをクローンまたはダウンロードします：
   ```
   git clone https://github.com/tanuu5/ScriptedScrollReader.git
   ```

2. ローカルサーバーで実行するか、`index.html`をブラウザで直接開きます。
   
   ```
   # Python 3の場合
   python -m http.server
   
   # Node.jsの場合
   npx serve
   ```

## 使用方法

### 基本操作

- **縦書き/横書きの切り替え**：「縦/横書き」ボタンをクリック
- **しおりを挟む**：「しおり🔖」ボタンをクリック
- **行間調整**：「行間大」「行間中」「行間小」ボタンで調整
- **フォント変更**：「フォント変更」ボタンでフォントを循環
- **テーマ変更**：「標準テーマ」「ダークテーマ」「薄黄色の背景」で変更

### キーボードショートカット

- **Ctrl+T**：縦書き/横書き切り替え
- **Ctrl+B**：しおり保存
- **Ctrl+F**：フォント変更

### モバイル操作

- **左右スワイプ**：章の移動
- **ツールバースワイプ**：表示されていないボタンを表示

## 独自コンテンツの追加

`content.html`ファイルを編集して、独自のテキストコンテンツを追加できます。

```html
<div class="toc">
  <h1>タイトル</h1>
  <h3>目次</h3>
  <ul>
    <li><a href="#chapter1">第1章：章のタイトル</a></li>
    <!-- 他の章 -->
  </ul>
</div>

<div id="content" class="content">
  <h4 id="chapter1">第１章：章のタイトル</h4>
  <p><ruby>漢字<rt>かんじ</rt></ruby>を含むテキスト</p>
  <!-- テキストコンテンツ -->
</div>
```

## ブラウザ互換性

- Chrome
- Firefox
- Safari
- Edge
- モバイルブラウザ（iOS Safari、Android Chrome）

## 開発計画

- [ ] ePubファイルのサポート
- [ ] テキストサイズの調整機能
- [ ] 暗闇モードの自動切り替え
- [ ] ユーザー辞書によるふりがな自動生成
- [ ] 画像のサポート強化

## 貢献

プロジェクトへの貢献はいつでも歓迎です。バグの報告、新機能の提案、コードの改善などについては、GitHubのissueやプルリクエストを通じてお知らせください。

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。詳細は[LICENSE](LICENSE.md)ファイルを参照してください。
