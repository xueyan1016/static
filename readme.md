## 开放静态文件 CDN

> URL: [StaticFile.org](http://staticfile.org)

### 一、背景和目标

像 Google Ajax Library，Microsoft ASP.net CDN，SAE，Baidu，Upyun 等 CDN 上都免费提供的 JS 库的存储，但使用起来却都有些局限，因为他们只提供了部分 JS 库。当然，我们还可以有像 CDNJS 这样的平台，存储了大部分主流的 JS 库，甚至 CSS、image 和 swf，但国内的访问速度却不是很理想，并且缺少很多国内优秀开源库。

因此，我们提供这样一个仓库，让他尽可能全面收录优秀的开源库，并为之提供免费 CDN 服务。使之有更好的访问速度和稳定的环境。并提供开源库源接入的入口，让所有人都可以提交开源库，包括 JS、CSS、image 和 swf 等静态文件。


### 二、如何提交开源库

Fork 这个仓库，新建一个开源库的目录，这个目录下可以有多个版本的目录（至少一个版本目录）如：

```
.
├── jquery
│   ├── 1.8.3
│       └── jquery.min.js
│   ├── 1.9.1
│       └── jquery.min.js
└── package.json
```


编辑 package.json 描述文件，这个文件描述最新版本的信息。具体写法请参照：[https://npmjs.org/doc/json.html]()。

然后给这个仓库提交 Pull Request。理论上我们会用最快的速度验证、审核这个库。一旦 Pull Request 被 Merge，则马上可以能过 CDN 访问。


### 三、更新开源库

理论让我们自动更新库的版本文件，并且不会删除旧版本，但如果你在 [Static File](http://staticfile.org) 找不到最新的版本，则可以通过提供多一个版本目录，并且修改 package.json 文件，利用 Pull Request 来提醒我们。
|

### 四、作者和服务商

此仓库由 [Sofish](https://github.com/sofish)、[hfcorriez](https://github.com/hfcorriez) 和 [ikbear](https://github.com/ikbear) 更新和维护。由国内优秀的 CDN 服务商 [七牛存储](http://www.qiniutek.com/) 提供。


### 五、开源协议

仓库基于 MIT License 开源

### 六、感谢

国外源更新自 [CDN JS](http://cdn.js)，多谢他们做出这么多的努力。