**One-Core-API バイナリへようこそ!**
***
**言語：**
[英語](README.md) | [简体中文](README_CN.md) | [Русский](README_RU.md) | [Українська](README_UK.md)  | [日本語](README_JP.md) | [Português do Brasil](README_BR.md)
***
***この日本語訳は機械翻訳をベースに誤訳などをできる限り修正したものです 間違いがある可能性があります***

このリポジトリには、One-Core-API プロジェクトのバイナリ リリースが含まれています。 これらは、Windows Server 2003 SP2、Windows XP SP3、および Windows XP x64 SP2 と互換性があります。


**公式 Discord サーバー**: https://discord.gg/eRcGuFtn6p

**注記**：
- Windows XP 非公式 SP4 およびおそらく Integral Edition はサポートされていません。

**言語サポート**
ほぼ すべての Windows 部分の言語サポート: ポルトガル語 (ブラジル)、ポルトガル語 (ポルトガル)、トルコ語、中国語 (繁体字および簡体字)、フランス語、イタリア語、ハンガリー語、ウクライナ語 (部分的)、スペイン語、ポーランド語、ロシア語、韓国語。

**このリポジトリ内のフォルダー:**
- Documents: プロジェクトのドキュメント、既知のバグ、sfxcab の使用法 (インストーラー作成用) など。
- Packages\x86 および Packages\x64: パッケージごとに分類されたバイナリ リリース。 ここからパッケージを直接ダウンロードしてインストール/更新できます (つまり、Packages\x86\Base installer\update に移動して update.exe を実行します)。
- Todo: やるべきタスク
- Test: テスト用のいくつかのバイナリとドキュメント。
- release: 新しいバイナリ リリースを生成するスクリプト。
- Output: バイナリ出力。リリース フォルダーのスクリプトを使用して生成できます。

**One-Core-API バイナリ プロジェクトは次のパッケージで構成されています:**
警告: OCA パッケージの再起動が必要な場合は、必ず再起動してください。 すべてのパッケージをインストールし、最後のパッケージだけを再起動すると、Windows が破損します。
- **Base**: One-Core-API のメイン パッケージであり、App Compat と Driver Update を除く他のすべてのパッケージで必要であり、このプロジェクトで使用されるすべてのラッパー (kernelbase や ntext など) が含まれています。
- **Additional Dlls**: Windows の以降のバージョンで導入されたいくつかの新しい DLL。
- **D3d**: D3D ランタイム (主に WineD3D に基づく DX10 および DX11);
- **App Compat**: Windows の新しいバージョンからバックポートされたアプリケーション互換性設定。
- **Driver Update**: ACPI 2.0 をサポートする最新の acpi ドライバー、Storachi (AHCI ドライバー コントローラー用)、NVME (NVME M.2 ドライバー コントローラー用)、USBXHCI (USB 3.0) などの新しいドライバーを導入します。
- **Branding**: Windows Vista で導入された新しいブランド システム。D3D および Modern Setup パッケージに必要です。

**パッケージのインストール順序:**
- **一般的な順序**: Base-> Additional Dlls -> Branding -> D3d -> Driver Update -> App Compat;

- **スタンドアロン パッケージ (必要な場合のみ、他のパッケージを一緒に使用する必要はありません)**
   - **App Compat のみ:** このパッケージは、他のパッケージなしでインストールできます。
   - **Driver Updateのみ**: このパッケージは、他のパッケージなしでインストールできます。
   - **AppCompat を最初に**: このパッケージは、他のパッケージなしでインストールできます。

**主な特徴**：
- x86では128GB、x64では2TBのメモリをデフォルトでサポート；
- 最新のWindows OS用に設計された新しいプログラムの実行をサポートする；
- 新しいドライバ・コントローラで新しいハードウェアをサポートできるようにする。
  
