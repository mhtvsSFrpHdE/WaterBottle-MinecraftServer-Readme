<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>管理员手册_MC水瓶</title>
  </head>
  <body>

# 管理员手册_MC水瓶 2020/02/27 a

<a name="catalog"></a>

## 目录
[学习路线](#learningPath)  
[常见指令](#commonCommand)  
[权限](#permission)  
[背包](#inventory)  
[多世界](#multiWorld)

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

<a name="commonCommandRegister"></a>

`authme register 玩家名 密码`  
为新玩家注册。

<a name="commonCommandActivate"></a>

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

<a name="multiWorld">

## 多世界
当创建一个世界，随机传送插件总是会把玩家传送到一个固定位置。  
到RandomTeleport\Worlds:下添加世界名和传送范围以便解决。

[返回总目录](#catalog)

  </body>
</html>