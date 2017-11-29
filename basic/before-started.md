
## 参考文章
 - [awesome-mobx](https://github.com/mobxjs/awesome-mobx/blob/master/README-CN.md)：很不错的 MobX 相关资源整合

## 准备
如何阅读源码，建议先从官方提供的[样例](https://github.com/mobxjs/awesome-mobx#example-projects)开始阅读，我这里挑选 [mobx-examples](https://github.com/mobxjs/mobx-examples) 这个官方提供最简单的 ES5 系列，之所以选择它，是因为它足够的简单、精简，没有涉及到 JSX、Babel 的预编译，利于学习 mobx 的核心概念；

我们就选第一个例子：

![autorun](https://ws4.sinaimg.cn/large/006tKfTcgy1fhqe46q4ltj30fv07mdgs.jpg)

我们将 `index.html` 中的 **mobx.umd.min.js** 修改成 **mobx.umd.js** ，方便直接调试源码：

![源码](https://ws1.sinaimg.cn/large/006tKfTcgy1fhqe4v6hxmj30qz0alta6.jpg)

然后在浏览器打开这个 `index.html` 文件，然后在 `demo.js` 中打断点：
![打断点](https://ws2.sinaimg.cn/large/006tKfTcgy1fhqe6yd2zej30n107kq4p.jpg)

另一方面直接将 [源码 (v3.1.2)](https://unpkg.com/mobx@3.1.2/lib/mobx.umd.js) 拷贝放到编辑器中，我们挨个解释其中的内容；

> 如无特殊说明，所有的代码解释都是基于 V3.1.2 版本

好了，准备工作完毕，开启源码阅读之旅吧；