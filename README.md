# Arianrhod RPG 2E Character Sheet Project.

## 素晴らしい先行ツール様
- アリアンロッド キャラクター作成補助ツール - 全て非公式
  - http://allunofficial.net/trpg/arianrhod_pc_making.html

## commit messages
git emoji
参考：[gitmoji](https://gitmoji.carloscuesta.me/)

## 開発の流れ
### ローカルでの立ち上げ方
1. `yarn`
2. `yarn dev`
3. `localhost:5000` で確認

### ローカルで立ち上げて同じwifi内の別端末(スマホなど)で確認
1. `yarn devMobile`
2. `http://your-pc-name` などでアクセス
3. 例えば Mac でならここなど参考 [iPhoneからMac上のRailsアプリにlocalhostでアクセスする方法 - もちゅろぐ](https://blog.mothule.com/mac/how-to-access-localhost-from-ios)

参考：
By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the `sirv` commands in package.json to include the option `--host 0.0.0.0`.

### デプロイ用ビルド
1. `yarn build`

### production mode での起動
1. `yarn build`
2. `yarn start`

---

## Built With:
- [Svelte](https://svelte.dev/)
- TypeScript
- SCSS
- [NES.css](https://nostalgic-css.github.io/NES.css/)
- [favicon.io](https://favicon.io/)

---

以下 sveltejs/template　のデフォルト README.md を一部残し

---

*Looking for a shareable component template? Go here --> [sveltejs/component-template](https://github.com/sveltejs/component-template)*

---

## Building and running in production mode

To create an optimised version of the app:

```bash
npm run build
```

You can run the newly built app with `npm run start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies` so that the app will work when you deploy to platforms like [Heroku](https://heroku.com).

## Deploying to the web

### With [Vercel](https://vercel.com)

Install `vercel` if you haven't already:

```bash
npm install -g vercel
```

Then, from within your project folder:

```bash
cd public
vercel deploy --name my-project
```
