# Lisa LP（リンク集＋ミニギャラリー）

Lisa の公式リンク集＋ミニギャラリーの静的サイトです。ビルド不要、そのまま GitHub Pages で公開できます。

## 構成
- `index.html` … 本体（CSS/JS はこの中に入っています）
- `assets/img/` … 画像（hero / avatar / ギャラリー6枚 / 動画ポスター）
- `assets/video/intro.mp4` … 自己紹介動画（10秒・音声あり・約3.2MB）。GitHub Pages は動画も置けますが、重くすると表示が遅くなるので動画は1本あたり10MB以内が目安です
- `.nojekyll` … GitHub Pages 用の空ファイル（そのまま置いてください）

## GitHub Pages での公開手順（Web画面だけ・約5分）
1. GitHub で新しいリポジトリを作る
   - 名前のおすすめ：`lisa-lp`
   - 公開範囲：Public（GitHub Pages の無料利用は Public が基本）
2. このフォルダの中身をすべてアップロードする
   - リポジトリ画面 → `Add file` → `Upload files` → ファイルをドラッグ＆ドロップ → `Commit changes`
   - ※ zip で受け取った場合は、解凍してから中身をアップしてください
3. Pages を有効化する
   - リポジトリの `Settings` → `Pages`
   - `Build and deployment` の Source で `Deploy from a branch` を選ぶ
   - Branch：`main` / フォルダ：`/ (root)` → `Save`
4. 数分待つと公開されます
   - URL は `https://<あなたのGitHubユーザー名>.github.io/lisa-lp/` の形
   - 公開されたら Instagram プロフィールのリンクを Beacons からこの URL に差し替え可能
     （差し替えは Beacons の様子を見てからでOKです）

## 独自ドメイン（任意・後からでOK）
- ドメインを取得したら、リポジトリに `CNAME` というファイルを作り、ドメイン名だけを書く
- ドメイン側の DNS に GitHub Pages 向けの設定を追加する

## 更新のしかた
- 写真を差し替えたい：`assets/img/` の同名ファイルを上書きアップロード
- ギャラリーを増やしたい：`index.html` の `Mini Gallery` 部分の `<figure>` を1つコピーして画像名とキャプションを変える
- リンク先変更：`index.html` 内の該当URLを書き換えるだけ

## メモ
- X のリンクは、ハンドルが @lisapple_156 に変更できてから公開する設計です。
  `index.html` のリンク部分に差し替え用コードがコメントで入っています。
- サウナ写真は仕様（ドリンク等）の確定版と合わないカットがあったため、ギャラリーには入れていません。
