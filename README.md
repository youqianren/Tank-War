# Tank-War
马士兵坦克大战项目学习


1.猜想可能要实现的功能：
                    1.创建出坦克
                    2.使坦克可以上下左右移动
                    3.坦克发射出子弹
                    4.创建敌方坦克
                    5.敌方坦克可以上下左右移动并发射子弹
                    6.击中敌方坦克，敌方坦克消失
                    7.自己被击中，游戏结束
2.实际需求：
          1.能够四处移动
          2.能够打击敌人
          3.敌人能够移动
          4.能够模拟爆炸
          5.能够产生障碍
          6.能够增长生命

p1、p2、p3： 创建窗口 使窗口可关闭，不可更改窗口大小.
p4： 画坦克
p5： 让坦克动起来  使用多线程不断重绘
p6： 消除坦克闪烁现象    创建背景图
p7:  代码重构  将经常需要改变的量设为常量
              常量一般是 public static final 
p8:  增加键盘事件监听
p9:  面向对象  给坦克单独创建类
     思考有哪些类、那些属性，优先考虑构造方法
p10: 使坦克可以朝8个方向移动  
     1.在键盘监听处 使用boolean 来判断坦克的移动方向，是为了防止坦克移动出错，所采取的一种方法
p11: 增加按键抬起的监听
p12: 添加子弹类
p13: 按下ctrl键打出子弹   
     1.按下ctrl 响应按下事件
     2.调用fire（）方法
     3.创建子弹
     因为在TankClient类绘制子弹，所以返回TankClient类下的Missile 类型，使TankClient类知道myMissile是否为空
     4.使子弹从坦克正中央发射出
p14: 绘制炮筒
P15: 打出多发炮弹
p16: 解决炮弹不消亡问题 、 以及炮弹出界问题
p17: 使用debug找错误
p18: 解决坦克出界问题
p19: 增加敌人坦克
p20: 将敌人坦克击毙
p21: 介绍了WinMerge的用法 可以对比两个版本哪个地方进行了更改
p22: 增加爆炸效果 
p23: 在坦克被打中时产生爆炸
p24: TankClient 没被赋初值
p25: 添加多辆坦克
p26: 解决右上角的坦克记数
p27: 使敌人坦克随机移动
p28: 使敌人坦克随机移动的更正常
p29: 敌人坦克可以发射子弹，并可以打死我方坦克
p30: 添加一堵墙
p31: 使子弹、坦克穿不过墙
p32: 坦克不能互相穿越
p33: 超级炮弹
p34: 给我方坦克增加血条
p35: 绘制血条
P36: 添加血块，随机出现，坦克吃掉血块可以补血
p37: 按f2我方坦克复活，敌方坦克全死亡后，再生成一波坦克
p38: 生成java文档、打包成jar
