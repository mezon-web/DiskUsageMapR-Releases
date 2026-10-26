# ダウンロードと照合

[GitHub Releases](https://github.com/mezon-web/DiskUsageMapR-Releases/releases/latest) から、同じ版の以下2ファイルをダウンロードしてください。

- `DiskUsageMapR-v0.3.7.zip`
- `DiskUsageMapR-v0.3.7.zip.sha256.txt`

PowerShellでZIPのSHA-256を計算します。

```powershell
Get-FileHash -LiteralPath .\DiskUsageMapR-v0.3.7.zip -Algorithm SHA256
Get-Content -LiteralPath .\DiskUsageMapR-v0.3.7.zip.sha256.txt
```

両方の64桁の値が一致することを確認してください。大文字・小文字の違いは問題ありません。ZIPを展開し、`DiskUsageMapR-v0.3.7` フォルダ内の `DiskUsageMapR.exe` を起動します。同梱する使い方は `使い方.html` の1つです。[使い方HTMLを単体で保存](https://github.com/mezon-web/DiskUsageMapR-Releases/raw/refs/heads/main/manual.html)することもできます。

必要環境はWindows 11 x64と.NET 10 **Desktop** Runtime x64です。ランタイムは同梱していません。Microsoftの [公式ページ](https://dotnet.microsoft.com/ja-jp/download/dotnet/10.0) から入手できます。

設定はEXE隣の `DiskUsageMapR.settings.json` へ保存します。旧版の `DiskHeatMap.settings.json` が同じフォルダーにあり、新設定がまだなければ初回起動時に引き継ぎます。旧ファイルは残ります。別のフォルダーへ展開する場合は、旧設定ファイルを新EXEの隣へコピーしてから起動してください。

GitHubの「Source code」リンクは公開資料のアーカイブです。アプリのダウンロードには上記の `DiskUsageMapR-v0.3.7.zip` を選んでください。
