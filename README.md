# 3分钟搞定自己的MarkDown静态网站

## Build Setup

1. 新建仓库，取名为yourname.github.io

2. import本仓库
   - `https://github.com/kyoapps-kyo/nuxt-content.git`

3. clone一份到本地，项目中可能需要改动的文件
   ```js
    /utils
          |--------------  global.js //网站名称，社交账号等的设置
    nuxt.config.js                   //配置文件，需要改动的项目
          |--------------  publicRuntimeConfig.baseUrl:'https://yourname.github.io/'
          |--------------  head.titleTemplate//函数返回部分的标题请按自己的需求修改
    /content
          |-------------- /articles //存放md文件的目录，文件取名随自己的喜好，文件格式参照其中的文章
    /static
          |-------------- /imgs  //存放照片文件，可以多层文件嵌套，使用时按路径直接引用即可，'/imgs/***/***.**'
   ```

4. 仓库设置项
   - Settings -> Pages
   - Build and deployment -> Source
      - 选择 GitHub Actions
   - 完成

5. 回到本地仓库，git3连，有兴趣的话可以去仓库页面的Actions中看提交的详细输出，等待完成部署后即可拥有自己的网站

## content目录下md文件的一些些说明

- 说说最上面的几个属性

   1. title，文章的标题，页面的页首，可以通过title进行文章的查找
   2. description，文章简要说明，一样看过去，能知道这里写了个啥
   3. image，可选项 列表显示时，左侧展示的小图
   4. tags，可选项 文章的标签，可以有很多个，便于联想
   5. category， 文章种类，这将它作为笔记本来装多个文章，只能设置一个
   6. published， 发布时间，便于排序查找

- 其他的一些小图标，给字体设置样式等，在content的md文件中有具体用法
