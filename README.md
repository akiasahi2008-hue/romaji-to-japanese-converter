# ローマ字→日本語変換ツール (Romaji to Japanese Converter)

Google Gemini API を活用し、入力されたローマ字を自然な「漢字・かな交じり」の日本語に一瞬で変換する完全ブラウザ完結型のWebツールです。

🔗 **[アプリを使う (GitHub Pages)](https://akiasahi2008-hue.github.io/romaji-to-japanese-converter/)**

## 💡 特徴

*   **サーバー・PHP不要**: すべてブラウザ上のJavaScriptで動作するため、サーバー環境の構築は一切不要です。
*   **文脈からのタイプミス補正**: スペースなしで連続入力したローマ字（例: `korenaraumakuikisoukana`）はもちろん、明らかなタイピングミス（例: `kyouhatiyottosamui`）も文脈を読み取ってAIが自動補正します。
*   **高速レスポンス**: 高速な `gemini-3.1-flash-lite` モデルを使用しているため、高速な変換が可能です。
*   **安心のAPIキー管理**: 入力したAPIキーはブラウザの `localStorage` にのみ保存され、外部サーバーに送信・記録されることはありません。

## 🚀 使い方

1. [アプリのURL](https://akiasahi2008-hue.github.io/romaji-to-japanese-converter/) にアクセスします。
2. 初回起動時は「設定」パネルが開くので、ご自身の **Google Gemini APIキー** を入力して保存します。
   *(※APIキーは [Google AI Studio](https://aistudio.google.com/) から無料で取得できます)*
3. エディタ部分にローマ字を入力し、`Enter` キーで改行します。
4. `Ctrl + Shift + J` を押す（または「変換」ボタンをクリックする）と、直前の行が日本語に変換されます。

## 💻 ローカル環境での実行方法

このリポジトリをZIPダウンロード、または `git clone` して `index.html` をPC上で直接ダブルクリックするだけでも完全に動作します。

## ⚙️ 使用技術

*   HTML5 / CSS3 / Vanilla JavaScript
*   Google Gemini API (Generative Language API)

## 📄 ライセンス

このプロジェクトはオープンソースです。自由に変更・活用していただいて構いません。
