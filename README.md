# And Family コミュニティLP

一般社団法人日本マタニティフード協会「And Family」コミュニティのランディングページ。
HTML1ファイル完結・依存なし。`index.html` をブラウザで開けばローカルでも確認できます。

- 公開URL: (Pages設定後にここに記載)
- CTA先: 公式LINE https://lin.ee/6G6ifwV
- 管理: マーケティング室(谷口) / コミュニティチーム(園部)

## 初回公開手順(GitHub Pages・ターミナル不要)

1. GitHubで新規リポジトリ作成
   - Repository name: `andfamily-lp`
   - **Public** を選択(無料プランのPages公開はPublicのみ)
2. リポジトリ画面の「uploading an existing file」から、このフォルダの中身
   (`index.html`, `images/`, `README.md`, `.gitignore`)をドラッグ&ドロップ → Commit changes
3. Settings → Pages → Branch を `main` / `(root)` にして Save
4. 1〜2分待つと `https://<アカウント名>.github.io/andfamily-lp/` で公開されます

## 写真の追加・差し替え

`images/` フォルダに指定ファイル名でアップするだけで自動表示されます(HTML編集不要)。
ファイル名と推奨サイズは `images/画像の入れ方.txt` を参照。

GitHub上での操作: `images` フォルダを開く → Add file → Upload files → 写真をドロップ → Commit。
反映まで1〜2分。

## 文言の修正

`index.html` をGitHub上で開き、鉛筆アイコン(Edit)→ 該当テキストを修正 → Commit。
デザイン(CSS)は `<style>` 内に集約。ブランドカラーは冒頭の `:root` 変数で一括管理:
cream #FDF7E8 / caramel #C97F22 / terracotta #DD6F14 / rose #D88A8A

## 独自ドメイン(任意・後日)

例: `community.maternity-food.org`
1. DNS管理画面でCNAMEレコード追加: `community` → `<アカウント名>.github.io`
2. Settings → Pages → Custom domain に `community.maternity-food.org` を入力 → Enforce HTTPS にチェック

## Claude Codeで改修する場合

```
git clone https://github.com/<アカウント名>/andfamily-lp.git
cd andfamily-lp
claude
```
改修後は `git add -A && git commit -m "変更内容" && git push` で自動反映。

## 注意事項

- Publicリポジトリのため、掲載する写真・文言はすべて公開情報として扱うこと(個人情報・未公開情報は入れない)
- 「約750名」等の数値は実数と乖離したら更新すること
- 写真は写っている方の掲載許諾を確認のうえアップすること
- 旧ペライチURL(簡易版)は検索流入の保険として並存させる運用
