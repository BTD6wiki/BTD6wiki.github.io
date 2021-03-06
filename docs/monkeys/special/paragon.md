# 模范猴子
## 简介
- 当场上有同种猴子3个路径的5级各至少一个时，玩家可以将其中一个5级升级至模范。
- 升级至模范时，场上所有的同种猴子均会被献祭，然后根据献祭的猴子的一些参数确定最终的模范度（degree）。
- 在27.0版本时，模范在胜利界面显示为6-0-0，而从28.0开始时，显示变为5-5-5。
- 模范度越高，模范猴的能力越强大！

## 注意事项
- 模范不能受到其他防御塔提攻击加成，但可以受到知识点提供的加成。
- 同种模范只能在场上存在一个，即使是合作模式。
- 玩家不能在沙盒模式中将防御塔升级至模范。


## 模范度的计算公式
达到每个模范度需要献祭的猴子所提供的“能量”达到特定的值。  
其中“能量”跟以下4个参数相关：

1. 5级的数量（多人联机）
    - 每拥有三条路径之一的5级增加10000点
    - 最高可达到90000点
    - 不包括用于合成的3个5级
2. 总花费
    - 每花费25块钱增加1点
    - 最高可达到10000点
    - 不包括用于合成的3个5级
3. 总击破数
    - 每180击破增加1点
    - 最高可达到90000点
    - 若防御塔有产生的钱，则将产生的钱的4倍计入击破数中
4. 升级数
    - 每拥有1个升级增加100点  
    计算方法：一个420猴子算4+2=6次升级，提供600点，一个000猴子算0次升级，提供0点
    - 不包括所有的5级

模范度的能量需求公式如下：

$$
\left\{\begin{matrix}
 0, & D=1 \\ 
 \frac{50D^3+5025D^2+168324D+843000}{600}, & 2\leq D\leq 99 \\ 
 200000, & D=100 
\end{matrix}\right.
$$

其中*D*为模范度，上述结果四舍五入至整数。

![模范猴能量](模范猴能量.png)

## 模范度提升指南
基本要求： 对应三条路径的5级塔

因为每 20 点模范度，猴子能获得更强大的外观和技能增强等等各方面强化，所以尽可能让模范点以20为倍数吧。

**1点模范度**  

需要 0 能量

**20点模范度**

需要 11,032 能量，主要组成：  

- 花费 $125,000 在献祭上（5000能量）
- 场上有 17 个 6次升级的塔（10,000能量，已满）

**40点模范度**

需要 31,360 次能量，主要组成：  

- 花费 $250,000 在献祭上（10,000能量，已满）
- 场上有 17 个 6次升级的塔（10,000能量，已满）
- 在祭祀塔上获得 204 万人口（13,000+能量）

**60点模范度**

需要 66,387 能量，主要组成：  

- 花费$250,000在献祭上（10000能量，已满）
- 场上有 17 个 6次升级的塔（10,200能量，已满）
- 在祭祀塔上获得 835 万人口（46,000+能量）

**76点模范度（单人最高）**

77 级需要 110,706 能量，是凑不够的。所以单人最高为76级，主要组成：  

- 花费 $250,000 在献祭上（10000能量，已满）
- 场上有 17 个 6次升级的塔（10,200能量，已满）
- 在祭祀塔上获得 1,620 万人口（90,000能量，已满）

**100点模范度（最大）**

需要 200,000 能量，主要组成：  

- 花费 $250,000 在献祭上（10,000能量，已满）
- 场上有 17 个 6次升级的塔（10,000能量，已满）
- 在祭祀塔上获得 1,620 万人口（90,000能量，已满）
- 9个三条路径之一的5级塔（来自联机玩家的90,000能量）


## 总结
- 由于单人无法建造更多的5级，因此通常情况下单人游戏的最高模范度为76。此时献祭提供的能量为110000，距离77级还有706。飞镖猴在有知识的情况下单人可以多建造一个5级，因此飞镖可以升至79级，距离80级还有115。  
也正因为如此，100模范度只有4人合作才能完成（飞镖猴可以为3人）。
- 模范猴子均对BOSS造成更高的伤害，所以在BOSS活动中推荐使用。  
- 在自由游戏中，模范猴子可以增加单位面积的输出（因为模范猴子通常比3个5级加在一起伤害高），也同样可以建造。
- 若将模范猴子用于BOSS活动，如果可能的话，建议玩家将模范度升至20的倍数，这样可以获得更多对BOSS伤害的加成。~~要知道39和40差的不是1%而是20%~~

## 参考资料
1. [Paragons | Bloons Wiki](https://bloons.fandom.com/wiki/Paragons  )
2. [Advanced Popology, vol. 7: Paragons](https://www.reddit.com/r/btd6/comments/qk3c09/advanced_popology_vol_7_paragons/)