<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>管理员常用资料_MC水瓶</title>
  </head>
  <body>

# 管理员常用资料_MC水瓶 2024/09/14 a

<a name="catalog"></a>

## 目录
[学习路线](#learningPath)  
[常见指令](#commonCommand)  
[新手接待](#newReception)  
[常见问题](#fAQ)

<a name="learningPath"></a>

## 学习路线

<a name="learningPathCatalog"></a>

[Git和Github](#gitAndGithub)  
[SpigotMC](#spigotMc)  
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
其中一个Minecraft修改版服务器软件的[网站](https://www.spigotmc.org/)。  
在网站上有下载Spigot服务器软件本身的方法和一个分享服务器功能的区域，一般叫插件下载。  
一个典型的插件在[这里](https://www.spigotmc.org/resources/coreprotect.8631/)，阅读说明便可找到插件的下载和如何使用。

[返回分类目录](#learningPathCatalog)

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

<a name="commonCommandUnregister"></a>

`authme unregister 玩家名`  
不再允许玩家登陆和在游戏内活动，和踢出具有同等效果。

[返回总目录](#catalog)

<a name="newReception"></a>

## 新手接待
事先准备资料：  
`PickaxeChat`安卓版，或iOS、Windows上的同类软件，  
特点是不需要进游戏就能聊天和发送命令（俗称“脱机挂”）。

`PWTech(PWGen)`或类似的随机数密码生成软件。

可在`群文件\管理员工具`找到。

将以下指令保存为记事本以便快速复制或查看`欢迎新人参考.txt`：

```
whitelist add 玩家名
authme register 玩家名 密码
```

### 步骤1:
当没有时间登记新玩家时，允许加入群然后把新玩家QQ号群发给其他所有管理员和群主，  
而有时间就直接在群里@新玩家，打招呼表示“我来登记”。  
收到QQ号的管理员如果有空就同上，多个管理员在线时以最先打招呼的人为准其他人不参与。

复制以下内容（可以按自己习惯修改）给每个新玩家：

```
MC水瓶Minecraft服务器
你好，邮箱地址（QQ邮箱？）和游戏名（启动器里填那个）发给我 不需要密码
游戏名只能是数字和字母
如果是盗版有皮肤也把皮肤文件传过来
```

然后发送“服务器说明书.html”给新玩家。  
QQ电脑版有个问题是，从群内发起私聊一开始不能发文件，  
要先发送一个消息以后关闭聊天窗口再**从QQ主界面消息列表**里打开聊天窗口，  
然后就能发文件。

### 步骤2：
应该收到新玩家回复的邮箱和启动器中填写的游戏名，然后回复“正在登记”。

[添加玩家到白名单](#commonCommandWhitelist)，  
在PWTech(PWGen)软件里生成12位大小写字母和数字组成的密码，  
用[注册指令](#commonCommandRegister)进行注册。  

### 步骤3:
修改玩家的群名片，用以下格式：

```
游戏名 QQ昵称
```

转发邮箱、游戏名、皮肤（如果有）、密码给群主，用以下格式：

```
邮箱
玩家名
生成的密码
```

### 步骤4：
复制以下内容给新玩家（把xxx换成刚刚注册的密码）：

```
密码是 xxx
进游戏后聊天栏发送

/l xxx

建议是用群文件整合包的自动登陆mod
或者记事本保存然后复制粘贴着用
```

[返回总目录](#catalog)

<a name="fAQ"></a>

## 常见问题

<a name="fAQCatalog"></a>

### 常见问题-目录
1. [怎么改密码？](#changePassword)

[返回总目录](#catalog)

<a name="changePassword"></a>

### 怎么改密码？
说明书里写了。

[返回当前分类目录](#fAQCatalog)

[返回总目录](#catalog)

  </body>
</html>
