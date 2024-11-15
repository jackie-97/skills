文档主要编写一些工具，要给合适的操作选择合适的流程，才能事半功倍，很多时候你用错了工具

教程

- 图标制作
  - https://www.bilibili.com/video/BV1oz421z76X?spm_id_from=333.788.videopod.sections&vd_source=522153461914a766fc002cc8619314e4
- gui
  - https://www.bilibili.com/video/BV1tW2cYuEJ5/?spm_id_from=333.999.0.0&vd_source=522153461914a766fc002cc8619314e4
- ai绘图：https://www.bilibili.com/video/BV1nA411j7Ur?spm_id_from=333.788.videopod.episodes&vd_source=522153461914a766fc002cc8619314e4&p=2
- 图标



## typora

输入符号

- win+句号



## 网络

websocket

- 



## 微信开发工具

：一定要学会调试，不然出了问题你没法解决的，只能像无头苍蝇一样乱飞乱撞



[支持条件断点](https://xidicom.cn/tecnolgy/13/1513.html)

- 不然一个一个点要累死我了



## 像素画

：太秀了，像素画都有

教程

- https://www.bilibili.com/video/BV1bU4y127ZN/?spm_id_from=333.788.recommend_more_video.1&vd_source=522153461914a766fc002cc8619314e4
- 地图：https://www.bilibili.com/video/BV1xY411w7yf/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4
- https://www.bilibili.com/video/BV13841167t4?spm_id_from=333.788.videopod.sections&vd_source=522153461914a766fc002cc8619314e4



## spine

：一个骨骼动画制作软件，通过将图片绑定在骨骼上，组成一个整体，然后动起来

spine本身居然算一个工作岗位，神奇！工资还不低，可以考虑一下



优点

- 支持复用动作



关键问题

- 先做哪部分后做哪部分？
- 骨骼的创建、修改
- 什么时候要用事件？
- 怎样保证丝滑？
- 导出配置



#### 坑

- 试用版无法保存，所以我要找个破解版
- 练习时只做简单的东西，比如跑步、攻击
  - 复杂的、耗时的不做，比如头发、



#### 制作技巧

难的、耗时长的尽量不要做

- 

过滤内容：面板左上方有小按钮可以点

不要再设置里移动某个图片位置，而是应该在动画模式下看

网格与权重

- 左右手、脚的制作一般是一样的
  - 你做好了左手，那就可以直接拷贝给右手了

制作某个部位，比如手，

- 你可以隐藏掉其他的部位



#### 素材

怎么找？

- 官网
- 论坛
- qq群



#### 导入

快速导入，而且不会错位！

- 



#### 导出



#### 骨骼

常见

- 创建
- 修改
- 删除



#### 网格与权重

网格线需要卡着骨骼

注意不要乱加顶点

- 我怎么知道是不是乱加



#### 动画

：这是是骨骼动画的魂，也是最耗时的

需要总结一些套路

- 跑步是啥流程：先迈开一只腿，再迈开另一只腿
- 

常见动画

- 角色：攻击、受伤、死亡



## Shader

：着色器，用来渲染一些东西的

【【游戏开发基础知识】什么是Shader?】https://www.bilibili.com/video/BV1qZ4y1q7pm?vd_source=00d0076e0b5ba0c2aa292cd3450f564e

常用的shader：**HLSL**，unity也是用它



## TexturePacker

：用来合成，做成图集或者是精灵表（包含多个帧动作的图）

也可以用来预览动画

- 但是不能导出动画



## tilemap

关键

- 能否制作动画？
- 图层一般分几层？
  - grounds
  - walls
  - items：对象层
  - enemies：对象层
  - 


tilemap本身也可以做动画

tilemap动画制作：比如海水波动

- [godot内置了](https://www.bilibili.com/video/BV11v4y1Y7zu/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4)，不用外部软件
- 

教程

- 入门：https://www.youtube.com/watch?v=ZwaomOYGuYo&list=PLu4oc9P-ABcOXNOyoAvnMyUwn_kkiVA5B&ab_channel=Gamefromscratch

- 关卡制作：https://delightcollab.com/unity2d-tilemap-production-level/

- [地图制作](https://www.bilibili.com/video/BV17t42157si/?vd_source=522153461914a766fc002cc8619314e4)

- [动态地形](https://www.bilibili.com/video/BV1Gy4y1A7ae/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4)

如果很多尺寸都不一样，你要怎么弄？

- 其实没关系的

不知道为啥很多功能用不了

- 比如动画编辑器、碰撞编辑器

背景会动

- 

新建项目

- 直接建立再cocos里面



tiledmap中一般是使用一个对象层生成多个类型的物体，还是用多个对象层，每层生成一种物体？

- 简单的项目用一个对象层即可
- 复杂复杂项目则是用多个对象曾



#### cocos

- 导入地图失败
  - 需要导入对应的图片，不能只导入tmx文件
- cocos 导入tilemap空白区域为黑色，且无法修改，无法显示后面的视差背景
  - 可能是cocos不支持高版本的tilemap
  - 可能是我这个操作本身就无法实现
  - 也可能是我cocos其他配置覆盖了tilemap的颜色




快速制作地形

- https://www.bilibili.com/video/BV12s4y1q7Dj/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4

添加碰撞体

- 可以考虑只铺上薄薄一层
- 或者是摄像机移动到了再添加碰撞体
- 代码加一部分，然后自己手动再加一部分，比如地面



## 美术对接

常见

- 切图
- 图集制作
- 制作动画



#### 切图

：在线切图网站

- https://www.aigei.com/tool/sprite/split



- 
- 如果只有png不附带plist，要如何得到plist？
  - 可以用texturePacker
  - 有些软件还能够使用像素拆图，能够只要你精灵之间有空白即可


不规则的图集：一般是用tilemap来切割



#### 图集制作



#### 动画制作

**cocos**

到底是要图集还是要拆分后的多个张图片来制作动画？

- 要的是图集，但是要带有plist的

- 动画要用到图集，图集带plist文件才能被cocos正确解析成多张图片

如何批量调整帧间隔时间？

- 在轨道上c+a选中所有帧，然后设置“间隔数”，再右键“间隔排列关键帧”

采样帧率和播放速度以一般为多少

- 帧率60，速度为1





**godot**

- 直接就可以切割，不用第三方工具，直接拿图集即可，然后指定行列即可



怎样打包得到图集？

- 可以通过texturePicker打包得到

- 



#### 视差背景

cocos

- 是通过tilemap做
- 还是直接在cocos中拖放几张图片来做？



## 素材制作

ps

- 也能做，但是需要你掌握一些使用技巧还有拆分、缝合技巧

#### ai绘图

好处

- 可以快速制作满足要求的图片

缺点

- 需要电脑高配置或者是购买账号，我现在电脑跑不起来，

- 



## ui制作

- 

#### fgui

：大型项目里制作，小项目则是直接在引擎编辑器制作即可

教程

- https://www.bilibili.com/video/BV1zt411p7ZZ/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4



## ps

关键

- 掌握抠图、缝合技巧

