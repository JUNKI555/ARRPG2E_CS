# Arianrhod RPG 2E Character Sheet Project.

## commit messages
git emoji
参考：[gitmoji](https://gitmoji.carloscuesta.me/)

## ローカルでの立ち上げ方
1. `yarn`
2. `yarn dev`
3. `localhost:5000` で確認

## ローカルで立ち上げて同じwifi内の別端末(スマホなど)で確認
1. `yarn devMobile`

参考：
By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the `sirv` commands in package.json to include the option `--host 0.0.0.0`.

## デプロイ用ビルド
1. `yarn build`

## production mode での起動
1. `yarn build`
2. `yarn start`

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


## Single-page app mode

By default, sirv will only respond to requests that match files in `public`. This is to maximise compatibility with static fileservers, allowing you to deploy your app anywhere.

If you're building a single-page app (SPA) with multiple routes, sirv needs to be able to respond to requests for *any* path. You can make it so by editing the `"start"` command in package.json:

```js
"start": "sirv public --single"
```

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
