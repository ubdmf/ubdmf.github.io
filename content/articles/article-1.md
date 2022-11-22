---
title: 说明文档
description: '这是一个说明文档'
image: /imgs/default.jpg
tags:
  [
    '说明文档',
    'Markdown',
    'cpp',
    'js',
    '雷达',
    '开车',
    '太阳',
    '月亮',
    '游泳',
    '711',
  ]
category: 'c++'
published: '2022-08-02'
---

> 注意下面每一个标记如果和内容同行，中间都加一个空格

## 右侧会把##标题和###标题自动显示

### 我是###标题

# 这是一级标题

## 这是二级标题

### 一直到 3 级标题

#### 一直到 4 级标题

##### 一直到 5 级标题

## 列表

- 无序写法 1

* 无序写法 2

- 无序写法 3
  - 嵌套加一个 Tab
    - 再套一层
      - 再来

1. 有序列表只有这一种写法
2. 数字加点

## 表格

| 字段 1     |  字段 2  |     字段 3 |
| ---------- | :------: | ---------: |
| 内容       |   内容   |       内容 |
| 这列左对齐 | 这列居中 | 这列右对齐 |

## fengexian

---

---

---

---

---

---

注意：如果用---要和前方空行防止被当成标题符号

## 字体

_斜体 1_
_斜体 2_
**粗体**
**粗体 2**
**_斜粗体_**
**_斜粗体 2_**
~~删除线~~

## 超链接

[百度](https://www.baidu.com"百度一下，你就知道")

## 插入图片

![alt](https://res.cloudinary.com/redfern-web/image/upload/v1599840408/redfern-dev/png/nuxt.png)
<img src="/imgs/default.jpg" class="mx-auto" />
<img src="/imgs/yellow.webp" class="mx-auto"  />

## 引用

> 引用内容
>
> > 嵌套引用

## 代码块

`flag === true ? return alex : return tom`

```cpp
void main(int arg){
  int flag = 0;
}
```

## 这是一些图标

- 恐龙<icon name="konglong"></icon>
- 狗<icon name="dog"></icon>
- 飞船<icon name="feichuan"></icon>
- 星星<icon name="star"></icon>
- 星球<icon name="xingqiu"></icon>
- 可以给一个值 `icon-style="w-10"` 设置一个宽度,太阳<icon name="sun" icon-style="w-10"></icon>
- 月亮<icon name="moon"></icon>

- 文字<text-style size="text-3xl font-bold" color="text-red-500">自定义的文字</text-style>文字
- [颜色参考连接](https://windicss.org/utilities/general/colors.html)
- [字体大小](https://windicss.org/utilities/general/typography.html#font-size)
- [字体宽度](https://windicss.org/utilities/general/typography.html#font-weight)
