<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>管理员手册_MC水瓶</title>
  </head>
  <body>

# 管理员手册_MC水瓶 2020/06/19 a

<a name="catalog"></a>

## 目录
[学习路线](#learningPath)  
[常见指令](#commonCommand)  
[新手接待](#newReception)  
[常见问题](#fAQ)  
[权限](#permission)  
[背包](#inventory)  
[多世界](#multiWorld)

<a name="learningPath"></a>

## 学习路线
有许多工具加入到这个过程中来以便提高效率，有一件事必须注意：  
所有这些都具有一个前提是要会英语，  
或至少有了解英文内容中的信息，和把自己所想写回英文的办法。  
无需担心关于不会的问题，现在就开始学也来得及，  
你不需要学习所有的英语就可以完成帮忙。  
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

<a name="commonCommandWhitelist"></a>

`whitelist add 玩家名`  
添加玩家到白名单

<a name="commonCommandRegister"></a>

`authme register 玩家名 密码`  
为新玩家注册。

<a name="multiWorldPermission"></a>

`multiverse.access.DigTheEnd`  
`multiverse.access.Dig`  
添加这些权限允许进入多世界的其中之一。  
需要玩家提供资格证明后分别添加对应世界的权限而不是一下全加上。

[返回总目录](#catalog)

<a name="newReception"></a>

## 新手接待
事先准备软件：  
`PickaxeChat`安卓版，或iOS、Windows上的同类软件，  
特点是不需要进游戏就能聊天和发送命令（俗称“脱机挂”）。

`PWTech(PWGen)`或类似的随机数密码生成软件。

将以下指令保存为记事本以便快速复制：

```
whitelist add 玩家名
authme register 玩家名 密码
pex user 玩家名 group remove trialMessage
```

### 步骤1:
当没有时间登记新玩家时，允许加入群然后把新玩家QQ号群发给其他所有管理员和群主，  
而有时间就直接在群里@新玩家，打招呼表示“我来登记”。  
收到QQ号的管理员如果有空就同上，多个管理员在线时以最先打招呼的人为准其他人不参与。

复制以下内容（可以按自己习惯修改）给每个新玩家：

```
MC水瓶Minecraft服务器
你好，邮箱地址（QQ邮箱？）和游戏名（启动器里填那个）发给我 不需要密码
如果是盗版有皮肤也把皮肤文件传过来
```

然后发送“服务器说明书.html”给新玩家。  
QQ电脑版有个问题是，从群内发起私聊一开始不能发文件，  
要先发送一个消息以后关闭聊天窗口再**从QQ主界面消息列表**里打开聊天窗口，  
然后就能发文件。

### 步骤2：
应该收到新玩家回复的邮箱和启动器中填写的游戏名，然后回复“正在登记”。  
在PWTech(PWGen)软件里生成12位大小写字母和数字组成的密码和用[注册指令](#commonCommandRegister)进行注册。  
之后转发邮箱、游戏名、皮肤（如果有）、密码给群主。

### 步骤3:
[添加玩家到白名单](#commonCommandWhitelist)之后，  
用新玩家的游戏名**进入游戏一次**触发新玩家自动初始化**后**退出游戏，  

### 步骤4：
复制以下内容给新玩家（把xxx换成刚刚注册的密码）：

```
密码是 xxx
进游戏后聊天栏发送

/l xxx

登陆，不要告诉别人密码
建议是用记事本保存然后复制粘贴着用，
这是为了防止一旦服务器被黑客攻击拿到密码本，
就能用来猜测其他网站的密码导致盗号

登陆一次后3天内再次进游戏不需要重新登陆
原因是中国大多数家庭宽带运营商约3天换一次IP
```

[返回总目录](#catalog)

<a name="fAQ"></a>

## 常见问题

<a name="fAQCatalog"></a>

### 常见问题-目录
1. [怎么改密码？](#changePassword)  
1. [不能进去资源世界等多世界？](#multiWorld)

[返回总目录](#catalog)

<a name="changePassword"></a>

### 怎么改密码？
说明书里写了。

[返回当前分类目录](#fAQCatalog)

### 不能进去资源世界等多世界？
查看服务器说明书“车站”章节，  
拥有一个车站和提供资格证明后管理员用[添加多世界权限](#multiWorldPermission)指令允许玩家进入。

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