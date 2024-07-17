快捷打开： https://github1s.com/facebook/react
源码部分放在packages目录下，主要看react，react-dom文件夹

源码目录笔记：
![1721061774987](image/01_怎么高效读react源码/1721061774987.png)

## 调试react源码

### 方式一

调试源码拉取最新的react代码

* 执行yarn
* 打包react、scheduler、react-dom

```
# 执行打包命令
yarn build react/index,react/jsx,react-dom/index,scheduler --type=NODE
# 申明react指向
cd build/node_modules/react
yarn link
cd build/node_modules/react-dom

# 申明react-dom指向

yarn link
```



## 方式二

利用 webpack 的 alias 将 react、react-dom 等库指向到源码文件，但是直接使用源码。

##### 创建react项目

[React 之如何调试源码 - 掘金 (juejin.cn)](https://juejin.cn/post/7168821587251036167#heading-8)

运行测试用例

看源码工具：

Bookmark
