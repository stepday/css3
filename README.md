# css3
搜集和整理css3.0的一些新特性

## flex
- flex是这一种新型的布局方式 类似于block、inline-block 让布局变得更简单
- 采用flex布局的元素被称为容器，所有子元素被称为成员（flex item)

![图片描述](https://img-blog.csdn.net/20160706144733310)

### 容器的属性
> flex-direction 决定主轴的方向，有四个值:
- row:主轴为水平方向，起点在容器的左端
- row-reverse:主轴为水平方向 起点在容器的右端
- column:主轴为垂直方向，起点在容器的上沿
- column-reverse:主轴为垂直方向，起点在容器的下沿

> flex-wrap 一行排不下 如何换行的设置
- nowrap: 不换行
- wrap:换行 第一行在上方
- wrap-reverse:换行，第一行在下方

> flex-flow  是flex-direction 和flex-wrap属性的简写形式
- 比如：flex-flow:row nowrap

> justify-content 设置项目在主轴上的对齐方式 有5个值
- flex-start: 向主轴的起始位置对齐
- flex-end:向主轴的结束位置对齐
- center:居中
- space-between: 项目之间的间隔均等 如果只有两个项目 则一边一个
- space-around:每个项目两侧的间隔相等

> align-items 设置项目的交叉轴上如何对齐
- flex-start: 交叉轴的起点对齐
- flex-end:交叉轴的终点对齐
- center:交叉轴的终点对齐
- baseline:项目第一行文字的基线对齐
- stretch:默认值 若项目未设置高度或设为auto 将占满整个容器的高度

> align-content 定义了多根轴线的对齐方式 如果项目只有一行/一列 则不起作用
- stretch: 默认值 多行占满整个交叉轴
- flex-start: 与交叉轴的起点对齐
- flex-end:与交叉轴的重点对齐
- center:与交叉轴的中点对齐
- space-between:与交叉轴两端对齐 轴线之间的间隔平均分布
- space-around: 每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍

### 项目的属性
> order 排列顺序 数值越小越靠前 默认为0

> flex-grow 定义项目的放大比例 默认为0

> flex-shrink 定义项目的缩小比例 默认为1

> flex-basis 占据主轴空间的大小 默认值为auto

> flex 是flex-grow flex-shrink flex-basis 的简写 默认为 0 1 auto

> align-self 允许单个项目与其他项目不一样的对齐方式 可覆盖align-items属性。默认值为auto，表示继承父元素的align-items属性，如果没有父元素，则等同于stretch

### 参考资料
[点这里](https://www.cnblogs.com/cblx/p/8976309.html)