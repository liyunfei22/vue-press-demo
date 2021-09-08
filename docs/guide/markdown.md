# markdown
[首页](../README.md)

[GITHUB](https://github.com)

VuePress 2 已经发布 :tada: ！
[[toc]]
# b
```ts{1,6-8}
import type { UserConfig } from '@vuepress/cli'

export const config: UserConfig = {
  title: '你好， VuePress',

  themeConfig: {
    logo: 'https://vuejs.org/images/logo.png',
  },
}
```
```ts
// 行号默认是启用的
const line2 = 'This is line 2'
const line3 = 'This is line 3'
```

```ts:no-line-numbers
// 行号被禁用
const line2 = 'This is line 2'
const line3 = 'This is line 3'
```
```md
<!-- 默认情况下，这里会被保持原样 -->
1 + 2 + 3 = {{ 1 + 2 + 3 }}
```

```md:no-v-pre
<!-- 这里会被 Vue 编译 -->
1 + 2 + 3 = {{ 1 + 2 + 3 }}
```
```js:no-v-pre
// 由于 JS 代码高亮，这里不会被正确编译
const onePlusTwoPlusThree = {{ 1 + 2 + 3 }}
```
一加一等于： {{ 1 + 1 }}
<span v-for="i in 3"> span: {{ i }} </span>
这是默认主题内置的 `<Badge />` 组件 <Badge text="演示" />
