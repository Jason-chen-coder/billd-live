# 简介

billd 直播间

# 安装依赖

```bash
pnpm install
```

# 项目运行

```bash
pnpm run start
```

script/constant.ts 里的 outputStaticUrl 如果是'/'的话，默认就运行在 [http://localhost:8000/](http://localhost:8000/)，如果 8000 端口被占用了，会自动递增+1
script/constant.ts 里的 outputStaticUrl 如果是'/aaa/'的话，默认就运行在 [http://localhost:8000/aaa/](http://localhost:8000/aaa/)，如果 8000 端口被占用了，会自动递增+1

> 项目启动完成后，终端会打印调试地址，不必担心调试地址是什么~

# 项目打包

```bash
pnpm run build
```

# billd 依赖

更新 billd：

```bash
pnpm i billd-utils@latest billd-scss@latest billd-html-webpack-plugin@latest billd-deploy@latest
```

| 包名                                                                                 | 版本                                                                                                                      |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------- |
| [billd-utils](https://github.com/galaxy-s10/billd-utils)                             | [![npm](https://img.shields.io/npm/v/billd-utils)](https://www.npmjs.com/package/billd-utils)                             |
| [billd-scss](https://github.com/galaxy-s10/billd-scss)                               | [![npm](https://img.shields.io/npm/v/billd-scss)](https://www.npmjs.com/package/billd-scss)                               |
| [billd-html-webpack-plugin](https://github.com/galaxy-s10/billd-html-webpack-plugin) | [![npm](https://img.shields.io/npm/v/billd-html-webpack-plugin)](https://www.npmjs.com/package/billd-html-webpack-plugin) |

- billd-scss，已在 sass-loader 里配置了 additionalData: `@use 'billd-scss/src/index.scss' as *;`
- billd-html-webpack-plugin，已在 webpack 配置里使用了该插件
