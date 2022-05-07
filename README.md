# fix bin-datav 装饰无法修改颜色的问题

> 原作者一直没有修复这个问题，所以只能自己发布一个修复的版本

 原[BinDataV](https://github.com/wangbin3162/bin-datav) 
`fix`之后的地址：[Vue3BinDatav](https://github.com/BeginnerDone/bin-datav)

# vue3-bin-datav


[![NPM version](https://img.shields.io/npm/v/bin-datav.svg)](https://www.npmjs.com/package/vue3-bin-datav)

### 安装

用如下方式进行安装

```bash
npm i vue3-bin-datav -S
```

### 引入

你可以引入整个`vue3-bin-datav`，或是根据需要仅引入部分组件。我们先介绍如何引入完整的。

#### 完整引入

在 main.js 中写入以下内容：

```javascript
import { createApp } from 'vue'
import BinDatav from 'vue3-bin-datav'
import App from './App.vue'
import 'vue3-bin-datav/lib/styles/index.css'

const app = createApp(App)
app.use(BinDatav)
app.mount('#app')
```

以上代码便完成了 vue3-bin-datav 的引入。需要注意的是，样式文件需要单独引入。

#### 按需引入

如果你只希望引入部分组件，比如 Icon，那么需要在 main.js 中写入以下内容

```javascript
import { createApp } from 'vue'
import { Icon } from 'vue3-bin-datav'
import App from './App.vue'
import 'vue3-bin-datav/lib/styles/components/icon.css'

const app = createApp(App)
app.use(Icon)
app.mount('#app')
```

**特别提醒:按需引用仍然需要导入样式，即在 main.js 或根组件 import 'vue3-bin-datav/lib/styles/index.css';**

