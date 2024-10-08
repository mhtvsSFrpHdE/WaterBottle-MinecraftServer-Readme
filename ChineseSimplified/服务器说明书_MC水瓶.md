<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>服务器说明书_MC水瓶</title>
  </head>
  <body>

# 服务器说明书_MC水瓶 2024/09/28 a

## 阅读方法
点击链接查看对应章节，连续点击到具体描述后如果想回到之前阅读的地方，  
在浏览器地址栏附近有“向后退”、“上一页”按钮，可返回点击某链接之前所在的位置。

<a name="catalog"></a>

## 目录
[玩法和重要提醒（先看这里）](#howToPlaySafe)  
[密码安全](#passwordSecurity)  
[游戏规则](#gameRules)  
[管理员权限（不给OP或创造）](#adminPermission)  
[基础设施](#infrastructure)  
[常见问题](#fAQ)

<a name="howToPlaySafe"></a>

## 玩法和重要提醒（先看这里）
1. **只有在高难度世界死亡时物品和等级会掉落**，具体看[这里](#died)。
1. **不要在网络很卡时打开箱子**，有一次一个人开着箱子掉线之后背包空了。
1. **设置家是用领地插件**，具体看[这里](#residenceRelated)。
1. 其他值得关注的内容在常见问题章节处列出，具体看[这里](#fAQ)。

[返回总目录](#catalog)

<a name="passwordSecurity"></a>

## 密码安全
有一个整合包在群文件，其中有自动登陆mod，模组设置-CommandKeys-设置-修改密码为自己的，  
在聊天栏没有打开的状态下，按退格下方的“\”键登陆。  
或将自动分配的密码保存在记事本文件中之后用复制粘贴的方式输入。

仍然使用以下指令可随时修改自己的密码，但不建议使用容易被猜对的和与其他处重复的密码。

<a name="authMeChangePassword"></a>

`/changepassword 旧密码 新密码`  
不要使用易于被猜测的和与其他网站相同的密码，因为Minecraft服务器的安全性缺乏保障。

无法阻止Minecraft服务器被黑客入侵，即使获取单个Minecraft服务器本身的密码经济利益不大，  
但有可能该密码同时被用于多个重要网站甚至银行卡，导致这些被黑客破解密码的机会变大而陷入危险。  
我们要求玩家使用服务器分配的至少12位长度的，大小写字母和数字随机分布的密码，  
这样即使密码数据库被黑客获取也能确保其他Minecraft服务器和重要网站甚至银行卡密码的安全。

[返回总目录](#catalog)

<a name="gameRules"></a>

## 游戏规则
除非特殊说明，这些规则对服务器中的“建筑世界”、“红石世界”起作用。  
所有规则指向一个简单的目标：

<h1>不要影响到其他人</h1>

<a name="considerOthers"></a>

### 思考某个行为对其他人的影响
<ul>
  <li>
    <p>
      不要破坏经常访问的区域如出生点或其他人家周围的地貌特征。<br>
      如挖掉一座山，或填平一块区域、大规模砍树且不补种等会导致改变视觉效果的行为。<br>
    </p>
  </li>
  <li>
    <p>
      垂直向下挖，这可以造成别人摔死，因此除非在自己家中“室内”，<br>
      任何公共场合下包括野外不要这样做。
    </p>
  </li>
</ul>

### 领地、地皮、占地相关
[点击此处](#residenceRelated)查看详情。

<a name="freeAccessServerHistory"></a>

### 服务器历史记录对所有玩家开放

<a name="coreProtectInspector"></a>

`/co i`  
调查某个方块或物品的活动历史记录，这是一个开关指令，  
第一次使用时进入调查模式，再次使用退出调查模式和继续正常游戏。  
在调查模式中：

* 左键点击某方块调查谁放置的
* 右键点击某方块调查附近的方块是否有被其他人破坏
* 右键在某方块处**摆放**方块调查被摆放的方块特定位置是否有被其他人破坏
* 右键点击某物体如门、箱子、按钮等调查是否有人使用过

所有的调查结果都会含有其他人的玩家名和行为，这代表当事人将能够报告是谁做了破坏行为。  
因此在做任何事之前需要了解这些事可**在之后被任何人随时调查**。

<a name="coreProtectLookup"></a>

`/co lookup`  
高级调查，查阅CoreProtect服务器插件的使用说明来了解这一点。

[返回总目录](#catalog)

<a name="adminPermission"></a>

## 管理员权限（不给OP或创造）
通常情况下不设置和使用管理员权限角色，任何人都可通过Github访问服务器设置文件。  
将服务器设置文件下载和修改后，给出修改理由并提交回原处。

即使可以通过群文件和聊天完成提交，但用Github完成的提交会具有更快的处理优先级。  
这是因为Git Diff工具在这个过程中提供了一系列的便利功能。

提交的修改经过资源占用、平衡性评估后会更新到服务器上。  
当决定修改服务器设置，提交到Github可提供绝大多数的帮助。

[返回总目录](#catalog)

<a name="infrastructure"></a>

## 基础设施

<a name="infrastructureCatalog"></a>

### 基础设施-目录
[箱子锁](#lWC)  
[马锁](#zHorse)  
[交易](#trade)  
[传送](#teleport)  
[多世界](#multiWorld)  
[呼叫](#notify)  
[皮肤](#skin)  
[彩色牌子](#coloredSign)  
[服务器状态](#serverStatus)  
[区块加载器](#chunkLoader)

[返回总目录](#catalog)

<a name="lWC"></a>

### **LWC**
是箱子锁，当一个箱子或重要物品被摆放时自动注册以防止他人破坏。  
大部分物体自动注册成“**有锁的**”以防止其他人使用，  
另一些不重要的会自动注册成“**共享的**”，这时其他人只能使用不能破坏。  
默认设置下，漏斗不能从有LWC的容器中取物品。

<a name="lWCPrivate"></a>

`/cprivate`  
使用指令后点击一个物体将自己登记为拥有者和状态为“有锁的”。  
前提是此物体尚未注册LWC，见[去除LWC保护](#lWCRemove)。

<a name="lWCPublic"></a>

`/cpublic`  
使用指令后点击一个物体将自己登记为拥有者和状态为“共享的”。  
前提是此物体尚未注册LWC，见[去除LWC保护](#lWCRemove)。

<a name="lWCModifyPlus"></a>

`/cmodify 玩家名`  
使用指令后点击一个物体允许特定的一个玩家使用。

<a name="lWCModifySubtract"></a>

`/cmodify -玩家名`  
相同的指令，但在玩家名前添加半角减号，  
点击一个物体不再允许特定的玩家使用。

<a name="lWCRemove"></a>

`/cremove`  
使用指令后点击一个物体去除LWC保护，使所有人可使用的同时也能破坏和[成为拥有者](#lWCPrivate)。

<a name="lWCInfo"></a>

`/cinfo`  
使用指令后点击一个物体查看目前的拥有者。

[返回当前分类目录](#infrastructureCatalog)

<a name="zHorse"></a>

### **ZHorse**
是马锁，驴和其他等载具生物也可利用到这些功能。  
和箱子锁不同，一个被驯服的马不会立刻被添加保护。  
被上锁的马不能被其他玩家骑走、解除或使用拴绳，  
但可能随机移动离开原处，因此总是使用拴绳固定马或放2格深坑里防丢。  
拴绳甚至会在所固定的物体被破坏之后仍然继续存在。

`/zh claim 马名（可选）`  
骑着马时使用，为马命名和添加保护。  
注册的马会避免受到一些常见伤害，并防止其他人使用和访问马的背包。  
当不指定马名时，将从一个预先设置的列表中随机起名。

`/zh free`  
骑着马时使用，取消注册马的保护。

`/zh friend add 玩家名`  
将马共享给玩家，允许他使用和访问马的背包。  
对所有马起作用。

`/zh friend remove 玩家名`  
将玩家从共享的马的列表中去除，将不再能使用马。

`/zh friend list`  
显示和自己有关的在服务器登记的马的共享关系。

`/zh give 玩家名`  
将登记的马的主人改为另一个玩家，使用此指令后不会立刻下马。  
如果自己不在对方的马共享列表中，将失去马的使用权。

[返回当前分类目录](#infrastructureCatalog)

<a name="trade"></a>

### **交易**
和商店以及交易有关的指令。关于经济系统完整的介绍查看[这里](#economy)。  
无限交易的系统商店位置在出生点，右键物品所在的台阶进行交易。

<a name="tradeSellHand"></a>

`/mp add 单价`  
当前持有的物品以**单价**登记到交易板。  
例如一组64个想卖总共100，那就100除16保留两位得1.57。

<a name="tradeShop"></a>

`/mp listings`  
打开交易板菜单，点击一个购买物品之后，下方提示变成确认，再点一次购买。  
购买的物品进入收件箱，菜单左下按钮切换到收件箱，或`/mp mails`

`/balance`  
查看余额。

<a name="tradeFaceToFace"></a>

`潜行状态右键点击另一个玩家`  
发起交易，收到交易请求时点击聊天框中颜色标记的命令，同意进行带有保证的交换物品、经验值、铁矿石币。  
能一定程度上防止扔物品时附近爆炸了苦力怕，或扔进火里，或总扔不到正在移动的对方身上。

[返回当前分类目录](#infrastructureCatalog)

<a name="teleport"></a>

### **传送**

<a name="teleportHome"></a>

`/tpa 玩家名`  
发送传送到别的玩家处的请求。

`/tpahere 玩家名`  
发送传送别的玩家到自己处的请求。

`/tpaccept`  
同意对方到自己这里，或自己到对方处。

`/home`  
没有等待时间的立刻回到最近一次游戏中**无论是否夜间**、**右键过**、**没有被破坏**的床处。

`/res tp 领地名`  
知道领地名就可以传送包括到别人的，没有名称是回自己领地。

`/warp 名称`  
前往预先设置的地标，一些常用的：
- `spawn` 出生点
- `grid` 和出生点是同一个地方，或叫主城
- `lemon` 前往红石世界或资源世界
- `lamp` 前往高难度世界

`传送门`  
在world, lemon, dig世界中，  
使用下界、末地传送门会分别去三个世界对应的下界和末地，返回时也一样。  
lemon_amp高难度世界没有自己的下界和末地，在其中使用传送门不知道会去哪，  
应该也是不能通过传送门进入高难度世界。

[返回当前分类目录](#infrastructureCatalog)

<a name="multiWorld"></a>

### 多世界
在出生点附近放有前往其他世界的牌子。  
特点是第二行写绿色字`[mv]`然后第三行写要前往的世界名。  
点击[这里](#multiWorldList)查看服务器上完整的世界列表。

<a name="multiWorldBack"></a>

要返回定居的世界，使用[/home或/res tp](#teleportHome)。

[返回当前分类目录](#infrastructureCatalog)

<a name="multiWorldList"></a>

### 多世界-目录
这是服务器上世界完整的列表：

[建筑](#multiWorldBuildWorld)  
[红石](#multiWorldRedstoneWorld)  
[资源](#multiWorldDigWorld)  
[放大化（高难度）](#multiWorldAmpWorld)

[返回当前分类目录](#infrastructureCatalog)

<a name="multiWorldBuildWorld"></a>

#### 建筑
世界名：`world`  
创建时间：`1.12.2`  
服务器首次创建时分配的世界。新玩家的出生点在这里。  
长期保留。  
有自己对应的下界和末地。

[返回当前分类目录](#multiWorldList)

<a name="multiWorldRedstoneWorld"></a>

#### 红石
世界名：`lemon`  
创建时间：`1.21.1`  
防爆插件关闭的世界，能运用更多原版红石特性但也更危险，不适宜居住。  
长期保留。  
有自己对应的下界和末地。

[返回当前分类目录](#multiWorldList)

<a name="multiWorldDigWorld"></a>

#### 资源
世界名：`dig`  
创建时间：`跟随服务器版本`  
防爆插件关闭的世界，可以反复获得一些不可再生资源或新版本内容。  
有自己对应的下界和末地。

不要进行长期建设或遗留物品，它可能在任何时候被清空。  
这里不受到[领地规则](#residenceRelated)的保护，但也别把出生点炸烂，别人也要走路跑图的。

[返回当前分类目录](#multiWorldList)

<a name="multiWorldAmpWorld"></a>
#### 放大化（高难度）
世界名：`lemon_amp`  
创建时间：`1.21.1`  
实验玩法，死亡背包物品和经验会掉落，有防爆，目前不知道有什么用，可能自然景观多用来建筑。  
没有放大化的下界和末地，使用传送门不知道会去哪，没试过，不建议。

[返回当前分类目录](#multiWorldList)

<a name="notify"></a>

### **呼叫**
提醒一个玩家回复消息。 

<a name="notifyAt"></a>

`@玩家名`  
没有空格，最少输入玩家名的前3位也能呼叫到。  
也可以@自己，效果是发出铁砧落地音效。

[返回当前分类目录](#infrastructureCatalog)

<a name="skin"></a>

### **皮肤**
使用去中心化的，不依赖外部皮肤站和mod的设置皮肤方法。

<a name="skinMenu"></a>

`/skins`  
打开一个菜单列出服务器上保存的所有皮肤和可以选择其中之一。

<a name="skinOthers"></a>

`/skin 玩家名`  
从一个别的正版玩家帐号上获得皮肤和设置成自己的。  
首次进入服务器时会根据玩家名自动获得皮肤而不用特意对自己的名字使用  
影响范围仅限此服务器。

[返回当前分类目录](#infrastructureCatalog)

<a name="coloredSign"></a>

### **彩色牌子**
在牌子上可以使用Minecraft颜色或格式代码。  
在<a href="https://minecraft-zh.gamepedia.com/%E6%A0%B7%E5%BC%8F%E4%BB%A3%E7%A0%81" target="_blank">Minecraft百科</a>上可以找到各种颜色和样式的示范。  
但在游戏内无法输入双S符号，因此以&符号代替双S符号进行牌子编辑。

[返回当前分类目录](#infrastructureCatalog)

<a name="serverStatus"></a>

### **服务器状态**
调查服务器状态。主要用于当发生延迟时，  
帮助判断是网络问题还是服务器系统资源耗尽。

<a name="serverStatusReport"></a>

`/tabtps toggle actionbar`  
切换持续显示服务器TPS、MSPT、Ping值。

`/tps`  
简化的服务器信息，仅报告TPS数值。  
理想情况下是20，当服务器处理器资源耗尽时会下降。  
此数字报告为16或以下时可认为服务器处理器资源严重不足和导致延迟。  
将连续显示三个，在多个数字都小于17时建议报告这个情况。

`/gc`  
`/lag`  
`/mem`  
`/memory`  
`/uptime`  
`/entities`  
查看服务器运行速度以及内存使用情况等信息。  
任何一个都有相同的效果，是仅为兼容旧版而保留的快捷方式。

`/ping 玩家名`  
可能是查看自己到服务器的延迟、服务器到目标玩家的延迟总和。

`/localdifficulty`  
查看单机模式中显示但多人游戏不可见的区域难度。

[返回当前分类目录](#infrastructureCatalog)

<a name="chunkLoader"></a>

### **区块加载器**
玩家离开后保持区块加载，服务器资源有限，加载器可能会不定期回收。  
不抗卸载的红石开机前注意相关区块是否设为保持加载。  
[用户宏](#clientMacro)和`coords`可以快速指定区块进行加载。

<a name="chunkLoaderLoad"></a>

`/kc keepchunk current`  
`/kc keepchunk coords 区块坐标x 区块坐标z 世界名`  
`current`是将所在区块设为保持加载。  
`coords`是按区块坐标（不是方块坐标）设为保持加载。

`/kc releasechunk current`  
`/kc releasechunk coords 区块坐标x 区块坐标z 世界名`  
`current`是将当前区块恢复默认设置（不保持加载）。  
`coords`是按区块坐标（不是方块坐标）恢复默认设置。

`/kc chunkinfo current`  
`/kc chunkinfo coords 区块坐标x 区块坐标z 世界名`  
`current`是查询所在区块是否保持加载，`Marked: Yes`是已设为保持加载。  
`coords`是按区块坐标（不是方块坐标）查询。

`/kc list`  
查询服务器上所有设为保持加载的区块。

`/kc help`  
查看区块加载器插件帮助。

[返回当前分类目录](#infrastructureCatalog)

<a name="clientMacro"></a>

### **用户宏**
客户端的`CommandKeys` mod可以用来做常见指令操作，  
将命令设置到按键，像是
- [快速登陆](#passwordSecurity)
- [切换显示TPS和MSPT](#serverStatusReport)
- [将当前或某几个区块设为保持加载](#chunkLoaderLoad)

[返回当前分类目录](#infrastructureCatalog)

[返回总目录](#catalog)

<a name="fAQ"></a>

## 常见问题

<a name="fAQCatalog"></a>

### 常见问题-目录
1. [需要买或卖东西，并且发现没有初始货币，这是怎么回事？](#economy)
1. [死了，但是物品和经验没保留？](#died)
1. [标记和占有一片区域的方法是什么，如领地或地皮等？](#residenceRelated)
1. [不能用漏斗或其他机器从箱子和其他容器中取出物品？](#hopperNotWorkWithChest)
1. [红石玩法（生电）相关](#technicalminecraft)

[返回总目录](#catalog)

<a name="economy"></a>

### 需要买或卖东西，并且发现没有初始货币，这是怎么回事？
在这里完整的介绍关于服务器的货币设计。  
在[基础设施](#infrastructure)章节的[交易](#trade)列出了相关的指令和如何使用。

当将1个精准采集获得的铁矿石交给系统商店，可获得10币并且保证可在任何时候用10币换回1铁矿石，  
因此暂时称为“铁矿石币”，在这个基础上换得的铁矿石币可方便的携带、转账、交易。  

假设找到下界要塞，但别人已经来过一次，整个下界要塞都找不到下界疣，就无法炼药。  
冒险途中遇到结构商店（下界要塞、末地船等），可以100/次的价格交换这类本来可以获得的绝版战利品。

除此之外，有玩家之间自由定价交易而非服务器指导价格的市场，  
可上架任何物品[销售给其他玩家](#tradeSellHand)获得铁矿石币。

[返回当前分类目录](#fAQCatalog)

<a name="died"></a>

### 死了，但是物品和经验没保留？
查看[服务器的世界列表](#multiWorldList)。

高难度世界和单人游戏一样，它们会留在死亡地点并且可能由于**各种原因**而消失。  
所有需要做的是别去高难度世界、[避免死亡](#teleportHome)，或及时赶回现场捡起。  
在1.21.1时代，由于`/gamerule keepInventory true`存在，没找到专门插件会保存背包，因此现在没有恢复能力。

[返回当前分类目录](#fAQCatalog)

<a name="residenceRelated"></a>

### 标记和占有一片区域的方法是什么，如领地或地皮等？
`Residence`插件创建最小3x3x3，最大16x320x16的区域好能传送回家。

手持木棍，左键一个方块，右键一个方块  
`/res create 名称`  
创建领地，创建时的位置和面朝方向是传送回领地时的位置。

`/res tpset`  
当前的位置和视角朝向设为领地传送时的目标地点。

`/res tp 名称`  
知道名称就可以传送到一个领地，不加名称是回自己的。

站在一个领地中  
`/res remove`  
删除不想要的领地

对于超过16x16的大型景点，建议的方式是在各个出入口以及边界放置牌子为此处起名。  
因此当你在任何地方看到已命名的区域，不要在此处进行建筑或破坏行为，  
你的行为[被服务器记录](#freeAccessServerHistory)，并可能在未来引起相关纠纷。

在陌生人家附近盖房子的建议是从别人家边缘远离100格以上（6个区块左右），  
留出足够的空间避免互相把房子盖进别人家中。

标记区域的大小没有限制，同时为了避免浪费，  
在一块**新命名**的区域内超过**28天**没有进行有意义的建造活动则失去占有权。  
后来者可通过[查询标记牌子](#freeAccessServerHistory)来确认**未开发区域**的空闲时间。  
在未进行开发的前提下，破坏命名牌子并重新放置不刷新空闲时间，  
因为**包括前一次放置牌子**在内的行为也都[被服务器记录](#freeAccessServerHistory)。

地表建筑与地下资源分别计算空闲时间，占有区域中的**地下不可再生资源**不受到保护，  
挖矿行为是合理的，但如果在挖矿过程中挖进别人地下家中，  
挖矿者有义务将墙壁恢复原状并绕路继续，或破坏了需要精准采集的，自己没有的物品，  
在显眼处放置牌子提醒所有者修复和找你赔偿。

[返回当前分类目录](#fAQCatalog)

<a name="hopperNotWorkWithChest"></a>

### 不能用漏斗或其他机器从箱子和其他容器中取出物品？
这是箱子锁LWC的防止物品被非玩家取出防盗导致的现象，  
需要去除目标物体上的保护，具体[查看LWC的说明](#lWCRemove)。

[返回当前分类目录](#fAQCatalog)

[返回总目录](#catalog)

<a name="technicalminecraft"></a>

### 红石玩法（生电）相关
不是专业生电服，仅对生电提供有限的支持：
1. 没有专业生电服的每日备份和还原（回档），机器爆炸风险自负。  
使用[区块加载器插件](#chunkLoader)和压力板制作离开后自动关机结构，  
防止掉线或临时有事离开忘记关机导致的炸膛等故障。  
区块加载器占用服务器资源，可能被回收，不可以假设永远有效，  
开机前检查区块加载器，人不在电脑前或用完机器打算离开就要关机，切换到区块即使被卸载也是安全的状态。  

2. 尽量避免使用音符盒加右键触发的危险开关，连点器忘记关闭右键了多次导致机器爆炸经常上报纸。  
在开关后附加锁存器也可以防止手滑发送多个脉冲到开机线路。

3. Spigot服务端不能保证精确的红石刻，在高负载下可能会跳过红石刻或游戏刻，  
造成某些机器不能复位或无效。针对这些现象已对`spigot.yml`[进行一些修改](https://github.com/mhtvsSFrpHdE/WaterBottle-MinecraftServer-Spec/commit/3008af62216584e570efacfb6426392270d5cf19)，  
可能减缓跳过现象，但从根本上说，Bukkit服务端不像Fabric服务端一样尊重原版特性。

4. 可观察[TPS、MSPT计数器](#serverStatus)，避免制造导致服务器TPS降低的机器。

[返回当前分类目录](#fAQCatalog)

[返回总目录](#catalog)

  </body>
</html>