**One-Core-API を使用すると、以下を実行できます。**
- JetBrains WebStorm 2018;
- Intellij 2018 (他のバージョンも動作する可能性があります);
- JetBrains WebStorm 2023.x.x (現時点では Windows XP x64 のみ)
- JetBrains IntelliJ 2023.x.x (現時点では Windows XP x64 のみ)
- Adobe Photoshop CC 2018;
- Filezilla (最新);
- Visual Studio コード 1.83.1 まで。
- Chrome はバージョン 122 まで!;
- Opera バージョン 105 まで。
- Firefox バージョン 116 まで (バグがあり、回避策が必要)。
- Microsoft Edge バージョン 115 まで。
- バージョン 117 までブレイブ;
- Yandex ブラウザの最新バージョン;
- 最大 109 のトリウムブラウザ;
- Supermium バージョン 117 まで。
- Seamonkey バージョン 2.53.10 まで。
- Thunderbird バージョン 115 まで。
- Maxthon バージョン 7.1.6 まで。
- 最新バージョンまでの Vivaldi;
- JDK 1.8 (現時点では Windows XP x64 のみ);
- バージョン 21 までの Java Alternative JDK または OpenJDK (他のバージョンでも動作する可能性があります)。 https://bell-sw.com/pages/downloads/#/java-11-lts からダウンロードできます。
- Maxthon 6;
- Epic Browser 94;
- Python 3.6;
- .Net Framework 4.8 まで。
- Geekbench 4.2;
- Performance Test;
- Adobe Reader DC (2017);
- Windows 7 ゲーム;
- Windows Vista ネイティブ アプリケーション;
- Windows XP/Vista サポート終了後の Spotify、バージョン 1.0.60。
- Yandex ブラウザ (最新);
- Zoom;
- 他のいくつかのアプリケーション;
- Node 10.24;
- Winrar 6.24 (最新);
- Directx 9EX、10、11 ゲーム:
   - ニード・フォー・スピード モスト・ウォンテッド (2012);
   - ニード・フォー・スピード・ザ・ラン;
   - ストリートファイターV;
   - インジャスティス：神々の激突
   - アサシン クリード IV ブラック フラッグ。
   - Crysis 1、2、および 3 (directx 10-11 モード);
- Kate 23.08.1 (現時点では Windows XP x64 のみ)
  
**既知の制限事項:**
- IFileDialog と呼ばれる Vista 実装によるため、いくつかのアプリケーションの開く/保存ダイアログが完全に動作しません。 現在作業中です。
- Firefox 56 以降を実行すると、ページの読み込みの問題が発生する可能性があります。 これを解決するには、バージョン 55 から 72 では、 MOZ_FORCE_DISABLE_E10S という環境変数を作成する必要があります。 これはユーザーの環境変数のキーとなり、値は 1 になります。バージョン 73 以降の場合、値はバージョン番号、つまり 73.0.0 になります (バージョン番号を確認してください)。
- ダイアログまたはウィンドウの一部の場所は英語のみのままです。 国際化は進行中です。
- Chrome、Maxthon、Discord、Team viewerなどの新しいアプリケーションのインストーラーがクラッシュし、アプリケーションがインストールされないことがあります。必要なもの 
他のオペレーティングシステムからコピーしたプリインストールバージョンを使用してください；
- Firefox 55-116 はいくつかの制限付きで動作します。
- バージョン 54 (32 ビット) 以降の Firefox は、Windows XP x64 では動作しません。 Chrome 61 以降も動作しません。
- 標準の Microsoft バージョンではなく、「SFXCAB Substitute」と呼ばれるツールを使用するため、パッケージを nlite を利用し WindowsのIso に統合することはできません。
- 4.6 以降の標準 .Net Framework インストーラーは、現時点ではサポートされていません。 このような再パックされたバージョンが必要です: https://github.com/abbodi1406/dotNetFx4xW7。 そして、ここで利用可能です: https://www.wincert.net/forum/topic/13805-microsoft-net-framework-472-full-x86x64-incl-language-packs-by-ricktendo/#comment-123251. 他のバージョンも入手可能です。フォーラムのトピックを検索してください。
- Palemoon バージョン 27 ～ 31 はダウンロードできない。ダウンロードが開始されません；
- Opera 39 ～ 46 を起動するには、次のパラメータが必要な場合があります: --disable-gpu (黒い画面を防ぐため) および --single-process (永遠に最初のページが読み込まれるのを防ぐため)。
- Dwrite を使用する Qt5 アプリケーションが起動時にクラッシュします。 dwrite を削除すると黒い画面になるなどの不具合があります (ただし、アプリケーションは起動し、使用できます)


