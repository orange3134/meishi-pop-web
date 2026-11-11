# MEISHI Pop! 公開ページ

ピピピ技研のiPhoneアプリ「MEISHI Pop!」のプライバシーポリシーとサポート窓口です。
HTML / CSSのみ。JavaScript、外部フォント、アクセス解析、広告、Cookieは使用しません。

## 公開URL

- プライバシーポリシー： https://orange3134.github.io/meishi-pop-web/
- サポート： https://orange3134.github.io/meishi-pop-web/support.html

GitHub Pagesの公開元は `main` ブランチの `/docs` です。
`docs/index.html` / `docs/support.html` / `docs/style.css` を編集し、mainへpushすると反映されます。

ローカル確認： `python3 -m http.server 8080 --directory docs`

## App Storeへの登録・申請前の確認

調査日：2026年11月11日。ページ作成時のコード調査であり、App Store審査通過やSDK内部の挙動の保証ではありません。

1. App Store Connectの「プライバシーポリシーURL」に上記URLを登録します。
2. 「サポートURL」には上記サポートURLを登録できます。
3. **アプリ内の設定画面などにもプライバシーポリシーへのリンクを追加してください。** ページ作成時のアプリの設定画面にはありません。このWebリポジトリの作業ではアプリを変更していません。
4. App Store Connectの「Appのプライバシー」はURL登録とは別です。現行のアプリ自身の実装では、名刺等はローカル処理で、Unity Analytics / Ads / Crash Reportingは無効です。Appleの定義上、端末内だけの処理は収集に該当しません。ただし「データを収集しない」と確定する前に、提出用ビルドと組み込む全SDK（特にバイナリ配布のSony製SRD SDK）の外部送信・保存の有無を提供元の資料と実機で確認してください。
5. お問い合わせ情報を任意開示扱いにできるかは、実際の収集方法とAppleの全条件に基づき判断してください。任意の問い合わせという理由だけで一律に申告不要とはしていません。Appleが独自に収集するデータと、開発者が利用する診断データも分けて判断してください。
6. プライバシーマニフェスト（PrivacyInfo.xcprivacy）とRequired Reason API、対象SDKの署名・マニフェスト要件は別途、提出するアーカイブで確認します。Webページではこれらを代替できません。
7. 運営者は、問い合わせメール・添付資料を対応完了後1年以内に削除する運用を継続してください。機能・SDK・問い合わせ方法が変わったら、本ページとApp Store Connectの回答を更新します。

## 内容の根拠

- プロフィール、画像、VRM / mpavatar、設定は端末内のファイルとして保存。
- QRは組み込みライブラリで生成。テクスチャ読み込みのUnityWebRequestは一時ローカルファイルに対するもの。
- 写真はPHPicker、ファイルはiOSのドキュメントピッカーでユーザーが選択。
- Sony製SDKの視点情報を表示とアバター制御に利用。アプリのコードに視点履歴の保存や運営者への送信は見つかっていません。SDKネイティブバイナリ内部や実機ネットワーク通信は未検証です。一般向けSRDの資料を、別の小型SRD用SDKの保証として扱っていません。
- 名刺削除は共有アバターを削除せず、JSON保存のバックアップが残る場合があるため、全削除手順を分けて記載。
- GitHub Pagesは閲覧者のIPアドレスをセキュリティ目的で保存するため、アプリのデータ処理と分けて説明。
- 運営者名、公開メールアドレス、問い合わせ情報の保存期間は運営者の指定。

## 公式資料

- [Apple App Review Guidelines 5.1.1](https://developer.apple.com/app-store/review/guidelines/#data-collection-and-storage)
- [Apple App Privacy Details](https://developer.apple.com/app-store/app-privacy-details/)
- [Apple：プライバシー情報の管理](https://developer.apple.com/help/app-store-connect/manage-app-information/manage-app-privacy/)
- [Apple：第三者SDK要件](https://developer.apple.com/support/third-party-SDK-requirements/)
- [Apple：PHPickerのプライバシー](https://developer.apple.com/videos/play/wwdc2021/10046/)
- [GitHub Pagesのデータ収集](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection)
- [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)
- [Google プライバシーポリシー](https://policies.google.com/privacy?hl=ja)
