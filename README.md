# wangEditor for React

<!-- Badge -->

![MIT License](https://img.shields.io/badge/License-MIT-blue)
![jest badge](https://img.shields.io/badge/unit%20test-jest-yellowgreen)

[English documentation](./README-en.md)

## 介绍

基于[wangEditor](https://www.wangeditor.com/) 封装的 React 组件。

## 安装

1. 安装组件包

```shell
yarn add @42how/editor-for-react
# 或者npm install @42how/editor-for-react --save

```

2. 安装核心包

```shell
yarn add @42how/editor

# 或者 npm install @42how/editor --save
```

3. 导入组件

```ts
import { Editor, Toolbar } from "@42how/editor-for-react";
```

## 使用

详情参考[wangEditor react 使用文档](https://www.wangeditor.com/v5/for-frame.html#react)。

### 在 Next.js 下使用

```js
import dynamic from "next/dynamic";
const WangEditor = dynamic(
  // 引入对应的组件 设置的组件参考上面的wangEditor react使用文档
  () => import("../components/myEditor"),
  { ssr: false }
);

export default function Home() {
  return <WangEditor />;
}
```

使用案例可以参考[wangeditorV5-nextjs-demo](https://github.com/hahaaha/wangeditorV5-nextjs-demo)
