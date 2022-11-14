
### 环境配置
 - node `10.23.1`

依赖安装

```sh
$ npm install
```

### 构建

打包:

```sh
$ npm run build
```

开发:

```sh
$ npm run dev
```

访问:
 http://localhost:4000

添加插件:
修改根目录文件`book.json`,中的 `plugins`数组中添加插件名称, 再安装插件,手动把依赖插件添加到`package.json`以便后面自动初始化依赖使用

偶尔打包运行或部署提示文件不存在的错误:

修改`copyPluginAssets.js`文件中的`copyResources`方法
```js
confirm: false
```

### 资源
- [gitbook 文档](https://chrisniael.gitbooks.io/gitbook-documentation/content/format/configuration.html)
- [GitBook插件整理 - book.json配置](https://www.cnblogs.com/mingyue5826/p/10307051.html)