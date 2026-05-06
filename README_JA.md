# NTE AutoFish

NTE: Neverness to Everness 向けの Windows 釣り支援ツールです。

![NTE AutoFish thumbnail](assets/nte-autofish-thumbnail.png)

[購入 / ダウンロード](https://cilabworks.lemonsqueezy.com/checkout/buy/33197307-b8af-4bfd-b07a-3355cbcce4b6)
| [デモ動画](https://youtu.be/0h5MJfFbXqk)
| [English guide](README.md)

NTE AutoFish は、画面認識で釣りUIを読み取り、キャスティング、魚が掛かった表示、釣りバー操作、リザルト画面からの復帰を支援する Windows 向けツールです。

## 主な機能

- `F` キーでキャスティングできる釣り待機状態から自動でキャストします。
- 「魚が掛かった」表示を検出して `F` キーを押します。
- 釣りミニゲーム中、黄色い操作バーが判定ライン付近に留まるように `A` / `D` を短く入力します。
- 釣り上げ後のリザルト画面を閉じ、次のキャスト待機へ戻ります。
- 餌切れ表示や釣りメニューを検出した場合は停止します。
- 実入力前に確認できる dry-run モードを同梱しています。

## 推奨環境

- Windows 10/11
- Python 3.11 以降
- NTE はボーダーレスフルスクリーン推奨
- 1920x1080 以上の解像度
- Windows の表示スケール 100%
- HDR と色補正フィルターはオフ推奨

NTE が管理者権限の入力を必要とする環境では、PowerShell またはコマンドプロンプトも管理者として実行してください。

## 購入前の注意

このツールは Python ベースの Windows ツールです。スマートフォンアプリや単体の実行ファイルではありません。

プログラムは、NTE 内で釣り場に立ち、手動で `F` を押すとキャスティングできる「釣り待機状態」から開始する想定です。

解像度、UIスケール、表示モード、HDR設定、ゲームアップデート、アンチチート挙動、アカウント環境によって動作が変わる場合があります。購入前にデモ動画と推奨環境を確認してください。

## 購入後の流れ

配布ZIPには以下が含まれます。

- `install.bat`
- `dry_run.bat`
- `run.bat`
- 英語/日本語の開始ガイド
- 調整用の `settings.json`

基本的な流れ:

```powershell
install.bat
dry_run.bat
run.bat
```

手動コマンドで実行する場合:

```powershell
python -m nte_autofish run --config .\settings.json
```

終了するときは `Ctrl+C` を押してください。

## サポート

セットアップで問題がある場合は、このリポジトリの GitHub Issue に以下を添えて投稿してください。

- Windows バージョン
- Python バージョン
- 解像度と表示スケール
- NTE をボーダーレスフルスクリーンで実行しているか
- どの画面で自動化が止まるか

公開Issueには、個人情報、購入レシート、UID が映ったスクリーンショットを投稿しないでください。

## 免責事項

このツールは非公式の自動化ツールです。Hotta Studio、Perfect World Games、YouTube、GitHub、LemonSqueezy、Neverness to Everness の公式製品ではありません。

ゲームプレイの自動化は、ゲームの利用規約に抵触する可能性があります。利用は自己責任で行ってください。