**問題レポート**

注：
ChromeやChromiumベースのブラウザに問題が発生している場合は、以下のリンクから報告してください: https://github.com/Skulltrail192/One-Core-API-Binaries/issues/178。

FirefoxやGeckoベースのブラウザに関連する問題の場合は、次のGitHubリンクを使用して報告してください: https://github.com/Skulltrail192/One-Core-API-Binaries/issues/214。

問題がBSoD（ブルースクリーンオブデス）に関連している場合は、以下のページで報告を検討してください: https://github.com/Skulltrail192/One-Core-API-Binaries/issues/233。

問題を再現するには、**常に**このテンプレートに従うことをお勧めします。
- 何が起こったのか説明してください。
   例: Windows をロードしようとすると、常に BSOD が発生します。 Windows がブート画面で停止する。 Windows で常に黒い画面が表示される
- VM/PC構成
   例: Vmware 10、virtualBox 6.1.0 または Core 2 Duo 8400、2Gb DDR2、IDE/SATA ハードディスク。
- Windows のエディションと構成
   例: POSReady 2009 updatesがインストールされた Windows XP Service Pack 3、プログラム リスト: Adobe、office など。

XP/Server2003上で動作するApplicaionのスクリーンショット：
**Chrome 122**
![Chrome 122](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/6442a5b0-036b-48e0-a6e8-3624825d3882)

**Edge 122**
![Edge122](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/734954f4-2540-4657-9a2d-ce6aed809bf5)

**Opera 106**
![Opera106](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/db509ccf-4e66-4e2b-ad4b-fd8512495333)

**Firefox 122**
![Firefox122](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/db647daf-0960-4ace-ad2f-63469dbf3881)

**Basilisk**
![image_2022_04_08T21_38_17_976Z](https://user-images.githubusercontent.com/5159776/178077859-079bfca4-bdb6-402e-8991-b88e7dfe387c.png)

**Vivaldi**
![vivaldi](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/86d5895f-977a-414f-b0d5-0e877a658676)

**Spotify (Windows 7用)**
![Spotify-Windows7](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/09de7c20-8670-45dc-9471-a6db9349abd0)

**Visual Studio Code 1.81**
![VisualCode](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/b21748b9-25bb-412d-95b3-2219d2efdf42)

**Microsoft Chess 3d**
![Chess3d](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/bd1ad0c6-edde-4ff2-a6e0-074c7379fab6)

**Libre Office 24 (最新)**
![LibreOffice](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/11fd191d-270c-428d-8d41-0498e8fafb3b)
![Writer-LibreOffice](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/e389a39b-febd-45f6-9c6f-25f64e460142)

**Discord 0.309**
![Discord-Login](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/8a4c12b5-19fc-454d-b02a-a1db807d3900)
![Discord](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/eb673541-4e66-4c76-867e-346edbaaa0af)

**Telegram Desktop**
![Telegram-Desktop](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/d23b9add-629d-45a3-a8e1-c331271bc0d3)

**Zoom meeting**
![Zoom](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/d002cf1b-c5f4-4c0c-b629-00e031a56765)

**Java 11**
![Capturar](https://user-images.githubusercontent.com/5159776/178078132-da504607-a1ca-4f8d-ae25-6a7eb367bdaa.PNG)

**Avast と Chromium 68**
![Avast](https://user-images.githubusercontent.com/5159776/178078208-c13b3448-ee6a-4c56-9d94-d0c62d51949e.PNG)

**Windows 7 Sticky Notes**
![StickyNotes](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/669ba3e4-b831-4a96-ad40-d87e3e9531e2)

**Windows 7 Paint**
![Paint](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/81728a44-c9e7-41e8-b68b-8ea7b119ebba)

**Windows 7 Wordpad**
![Wordpad](https://github.com/Skulltrail192/One-Core-API-Binaries/assets/5159776/9dac02c7-7139-47fe-8732-ccd9ef91090b)



