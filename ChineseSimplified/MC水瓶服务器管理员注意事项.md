<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>MC水瓶服务器管理员注意事项</title>
  </head>
  <body>

# MC水瓶服务器管理员注意事项 2020/02/27 a

<a name="catalog"></a>

## 目录
[在开始之前](#beforeEverything)  
[学习路线](#learningPath)  
[常见指令](#commonCommand)  
[权限](#permission)  
[背包](#inventory)  
[多世界](#multiWorld)

<a name="beforeEverything"></a>

## 在开始之前
我已尽力使服务器的运行“去中心化”，这意味着每个人都可以参与到服务器管理中，  
我能对服务器做什么，所有人就也可以做什么，  
包括和不限于解决问题、封禁、更新、添加功能。  
更重要的是，为什么你会想要成为管理员。

我们有一份规则书作为大多数人的共识，  
它在游戏里限制人的行为，却因此为人提供保护。  
你不能入侵别人的房子和带走物品，看起来这好像很不“自由”，  
但别人却也不允许入侵你的房子，因此你的游戏进度是安全的。  
在服务器上有许多技术手段支持这些规则，但永远不可能面面俱到。  
因此一旦这些规则不被遵守，人将被抢走私有财产和不再有安全感。

允许任何人随时读档和封禁其他人不能对此提供帮助，  
当你可以这样做时，入侵者同样可以这样做而最终陷入更大的混乱。  
要解决这个问题，一些人必须出现和能够做其他人和入侵者不能做的事，  
最终对抗入侵者和保护所有人以及这些共识。  
在这个过程中，能飞行、无敌、和开创造权限刷道具，  
只是“能做其他人不能做的事”的最终体现，但不是本来的设计目的。  
整个事情是，人保证自己不入侵其他人的家，  
然后允许另一些人去读档和封禁，以便获得别人不入侵自己家的保障。  
但本来并不是要让这些人有游戏中的特权。

有时，这套机制会发生故障，例如这样的事：  
“支持我成为管理员，然后我从创造模式给你拿64个钻石块”  
“帮你封禁掉你不喜欢的人”、“悄悄让你飞行”等等。  
要避免这些不公平事情发生，不可能每天每秒都去监督。  
我的思考和制定的解决办法是，“不让管理员去接触游戏内的事”，  
而是将构成服务器的核心文件公布出来，直接修改文件来进行管理，  
最终通过简单的检查和将修改的部分“合并”进运行中的服务器来使修改生效。  
同时这些核心文件的修改过程也对所有人公开，  
这样“最终检查者”便也不能和管理员偷偷进行不公平的修改而不被发现。

然而，这对管理员和最终检查者提出了极高的道德要求。  
他必须要超越作为玩家的存在，对游戏内的任何特权都不在意。  
一件事如果没有好处，就难以说服人去做。  
也许，一个最终检查者或管理员想要的只是一个公平或稳定的游戏环境，  
那么对于他们来说，这显然就是足以支持他们不动摇的，天大的好处。  
但包括我在内，由于没有游戏内特权，也没有工资，  
我的思考不能告诉我如果最终检查者还是出了问题该怎么办。  
考虑到“服务器的核心文件是公开的”，那么如果你对这些管理员不满，  
你就随时可以用这些文件再开一个“一模一样的服务器”，  
然后自己成为最终检查者，和人们一起抛弃这些做的不好的人，这就是最后的手段。

就像你刚来的第一天发现的那件事一样，  
当你发现历史记录是公开的，你不会再侥幸关于偷着做某个事而不被发现。  
那么在一个人人都可以成为龙的世界里，还需要再担心我们的勇士发生故障吗？

[返回总目录](#catalog)

<a name="learningPath"></a>

## 学习路线
有许多工具加入到这个过程中来以便提高效率，有一件事必须注意：  
所有这些都具有一个前提是要会英语，  
或至少有了解英文内容中的信息，和把自己所想写回英文的办法。  
目前，最大的电脑技术圈子使用英语，  
这意味着一个德国的开发者能用英语编写软件，  
然后阅读和处理印度用户用英语写的错误报告，  
为了交流，人不用学全世界所有语言而只要其中之一。  
我们是服务器软件的中国用户，而我们还是要写英语回去报告错误。  
同时，这些服务器软件的使用方法也基本都是用英语写成。  
在进行“开服”的过程中其实并没有什么秘密，但它们都是用英语写成的。

<a name="learningPathCatalog"></a>

[Git和Github](#gitAndGithub)  
[SpigotMC](#spigotMc)  
[Bukkit](#bukkit)  
[实际应用](#howToUse)

[返回总目录](#catalog)

<a name="gitAndGithub"></a>

### Git和Github
一套服务器软件在使用过程中，为了符合一群玩家的需要，  
可能发生数百次以及数百处修改，要知道怎么改和改哪里不是很大的问题，  
而是五年之后，如何能知道是谁、什么时候、为什么改成了这个？  
如果这个修改导致了错误，那么原始的默认值又是什么？

有人很早就注意到了这些问题并带来了“Git”，可以解决上面提到的问题。  
“Github”是一个网站让人互相共享Git的文件夹。  
在一人电脑上的修改经过Github而到达另一人的电脑。

在[这里](https://git-scm.com/)查看Git的说明。  
在[这里](https://guides.github.com/activities/hello-world/)查看Github的说明，以及Github需要注册帐号。

[返回分类目录](#learningPathCatalog)

<a name="spigotMc"></a>

### SpigotMC
其中一个高性能Minecraft修改版服务器软件的[网站](https://www.spigotmc.org/)。  
在网站上有下载Spigot服务器软件本身的方法和一个分享服务器功能的区域，一般叫插件下载。  
一个典型的插件在[这里](https://www.spigotmc.org/resources/coreprotect.8631/)，阅读说明便可找到插件的下载和如何使用。

[返回分类目录](#learningPathCatalog)

<a name="bukkit"></a>

### Bukkit
吃水不忘挖井人，Bukkit是古典的Minecraft服务器软件。  
Spigot从Bukkit上再次修改而试图进一步优化。  
在[这里](https://bukkit.org/)查看Bukkit自己的下载，  
Spigot和Bukkit一样具有下载插件的提示。

[返回分类目录](#learningPathCatalog)

[返回总目录](#catalog)

<a name="howToUse"></a>

### 实际应用
服务器插件是Bukkit提供的，而Spigot大致兼容Bukkit规格的插件。  
从Spigot处取得服务器软件和用Java启动，再把plugins在内的整个文件夹制成Git，  
每次修改时在Git处登记修改理由，修改时间和修改人会自动登记。  
完成后通过Github交换Git文件夹，把一个修改过的Git合并进原始的Git从而实现更新原始Git的内容。  
有关于“到底应该怎么修改”，应该亲自去查阅每个插件或Spigot、Bukkit本身的说明。

[返回分类目录](#learningPathCatalog)

[返回总目录](#catalog)

<a name="commonCommand"></a>

## 常见指令

`pex user 玩家名 group remove trialMessage`  
去除玩家的垃圾短信提醒。

[返回总目录](#catalog)

<a name="permission"></a>

## 权限
[权限](#permissionPermission)  
[权限组](#permissionPermissionGroup)

[返回总目录](#catalog)

<a name="permissionPermission"></a>

### 权限
由于使用两个以上的权限组来实现临时权限，这些权限组之间的继承关系不会立刻刷新。  
在修改权限后，记得使用`/pex reload`重新载入权限以便刷新继承关系。

<a name="permissionPermissionGroup"></a>

[返回分类目录](#permission)

### 权限组
每次新增或删除权限组时应注意，少数插件需要分别修改配置文件以便识别权限组。  
完整的列表：

- ZHorse\config.yml

[返回分类目录](#permission)

[返回总目录](#catalog)

<a name="inventory"></a>

## 背包
恢复意外死亡的玩家背包，使用[Inventory Restore 2](https://www.spigotmc.org/resources/inventory-restore-remastered.22027/)。  
调查玩家的背包以及末影箱，使用[OpenInv](https://dev.bukkit.org/projects/openinv)。  
调查临时创造模式玩家是否作弊，使用[Core Protect](https://www.spigotmc.org/resources/coreprotect.8631/)。

[返回总目录](#catalog)

## 多世界
当创建一个世界，随机传送插件总是会把玩家传送到一个固定位置。  
到RandomTeleport\Worlds:下添加世界名和传送范围以便解决。

[返回总目录](#catalog)

  </body>
</html>