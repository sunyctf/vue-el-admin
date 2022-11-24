# vue+element单页面电商后台管理系统
### 介绍

- vue-el-admin是一个单页面电商网站后台管理系统，基于 [vue](https://github.com/vuejs/vue) 和 [element](https://github.com/ElemeFE/element)。它使用了最新的前端技术栈，内置动态路由，导航菜单渲染，权限验证等，提炼了典型的业务模型，用户UI界面干净整洁。

- **完整版**

  [Github仓库](https://github.com/sunyctf/vue-el-admin) | [预览地址](https://sunyctf.github.io/vue-el-admin)
  
  [码云仓库](https://gitee.com/sunyctf/vue-el-admin) | [预览地址](https://sunyctf.gitee.io/vue-el-admin)

### 前序准备

你需要在本地安装 [node](http://nodejs.org/) 和 [git](https://git-scm.com/)。本项目技术栈基于 [ES2015+](http://es6.ruanyifeng.com/)、[vue](https://cn.vuejs.org/index.html)、[vuex](https://vuex.vuejs.org/zh-cn/)、[vue-router](https://router.vuejs.org/zh-cn/) 、[axios](https://github.com/axios/axios) 和 [element-ui](https://github.com/ElemeFE/element)，提前了解和学习这些知识会对使用本项目有很大的帮助。

### 软件架构

软件架构说明

### 安装教程

#### 开发

- **克隆项目**

```bash
git clone https://github.com/sunyctf/vue-el-admin.git  # clone the project
```

- **进入项目**

```bash
cd vue-admin-template # enter the project directory
```

- **安装依赖**

```bash
yarn install # install dependency
```

- **运行项目**

```bash
yarn run serve # Compiles and hot-reloads for development
```

#### 发布

- **打包测试**

```bash
yarn run build:test # Packaging test
```

- **正式打包**

```bash
yarn run build # Compiles and minifies for production
```

- **运行测试单元**

```bash
yarn run test # Run your tests
```

- **格式化代码**

```bash
yarn run lint # Lints and fixes files ——代码格式检查并自动修复(规范代码)
```

### 演示

- username: admin  |  password: 任意
- username: editor  |  password: 任意

### 其他注意事项

#### SVG

##### 安装

```bash
npm i -D vue-svg-loader vue-template-compiler
```

##### 修改配置

```javascript
// vue.config.js
module.exports = {
  chainWebpack: (config) => {
    const svgRule = config.module.rule('svg');
 
    svgRule.uses.clear();
 
    svgRule
      .use('babel-loader')
      .loader('babel-loader')
      .end()
      .use('vue-svg-loader')
      .loader('vue-svg-loader');
  },
}
```

##### 使用

```javascript
<script>
import daiban from '@/assets/icon/daiban.svg'
export default {
    components:{
        daiban
    }
}
</script>
```

##### 修该颜色

```css
/* 删除SVG文件中的 fill */
.index-head-centent-right-list-icon-is{
    color: #F515EA !important;
    width: 20px;
    height: 22px;
    fill: currentColor;   /* 重点 */
}
```
### 使用说明

1.  xxxx
2.  xxxx
3.  xxxx

### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request


### 特技

1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
2.  GitHub 官方博客 [blog.github.com](https://github.blog)
3.  你可以 [https://github.com/explore](https://github.com/explore) 这个地址来了解 GitHub 上的优秀开源项目
4.  GitHub官方提供的使用手册 [https://docs.github.com/cn](https://docs.github.com/cn)
5.  GitHub中文社区 https://www.githubs.cn/
