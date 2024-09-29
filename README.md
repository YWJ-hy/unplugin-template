# unplugin-template

当前unplugin模板是 fork 自 [unplugin-starter](https://github.com/unplugin/unplugin-starter/tree/main)
做了部分改动

## 模板使用

```js
npx degit YWJ-hy/unplugin-template my-unplugin
```

## Install

```bash
npm i unplugin-template -D
```

## ⚙️ Options

```ts
interface Options {

}
```

<details>
<summary>Vite</summary><br>

```ts
// vite.config.ts
import Unplugin from 'unplugin-template/vite'

export default defineConfig({
  plugins: [
    Unplugin({ /* options */ }),
  ],
})
```

Example: [`playground/`](./playground/)

<br></details>

<details>
<summary>Rollup</summary><br>

```ts
// rollup.config.js
import Unplugin from 'unplugin-template/rollup'

export default {
  plugins: [
    Unplugin({ /* options */ }),
  ],
}
```

<br></details>

<details>
<summary>Webpack</summary><br>

```ts
// webpack.config.js
module.exports = {
  /* ... */
  plugins: [
    require('unplugin-template/webpack')({ /* options */ })
  ]
}
```

<br></details>

<details>
<summary>Nuxt</summary><br>

```ts
// nuxt.config.js
export default defineNuxtConfig({
  modules: [
    ['unplugin-template/nuxt', { /* options */ }],
  ],
})
```

> This module works for both Nuxt 2 and [Nuxt Vite](https://github.com/nuxt/vite)

<br></details>

<details>
<summary>Vue CLI</summary><br>

```ts
// vue.config.js
module.exports = {
  configureWebpack: {
    plugins: [
      require('unplugin-template/webpack')({ /* options */ }),
    ],
  },
}
```

<br></details>

<details>
<summary>esbuild</summary><br>

```ts
// esbuild.config.js
import { build } from 'esbuild'
import Unplugin from 'unplugin-template/esbuild'

build({
  plugins: [Unplugin()],
})
```

<br></details>
