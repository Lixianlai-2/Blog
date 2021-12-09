## 用 left 制作从左到右的动画

![从左到右](img/从左到右的代码.png)
![不断渲染](img/不停渲染.gif)

#### 原理

- 每过一段时间（用 setInterval)
- 将 div 移动一小段距离，直到移动到目标地点

#### 注意性能

- 绿色表示重新绘制
- CSS 渲染过程一次包含了布局、绘制、合成
- 其中布局和绘制有可能被省略

#### 打开 rendering 查看渲染过程

- ![](img/rendering1.png)
- ![](img/rendering2.png)
- ![](img/rendering3.png)

## 浏览器的渲染原理

#### 参考文章

- []()

#### 查看 CSS 各属性触发什么

- []()

## 浏览器渲染过程

#### 步骤

- 将 HTML 构建成 HTML 书（DOM）
- 将 CSS 构建成 CSS 树（CSSDOM）
- 将两棵树合并成一棵渲染树（render tree)
- Layout 布局（文档流、盒模型、计算大小和位置）
- Paint 绘制（把边框颜色、文字颜色、阴影等画出来）
