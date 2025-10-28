# [Image Converter]
![image1](images/image-1.png)

## Recommended Environment
This tool is designed for use on a PC with the Google Chrome browser. Operation on other devices or browsers is not guaranteed.

## 推奨環境
このツールは、PC上のGoogle Chromeブラウザでの使用を想定しています。他のデバイスやブラウザでの動作は保証されていません。

## Demo
You can try this tool on the page below.

https://black-sesame-ice-cream.github.io/image-converter/

## デモ
以下のページでこのツールを試すことができます。

https://black-sesame-ice-cream.github.io/image-converter/

## Overview
This is a client-side web tool for bulk image file conversion. All processing is completed within the browser, and no files are uploaded to a server.

It supports converting from JPEG, PNG, WebP, BMP, GIF, and HEIC/HEIF formats. Output formats include JPEG, PNG, WebP, and BMP. The converted files are downloaded together as a single ZIP file.

### Features
- **Batch Conversion**: Convert multiple files at once.
- **Client-Side Processing**: Operates entirely within your browser for privacy and speed.
- **Input Formats**: JPEG, PNG, WebP, BMP, GIF, HEIC, HEIF
- **Output Formats**: JPEG, PNG, WebP, BMP
- **Conversion Options**:
    - Output Format (JPEG, PNG, WebP, BMP)
    - Quality (For JPEG and Lossy WebP)
    - WebP Type (Lossy / Lossless)
    - Resize (Scale percentage)
- **Output**: Downloads all converted images in a single ZIP file.

## 概要
クライアントサイドで動作する画像ファイルの一括変換ツールです。すべての処理はブラウザ内で完結し、ファイルがサーバーにアップロードされることはありません。

JPEG, PNG, WebP, BMP, GIF, HEIC/HEIF 形式からの変換に対応しています。出力形式は JPEG, PNG, WebP, BMP です。変換されたファイルはZIPファイルとして一括ダウンロードされます。

### 主な機能
- **一括変換**: 複数のファイルを一度に変換します。
- **クライアントサイド処理**: プライバシーと速度のため、すべての処理がブラウザ内で完結します。
- **入力形式**: JPEG, PNG, WebP, BMP, GIF, HEIC, HEIF
- **出力形式**: JPEG, PNG, WebP, BMP
- **変換オプション**:
    - 出力形式 (JPEG, PNG, WebP, BMP)
    - 品質 (JPEG および 非可逆WebP)
    - WebPタイプ (非可逆 / 可逆)
    - リサイズ (パーセンテージ指定)
- **出力**: 変換されたすべての画像を単一のZIPファイルでダウンロードします。

## Usage
1.  Drag and drop image files onto the designated area, or click the area to select files from your computer.
2.  The selected files will be added to the "Media Pool" on the right. (HEIC/HEIF files will be pre-converted to PNG for preview).
3.  You can remove individual files by clicking the 'X' button next to them, or clear all files using the "Clear All" button.
4.  In the "Conversion Options" section below, select the target format (e.g., JPEG, WebP).
5.  Adjust the options (Quality, WebP Type, Resize) as needed. Options will be enabled or disabled based on the selected format.
6.  Click the "Convert and Save as ZIP" button.
7.  The tool will process all files in the pool, and a ZIP file named `converted_images.zip` will be downloaded.

## 使い方
1.  指定されたエリアに画像ファイルをドラッグ＆ドロップするか、エリアをクリックしてファイルを選択します。
2.  選択されたファイルが右側の「メディアプール」に追加されます。（HEIC/HEIFファイルはプレビューのためにPNGに事前変換されます）
3.  個別のファイルを削除したい場合は、ファイル名の横にある「X」ボタンをクリックします。「すべてクリア」ボタンでプール全体を空にすることもできます。
4.  下部の「変換オプション」セクションで、変換先の形式（例: JPEG, WebP）を選択します。
5.  必要に応じて品質、WebPタイプ、リサイズの各オプションを調整します。オプションは選択した形式に応じて有効化・無効化されます。
6.  「変換してZIPで保存」ボタンをクリックします。
7.  プール内のすべてのファイルが処理され、`converted_images.zip` という名前のZIPファイルがダウンロードされます。

## Licenses
Please see below for details.

[License](LICENSE/)

[Third-Party Licenses](THIRD-PARTY-LICENSES.txt/)

## ライセンス
以下を参照してください。

[ライセンス](LICENSE/)

[第三者ライセンス](THIRD-PARTY-LICENSES.txt/)

## Tech Stack
- **Core**: HTML, CSS, JavaScript (Async/Await)
- **Styling**: Tailwind CSS
- **ZIP Archiving**: JSZip.js
- **HEIC/HEIF Support**: heic2any.js
- **PNG Encoding**: UPNG.js
- **PNG Compression**: pako.js (Dependency for UPNG.js)