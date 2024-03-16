# story painter

### 2.2.1 2024/03/16

* 新增: 将回复或@一类的消息格式，染色后呈现为@对应的玩家名称 - 星尘 (#16)

* 优化: 删除helloworld，添加反向代理测试，添加codemirror的type依赖 - dreamerFsboy (#13)

* 修复: 删除角色操作，点击取消后，对应的角色名字会被清空 - 星尘 (#16)


### 2.2.0 2024/01/06

* 新增: 转论坛代码“对单次发言，从次行进行空格缩进”功能

* 新增: 转论坛代码“使用颜色名，而非16进制颜色码”功能，兼容不同论坛

* 优化: 安全性增强

* 修复: 如果一条发言有换行，点一键复制，此条发言的几行会粘连在一块。正确情况是粘贴出来也是多行。影响转论坛代码和回声工坊

* 其他: 更新回声工坊链接为2.0版本介绍视频


### 2.1.2 2023/04/08

* 优化: ..开头的文本不再被视为指令，只有单个.或。或/开头才是

* 修复: 修复了句中有()时被场外发言过滤筛掉的错误情况


### 2.1.1 2023/03/25

* 优化: 对缩进进行了调整 #9


### 2.1.0 2023/03/25

* 新增: 增加一个Importor用于导入染色好的文本，即 RenderedLogImporter #2

* 新增: 增加一个Importor用于导入fvtt的log #4

* 优化: 更换取色器 #5

* 优化: 建立“名字 : 颜色”的浏览器缓存，同名角色第二次访问保持颜色不变 #6

* 修复: QQ聊天窗口直接复制文本到染色器，预览时时间信息丢失 #3

* 修复: 如果为场外发言前做了@或回复，将不会被识别，如 [CQ:at,qq=12345]（场外发言 #1

* 修复: 单张图片发言预览时被吃掉问题


### 2.0.6 2023/01/23

* 增强了对赵骰log的兼容性(某版本发言条的句末会带一个空格)


### 2.0.5 2023/01/23

* 修复编辑异常


### 2.0.4 2023/01/22

* 修复了场外发言指令过滤导致的预览显示错误，并因为修改实现方式又提升了一点预览页面的性能

* 处理了因为@别人或者发的图片被过滤掉，导致的预览首行空白情况

* 可能解决了iOS/safari上改名弹出两次的问题


### 2.0.3 2023/01/22

* 修复了角色改名部分一个潜在的xsrf问题

* 修正了改角色名后按回车，点击确定后改不了名的问题(只有按回车受影响)

* 导出时的CQ码过滤补完


### 2.0.2 2023/01/21

* 修复了少部分log的角色名乱码问题

* 缩短帐号部分以更好适配移动端


### 2.0.1 2023/01/21

* dice!默认格式支持优化

* 全选替换现在会自动清除角色列表


### 2.0.0 2023/01/20

* 重构核心代码

* 极大提升性能，实现了5w行log预览的秒级加载，可能是目前最快的染色器。

* 完善了删除角色和角色改名


### 1.0.8

* 支持了带空格的名字、带/的名字、带括号的名字

* 修复QQ/IRC风格聊天记录导出出现\<br />问题

* 修复QQ聊天记录有部分不支持问题

* 修正了回声工坊coc日志的ra检定检定值和出目顺序颠倒的问题

