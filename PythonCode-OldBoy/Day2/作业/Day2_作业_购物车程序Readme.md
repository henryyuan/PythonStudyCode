### 此Readme文档是针对编写的购物车程序的说明


### 程序基本信息

- 作者：zengchuixin
- 日期：2017/07/16
- 版本：Version 1.0
- 工具：PyCharm 2017.1.4
- 版本：Python 3.5
- MarkDown工具：HBuilder
- 流程图工具：ProcessOn

### 程序要求

- 启动程序后，输入用户名密码后，如果是第一次登录，让用户输入工资，然后打印商品列表
- 允许用户根据商品编号购买商品
- 用户选择商品后，检测余额是否够，够就直接扣款，不够就提醒 
- 可随时退出，退出时，打印已购买商品和余额
- 在用户使用过程中， 关键输出，如余额，商品已加入购物车等消息，需高亮显示
- 用户下一次登录后，输入用户名密码，直接回到上次的状态，即上次消费的余额什么的还是那些，再次登录可继续购买
- 允许查询之前的消费记录

### 程序相关文档

- GitHub,[ChuixinZeng-Python笔记主页](https://github.com/ChuixinZeng/PythonStudyCode/tree/master/PythonCode-OldBoy/Day2)
- 博客园,[老男孩Day2作业-编写购物车程序](http://www.cnblogs.com/ChuixinZeng/p/JamieZeng_Day2.html)

### 2017/07/16程序优化备忘

- shopping过程中余额不足的话，无法在购物过程中直接充值，所以增加了判断，让用户在购物过程中可以选择充值、退出、返回

- 循环打印第一级的分类的时候，使用enumerate，可以输出下标，而脚本中没有使用下标进行判断，而是让用户直接输入分类名称，实际上这个地方使用enumerate更灵活，后面判断用户输入的时候，可以用下标判断或用分类判断

- 开始使用了os.system('clear')，但是发生乱码问题，应该是字符集的问题
