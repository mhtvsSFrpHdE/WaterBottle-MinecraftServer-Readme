<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>MC水瓶服务器管理员注意事项</title>
  </head>
  <body>

# MC水瓶服务器管理员注意事项 2020/02/13 a

## 目录
[权限](#permission)

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

  </body>
</html>