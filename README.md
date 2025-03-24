# Live2D-Custom-Widget

## live2d说明
- Live2D 是一种先进的二维动画渲染技术，由日本 Cybernoids 公司开发，广泛应用于电子游戏、动画制作以及各类交互式应用中。它能够为静态的 2D 图像赋予流畅的动态效果，使角色表现更加生动，极大地提升了视觉体验和互动感。Live2D Cubism 通过变形网格（Deform Mesh）技术，将 2D 图像分割成多个可独立变形的部分（如眼睛、嘴巴、头发等）。每个部分可以通过参数控制进行旋转、缩放、拉伸、扭曲等操作，从而创建流畅的动画效果。例如，角色的头部转动可以通过调整多个网格的形变来实现，模拟出接近 3D 的立体效果，而无需使用 3D 建模。
- Live2D 技术主要包括两个分支：Cubism 和 Euclid。其中，Cubism 是当前的主流版本，被广泛用于游戏开发、虚拟主播、互动式内容创作等领域，而 Euclid 分支则已停止开发。因此，通常提及 Live2D 时，一般指的是 Cubism。


## 如何在前端网页实现live2d的动态效果？
~~1. 懒人方法~~
### 2. 本地化资源
- 先把assets文件夹下，内包含三个文件，assets文件夹和你的网页首页index.html同一级目录（当然，也可以不同目录，修改下面代码的路径即可）
- 在index.html中插入以下代码
1. 在文件头部<head>标签内引入css样式
```js
    <link rel="stylesheet" href="/assets/live2d/css/live2d.css" />
    <link rel="stylesheet" href="/assets/live2d/css/waifu.css" />
```
2. 在文件尾部<body>标签内引入js及初始化Live2d
```js
    <script type="text/javascript" src="/assets/live2d/js/jquery.min.js"></script>
    <script type="text/javascript" src="/assets/live2d/js/live2d.js"></script>
    <script type="text/javascript" src="/assets/live2d/js/waifu-tips.js"></script>
    <script type="text/javascript">
    initWidget({
        waifuPath: "/assets/live2d/waifu.json",
        cdnPath: "/assets/live2d/"
    });
    </script>
```
## 效果展示
![alt text](/images/image.png)

## 功能修改介绍
1. 模型现包括聊天、换模型、拍照、关闭模型
2. 更换功能图标
3. ...

## 埋个坑
- 更新全局方法
- 接入好玩的api
- 电脑桌面版本
- 参考MakeS游戏设计思路
- ...

## bug清单
- 增加手机检测自动收起模型
- 模型对于鼠标反馈问题
- 母版网页修改模型，配色
