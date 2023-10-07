# 全部OBSで制御できるのライブ姫配信方法「2023/10/07」
- [準備材料](#準備材料)
- [ソフトをインストール](#ソフトをインストール)
  - [ビリビリライブ姫](#ビリビリライブ姫)
  - [OBS](#obs)
  - [mediamtx](#mediamtx)
- [ソフトの設定と使用方法](#ソフトの設定と基本使用方法)
  - [mediamtx](#mediamtx-1)
  - [obs](#obs-1)
  - [ビリビリライブ姫](#ビリビリライブ姫-1)
- [配信開始の手順](#配信開始の手順)
- [配信終了の手順](#配信終了の手順)
- [実現原理](#実現原理)

## 準備材料
- ビリビリライブ姫
  > 今ゲーム配信必要なソフト
- OBS
  > バージョン >= 30
- mediamtx
  > ローカル配信サーバ（[原理と理由](#実現原理)）

## ソフトをインストール

### ビリビリライブ姫
  1. ダウンロード先（[https://live.bilibili.com/liveHime](https://live.bilibili.com/liveHime)）

  2. このボタンをクリック

  ![livehime-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/download/livehime-1.png?raw=true)

  3. さっきダウンロードしたプログラム開いて

  4. ここはインストール先、ご自由に設定してください

  ![livehime-2](https://github.com/Greesea/livehime-with-obs/blob/main/images/download/livehime-2.png?raw=true)

  5. ①をチェックにして、そして②をクリック

  ![livehime-3](https://github.com/Greesea/livehime-with-obs/blob/main/images/download/livehime-3.png?raw=true)

### OBS
  1. ダウンロード先（[https://github.com/obsproject/obs-studio/tags](https://github.com/obsproject/obs-studio/tags)）

  2. 中で**バージョン>=３０**の最新版をクリック

  ![obs-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/download/obs-1.png?raw=true)

  3. ページの真下にスクロールして、**Assets**の中で**Full-Installer**含めてのリンクをクリック

  ![obs-2](https://github.com/Greesea/livehime-with-obs/blob/main/images/download/obs-2.png?raw=true)

  4. 普通にOBSをインストールしてください

### mediamtx
  1. ダウンロード先（[https://github.com/bluenviron/mediamtx/tags](https://github.com/bluenviron/mediamtx/tags)）

  2. 一番上の最新版をクリック

  ![mediamtx-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/download/mediamtx-1.png?raw=true)

  3. ページの真下にスクロールして、**Assets**の中で**windows_amd64**含めてのリンクをクリック

  ![mediamtx-2](https://github.com/Greesea/livehime-with-obs/blob/main/images/download/mediamtx-2.png?raw=true)

  4. 好きな所に解凍してください

## ソフトの設定と基本使用方法

### mediamtx

#### 直接exeを開いてください

![mediamtx-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/mediamtx-1.png?raw=true)

#### プログラムの画面でこの「WebRTC」示す後ろの数字一旦メモしてください

![mediamtx-2](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/mediamtx-2.png?raw=true)

### OBS

#### 配信設定はこのような設定にしてください
> 🟥 配信やすいのため、OBSのプロフィールでライブ姫と連動に専用プロフィール作るのはおすすめです 🟥
>
> サービスの「WHIP」選択は**バージョン>=30**時のみ存在している選択です、ないの場合は[こっち](#obs)に参考してアップデートしてください
>
> サーバーのところは「[http://localhost:8889/live/whip](http://localhost:8889/live/whip)」を基本にして、中の数字は[mediamtxところの数字](#プログラムの画面でこのwebrtc示す後ろの数字一旦メモしてください)に切り替えって、そしてOBS中で入力してください

![obs-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/obs-1.png?raw=true)

### ビリビリライブ姫

#### いつものビリビリログイン画面、ＰＣと同じ方法でログインできる
  - パスワードでログイン

  ![livehime-password](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-password.png?raw=true)

  - SMSでログイン

  ![livehime-sms](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-sms.png?raw=true)

  - 認証がある場合

  ![livehime-verify](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-verify.png?raw=true)

#### 初使用の設定
  1. 要らないもの全部閉じる

  ![livehime-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-1.png?raw=true)

  ![livehime-2](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-2.png?raw=true)

  ![livehime-3](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-3.png?raw=true)

  ![livehime-4](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-4.png?raw=true)

  2. 左下の場所スクロールして、「**直播设置**」押してください

  ![livehime-5](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-5.png?raw=true)

  3. この設定を「**自定义**」にしてください

  ![livehime-6](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-6.png?raw=true)

  4. 全部OBSと同じ設定にしてください、映像エンコーダはGPUやTURING GPUに選択してください

  ![livehime-7](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-7.png?raw=true)

  ![livehime-8](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-8.png?raw=true)

  5. 設定完了した後、マイン画面に戻して、「**素材**」をクリックしてください

  ![livehime-9](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-9.png?raw=true)

  6. 「**浏览器**」をクリックしてください

  ![livehime-10](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-10.png?raw=true)

  7. 画像のように設定してください
  > URLところは「[http://localhost:8889/live?muted=false&controls=false](http://localhost:8889/live?muted=false&controls=false)」を基本にして、中の数字は[mediamtxところの数字](#プログラムの画面でこのwebrtc示す後ろの数字一旦メモしてください)に切り替えって、そして入力してください

  ![livehime-11](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-11.png?raw=true)

  > 画面がフルスクリーンしないの場合は①のところ右クリック、そして②をクリックしてください

  ![livehime-12](https://github.com/Greesea/livehime-with-obs/blob/main/images/setup/livehime-12.png?raw=true)

### 配信開始の手順

1. mediamtx開いてください

> このような仕様ならおｋです

![mediamtx-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/start/mediamtx-1.png?raw=true)

2. OBS開いてください、そしていつものようにOBSの「配信開始」ボタン押してください（今は実際配信していない）

3. ライブ姫開いてください

4. ライブ姫の①のところ全部オフを確認して（オフじゃないの場合はオフに切り替えて、画像中のようなら大丈夫）、②を押してください（今は実際配信中）

![livehime-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/start/livehime-1.png?raw=true)

### 配信終了の手順

1. ライブ姫のこのボタン押してください

![livehime-1](https://github.com/Greesea/livehime-with-obs/blob/main/images/stop/livehime-1.png?raw=true)

2. この画面が出る時はこのボタンを押してください

![livehime-2](https://github.com/Greesea/livehime-with-obs/blob/main/images/stop/livehime-2.png?raw=true)

3. OBSの「配信終了」ボタン押してください

4. mediamtxを直接閉じてください

### 実現原理
> 後で書く
