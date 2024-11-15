教程

- 论坛
  - [官方文档](https://docs.godotengine.org/zh-cn/4.x/about/introduction.html#before-you-start)
  - 去qq问一下知道的人，我目前只找到掘金，其他都是没人的
- 入门
  - [大全](https://www.bilibili.com/video/BV1C64y1h71j?p=7)
  - https://www.bilibili.com/video/BV14Y411h7Po?p=38&vd_source=522153461914a766fc002cc8619314e4
- 各种插件：一般找awesomexxx的即可
  - [awesome](https://github.com/godotengine/awesome-godot)
  - [5大插件](https://www.bilibili.com/video/BV1Z1421r79y/?vd_source=522153461914a766fc002cc8619314e4)
- [gdscript](https://docs.godotengine.org/zh-cn/4.x/tutorials/scripting/gdscript/gdscript_basics.html)
- [godot更新](https://www.bilibili.com/video/BV1GepSeVE3t/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4)
- 使用感受
  - https://www.bilibili.com/video/BV1yh411k783/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4

- [godot看法](https://www.bilibili.com/video/BV1oF41127yy/?spm_id_from=333.999.0.0&vd_source=522153461914a766fc002cc8619314e4)
- godot独立游戏
  - [十大游戏](https://www.bilibili.com/video/BV1nD42177iq/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4)



## 关键问题

#### 学习计划

- [ ] 看完入门80集：8h
  - 当前进度：第20集

- [ ] 模仿跳跃游戏教程：10h
- [ ] 



优缺点分析

- 缺点

  - 很少工作岗位
  - 很少中文教程
  - 3d比较拉跨
- 优点

  - 2d市场的王者，生态良好，有很多插件和示例项目
  - 开发效率高，适合独立游戏开发者
  - 

使用策略

- 适合使用了其他引擎，然后再转godot
- 优先使用gdscript，大多数答案也是这个语言的
- 但是我如果学了c#

学习项目在哪里

- 





#### 技巧

position.x可以直接修改

碰撞体必须挂载在刚体下面

- 

引入物理引擎的物体，比如刚体

- 就不要去直接控制它的位置了，而是要施加力或者是控制速度



## 坑

官方文档居然没有搜索功能

- 

- 

卡迪尔坐标系，原点在左下角，y轴是向上的

- godot的坐标系不是笛卡尔类型，原点在左上角，y轴是向下的

不添加碰撞体，刚体居然无法发生碰撞

- 而且它的碰撞组是在刚体里配置的，而不是在碰撞体里面配置

定时器不生效了

- 你没设置自动启动，autoStart



#### gdcript

- 定时器居然要独立创建，并且要手动连接
  - 而且不利于阅读
- 居然没有三目运算符
  - 只能写ifelse
- 运算符
  - 没有switch、case，而是match
- 比如定时器绑定的节点
- 变量命名不能有中划线，我喜欢中划线啊
- 只能直接移除某个子节点，而不是直接移除某个孙节点



- 

变量不能赋值给常量

- 神经，居然只能赋值给变量





#### 编辑器

不支持多开项目

节点面板是指节点有关的属性，而不是里面全是节点

连接一定要通过编辑器操作吗？能否直接用代码实现连接

- 一定要连接，不然直接写代码是无效的

软件里无法搜索插件，一直提示无法联网

- godot代理配置的问题你修改一下即可

搜索功能很慢

- 



## 插件

分为：编辑器插件和项目插件

常用插件

- [对话插件](https://godotengine.org/asset-library/asset/833)

godot插件需要每个项目都重新导入一遍吗？





## 场景

场景与节点的关系

- 我的理解是场景是节点的容器，场景可以实例化，节点不能脱离场景起作用

怎么切换场景？

- 通过文件系统点击tscn
- 或者是再场景栏中切换场景





## 节点

常见crd

- 添加
  - add_child
  
- 获取
  - get_node，支持动态，支持找兄弟节点，不过要先..，如../sp2，找到sp1的兄弟
  - $xxx，这种是写死的，而且只能找子节点，如$sp1,$sp1/sp2，无法找到兄弟节点

- 删除
  - 移除节点：remove_child只是从节点树上移除了，不删除
  - 删除节点，推荐：node.queue_free



实例化对象用new方法，而不是关键字

- Sprite.new()



## 脚本

一个节点只能挂载一个脚本

被连接对象必须提前配置脚本

- 



#### 输入

直接监听即可，用II，如Input.is_action_pressed

- 在input函数中检测，而不是在process中监听
- 



## 定时器



## 坐标系

a指向b：a.position.direction_to(b.position)，这算出来只是方向，没有速度，速度要自己指定，

- 获取长度：length
- 获取距离：a.distance_to(b)

## 物理系统

#### 刚体

刚体与碰撞体节点一般是父子关系，而cocos则是兄弟关系

力

- 一次性的力：apply_force
- 恒定力：add_constant_force



move_and_slide与move_and_collide

- 前者是继续滑动，常用于角色控制，比如撞到墙了，然后还要能够继续走动，斜着走或者是蹲着走
  - 这个只有角色刚体才有，其他没法用这个函数
- 后者则是立即停止
  - 

#### 碰撞体





不能向量x向量，只能是标量x向量

怎样判断是否发生了碰撞？

- 



#### Area2D

：能够检测物体进入、退出这个区域



## 输入





## GUI

：图形化用户界面

一般是容器来控制元素的布局

- 元素本身也可以调整它在父容器中的定位

容器分类

- 居中
- 横向
- 纵向
- 流动
- 网格
- 还有margin



## 插件

[大全](https://www.bilibili.com/video/BV1RH4y1c7E9/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4)

它的插件居然不显示下载量

- 傻逼玩意来着的，



## 问题

开发方式

- 脚本
- 拖拽



生命周期：irp

- 



语法

- 函数：用冒号和pass
- 

图片本身就是纹理的一种

- 

推荐按场景给文件进行分类

