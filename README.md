# 阿曽みんなのたたら花火

公開ページ: https://osagix.github.io/azohanabi/

通常のHTML/CSS/JavaScriptで表示する支援メーターです。オンライン・現金寄付の集計値と公開を許可されたコメントのみをGASから取得します。

## 公開方法
リポジトリの Settings → Pages → Source を Deploy from a branch、Branch を main / (root) に設定します。mainへの更新で公開されます。

## 管理
- 公開APIのURLはconfig.jsに設定します。
- Stripeの秘密キー・寄付台帳・管理者情報はこのリポジトリに保存しません。
- 現金受付とStripe Webhookは既存GASで処理します。
- 現在の決済リンクはStripeテスト環境です。本番運用前に本番設定へ変更してください。
- Stripeの決済後URLは公開確認後に上記URLへ変更し、`?thanks=1&session_id={CHECKOUT_SESSION_ID}`を付けます。
