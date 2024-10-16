# subgrade-admin-web
## 项目搭建
1. 项目创建
~~~shell
npm create vue
~~~~
2. 依赖安装
~~~shell
npm install
~~~
3. 启动项目
~~~shell
npm run dev
~~~
4. 打包项目
~~~shell
npm run build
~~~

## 项目结构
```
├── README.md
├── e2e
│   ├── tsconfig.json
│   └── vue.spec.ts
├── env.d.ts
├── eslint.config.mjs
├── index.html
├── node_modules
├── package-lock.json
├── package.json
├── playwright.config.ts
├── public
│   └── favicon.ico
├── src
│   ├── App.vue
│   ├── assets
│   ├── components
│   ├── main.ts
│   ├── router
│   ├── stores
│   └── views
├── tsconfig.app.json
├── tsconfig.json
├── tsconfig.node.json
├── tsconfig.vitest.json
├── vite.config.ts
└── vitest.config.ts

```

## UI组件库
### 安装 Element Plus
1. 安装依赖包
~~~shell
npm install element-plus --save
~~~
2. 配置按需导入
~~~shell
npm install -D unplugin-vue-components unplugin-auto-import
~~~
   
~~~js
// vite.config.ts
import { defineConfig } from 'vite'
import AutoImport from 'unplugin-auto-import/vite'
import Components from 'unplugin-vue-components/vite'
import { ElementPlusResolver } from 'unplugin-vue-components/resolvers'

export default defineConfig({
  // ...
  plugins: [
    // ...
    AutoImport({
      resolvers: [ElementPlusResolver()],
    }),
    Components({
      resolvers: [ElementPlusResolver()],
    }),
  ],
})
~~~

### 配置 Element Plus 组件主题色



## 安装 vueuse
~~~shell
npm i @vueuse/core
~~~
