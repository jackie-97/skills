这个文档只在我学习阶段补充，在做项目的时候只写另一个文档

教程

- 学习路线？？？
  - https://www.cnblogs.com/bycw/p/17843263.html
  
- 论坛

  - 官网：[Cocos Creator 3.8 API - Tween](https://docs.cocos.com/creator/3.8/api/zh/class/Tween)

  - 掘金：https://juejin.cn/user/1972988307323236

- awesome

- up主推荐
  - [程序员长风的个人空间-程序员长风个人主页-哔哩哔哩视频 (bilibili.com)](https://space.bilibili.com/50743344/?spm_id_from=333.999.0.0)
  - 列表：https://forum.cocos.org/about
  - 
  
- 关卡设计
  - [如何设计好玩的游戏关卡？四个原则打造极致体验_单机游戏热门视频 (bilibili.com)](https://www.bilibili.com/video/BV14H4y1z7ar/?spm_id_from=333.999.0.0&vd_source=522153461914a766fc002cc8619314e4)

- 学习路线
  - [游戏开发学习路线推荐_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1Ms421A7fp/?spm_id_from=333.788&vd_source=522153461914a766fc002cc8619314e4)

  

## 关键问题





#### 注意事项

- 每天的学习都要确保有足够的时间来实践和消化所学内容。
- 不要忘记休息和避免疲劳。
- 如果某个主题需要更多时间，可以适当调整计划。

请记住，这个计划是紧凑的，每天 8 小时的学习需要高度的专注和投入。确保你有足够的休息和适当的休息时间来保持效率。



## 坑

为啥教程这么少？https://forum.cocos.org/t/topic/152443

unity的威胁：https://forum.cocos.org/t/topic/152124

- cocos要凉了，能转就快点转

https://forum.cocos.org/t/topic/131360

- 

编辑器跟屎一样

- 老是不更新视图

论坛也跟屎一样

- 永远只有入门问题

没有多少实用demo，官方也不出，社区也不出

- 严重阻碍学习效率

- 




## 技巧

要找一下面试题，才知道重点在哪里

观察一下别人是怎么用 ai 写代码的，模仿是最快的学习方式，前提是找对老师

- 

显示控制与逻辑控制分离

- 

快捷键

- 展开、折叠：左右方向键
- 打开面板：ctrl+1、2、4

出现报错多去官网、github搜一下

- 记得关键字要选对，不然没法搜到问题



## 编辑器

热更新啥时候生效？

- 我说的热跟新是本地的行为

如何控制场景视角？

组件的配置可以重置

相机参数

- 滚轮：0.8
- 漫游：50

如何减少我切换页面的次数

- 我希望修改完脚本后，直接切换到浏览器，就能看到效果
  - 目前是需要切换回 cocos

为啥会有红色的线框？

- 把场景删除

为啥画布尺寸这么小？

怎样统一调整画布大小？

属性编辑器

- 上锁的，是无法编辑，还是开锁后编辑



不是所有的节点都能添加帧动画

- 必须是有 sprite 组件的节点才能添加帧动画，而且一个动画组件可以有多个帧动画

快捷键

- 

添加帧动画

- 先创建带精灵的节点
- 再添加动画组件
- 再创建帧动画
- 
- 拖一下就会打一帧，不用选中



卡死问题

- 重启搞定
- 或者是等一下



老是弹窗：参考图

- 把右上角的参考图开关关掉
- 很多问题，你问 ai 它就能帮你回答咯



开发阶段热更新

：他们讨论的好像是线上热更新



刷新属性面板

- 右上角有刷新按钮

如何移动场景编辑器视角？

- 通过右键，然后移动方向盘
- 能够移动，但是不会保存，移动一下其他面板又会收到影响

场景编辑器有运行时刷新功能？或者是重启项目

- 

为啥你妈的谷歌浏览器预览时需要先切到 cocos，才会触发自动编译，你自己检测到修改了重新编译不就好了？

- 

#### 场景编辑器

刚体

- 删除节点：ctrl+点击
- 移动节点
- 

视角怎么调？

- 按1比1显示为啥没有快捷键？

视图模式

- 你要切换到2d模式，妈的之前一直在3d模式下看着

怎么快速选中场景，不通过双击的方式？我讨厌双击

- alt+f实现双击效果





#### 动画编辑器

添加帧

修改属性

- 

批量操作

- 还可以批量选中、拷贝、删除



空指针问题

- 可能是项目内存分配的设置太小了，改一下即可：https://forum.cocos.org/t/topic/138971/4
- 



有没有切图的功能？

- 



## 资源管理

场景与资源的关系

- 场景是资源的一种。
- 场景是容器，一个游戏是由很多场景组成

教程：[Asset Manager 概述 | Cocos Creator](https://docs.cocos.com/creator/3.8/manual/zh/asset/asset-manager.html#加载管线)



#### 资源加载

load 和 preload 都是异步的





#### 图像



#### 字体







#### 音频

播放、暂停、恢复、停止

方式

- 音乐组件
- 音乐引擎

播放

- 一般是跟按键绑定的，比如攻击、防御

通过获取组件的方式来控制播放、暂停

- play
- pause



#### 预制体

：相当于前端组件，是为了提高复用性，降低维护成本，有预制体资源、预制体实例

预制体本质上就是一个预先创建的节点对象

为啥保存预制体时总是弹出一个参考图弹窗

- 

场景

- 大量重复对象：子弹、敌人、金币

制作流程

- 先创建节点，设置一下精灵，初始位置，大小
- 然后再设置为预制体
- 更新



获取预制体

- 通过引用，然后拖拽赋值
- 通过 load 方法

在预制体中依赖另一个节点，如何定义获取？

- 

#### asset bundle

关注点

- 包的划分
- 构建
- 获取
- 删除

:smiley:

什么时候需要分一个包

资源包的获取

- 

bundle对象的获取

- assetManager.getBundle

怎么判断全部资源都参与打包了？

怎样避免重复加载？

- assetManager.getBundle

bundle.load方法



#### 管线

：其实就是一个串联组合



- 







## 场景

一个游戏里由多个场景，一个场景就是一个界面、一个关卡

场景是特殊的一种资源

常见操作

- 动态加载：
- 预加载



#### 坐标

使用哪种坐标？

- 一般使用本地坐标
- 除了相机、碰撞相关的，使用世界坐标

原点在左下角

- 



#### 节点

：只是容器

节点本身的操作

- crd 操作，添加、获取、销毁操作
  - 查找：查找子节点、全局查找
    - find
    - getChildByName
    - 
- 变换：移动、旋转、缩放
  - 移动：通过指定目标点、增量
    - setPosition、node.position、node.position.x
    - translate：相对于当前位置
    - 
- 激活
- 可见性
  - 通过node.active=false


基于关系的操作

- 获取、设置、移除父子节点
  - 索引来获取



层级管理器中的是否建立了父子节点关系？

- 会



监听节点事件

- on、off

节点上只能绑定一些常规事件，比如暂停，恢复

- 

layer

：决定了节点是否能被相机看见

子节点默认继承父节点的layer





## 组件



常见操作

- crd组件
- 控制组件的执行顺序

为啥要控制组件的执行顺序？

- 因为某些组件依赖于其他组件



#### 渲染组件

**sprite 组件**

- 设置 sprite 组件大小




#### ui 组件

与节点关系：组件负责功能，节点负责容器

与渲染组件的区别

- 渲染组件受到光照、阴影的影响
- ui 组件不会

组件与节点的关系：多对一关系

与 2d 组件有啥区别？

- 

获取组件 getComponent，

拿到节点往往还不够，你要还要拿到对应的组件

- 



button



#### 其他组件

camera





## 脚本

**生命周期**

：lsu



**事件**

常用的是触摸事件

- 



一个游戏既要在 pc 端运行，又要在移动端运行

- 应该绑定触摸事件，而不是鼠标事件，这样可以保证兼容性

systemEvent

- 



## 动画系统

为啥叫缓动？

- 不是表示移动的慢，而是表示动画流畅

不写一行代码或少量代码，通过 cocos 的配置来实现动画

动画剪辑

- 

关键帧动画

- 怎样保证流畅？
  - 需要上一个帧和下一个帧的头几乎在同一位置，不要偏差太远，产生不连贯的感觉
  - 飞机大战的，保证连贯是通过修改锚点位置来保证头连贯

要掌握一些动画技巧

- 很多角色都有动画的



#### 帧动画

记得要先加入帧组件cai'xing

怎样快速制作帧动画？

- 通过选中一批图片然后拖入就可以完成批量插入咯

怎样快速调整帧间隔？

- 



#### 骨骼动画

：看spine那块

做骨骼动画能做很多很有意思的事情，不如跑步，跳跃，攻击，防御，受伤，

- 更加流畅



## 缓动系统

：为啥叫缓动，它想表达丝滑的意思

与动画系统相反，是纯代码，





## 粒子系统

：用来做特效的，可以模拟水、火、烟、云、雪

关注点

- 粒子资源文件制作
  - 由美术或美工来做
- 粒子属性、方法
  - stopSystem
  - resetSystem

首先考虑做一个奔跑烟尘的练练手

- 



## shader

https://forum.cocos.org/t/topic/153452

可以用于实现光影、粒子、材质效果











## 物理系统

：也叫物理引擎，分 buildin-2d 和 box-2d，前者只支持简单的碰撞检测，后者支持更多，主要用box-2d

#### 刚体

：主要



#### 碰撞体

是否发生碰撞取决于碰撞体的分组，而不是刚体的分组

实操发现碰撞体的中心点没有跟随节点的锚点

- 一直在左下角



offset是设置距离锚点的位置，如果锚点默认是在左下角，那么你就需要

- 

锚点就是节点的中心点，但是不一定在节点的中心位置

- 节点的移动、缩放都是依靠这个
- 锚点



#### 碰撞检测

我 2d 游戏可以用 3d 的碰撞检测？





## 插件

：基本没有，cocos社区跟坟场一样



- 



## 数据存储

好处

- 简化开发流程，方便你做一些模拟
- 保存进度
- 



- 





## 性能分析&优化

https://www.bilibili.com/video/BV1TC411G7Gz/?spm_id_from=333.999.list.card_archive.click&vd_source=522153461914a766fc002cc8619314e4



## 相机

：我们最终看到的游戏效果是一个或多个相机叠加的结果！

多相机

：他们的visibility可以交叉，比如default、

画布本身没有层级的概念

- 只是为了方便快速修改它子节点的层级

相机的几个参数不了解

- Priority：值越大，越显示越靠前，能覆盖后面的
- clear flags：需要清除哪些缓冲，一般选清除深度缓冲即可
- clear color: 相机颜色缓冲默认值
- clear depth: 深度缓冲默认值



## 适配

https://www.cnblogs.com/gamedaybyday/p/12069570.html



## 广告接入

分微信、抖音

教程

- https://www.bilibili.com/video/BV1Ja4y1T7bh/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4



- 



## 游戏框架



关键

- 框架能做啥东西？
- 怎么找？
- 怎么学习？
- 怎么做自己的框架？
- 



教程

- 前端开发框架：https://forum.cocos.org/t/topic/150588
- puremvc：
- https://forum.cocos.org/t/topic/100941
- https://forum.cocos.org/t/topic/100942
- https://forum.cocos.org/t/topic/137215/12



## 问题

游戏引擎是啥？

- 为游戏开发提供了核心的功能，让开发者不必从 0 开始写代码，更加专注业务

场景

- 里面有很多节点，自带的是自然光和摄影机，还有自定义节点



编辑器的使用

- 如何移动视野
- 如何基于节点移动视野
- 如何移动节点

节点与组件有区别？

- 节点是容器，组件必须挂载到组件上，不能单独存在

为啥场景编辑器不能看到画面？

怎么评估性能好坏，

- 如果没法评估，你就没法做针对性的优化

- 

加注解是为了可以在编辑器里配置

- 

一帧对应一张图片，一帧占据的时间 = 1/fps，fps 即帧率

- 帧率越高，动画越流畅，帧率越低，越不连贯，越卡顿

2d 对象与 ui 组件有啥区别？

- 

res 与 resources 区别：

- resources 放需要动态加载的资源

物理引擎主要做了啥？

：不用你写很多判断了，它直接告诉你答案

- 检测碰撞，
- 刚体力学，能进行受力分析

鼠标、键盘的监听

- 通过 Input 这个类

我怎么知道要有多少个场景？

- 一般是一个新关卡就要一个新场景

什么时候需要新建节点？

- 

物理引擎的开启时全局的吗？还是可以一个场景开启一个？

- 

怎么让游戏角色移动？

- 移动角色
- 移动背景



sdk 就是第三方包，相当于npm包

- 可以减少开发者的工作量，同时减少出错率，统一标准
- 玩家也可以有更好的体验



bundle管理

- 

原点

- 

精灵与纹理区别

- 会动的才是精灵
- 不会动的是纹理



节点所处位置与节点的layer对于渲染顺序的影响，哪个优先级更高？

- 先看layer
- 再看位置



