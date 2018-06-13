# storage-controller
一个本地存储工具，通过相同的api去支持`localStorage`和`sessionStorage`
## 安装

```
 npm install storage-controller --save
```

## 使用

```
 import storage from 'storage-controller'
 
 // localStorage
 storage.set(key,val) 
 
 storage.get(key, def)
 
 // sessionStorage
 storage.session.set(key, val)
 
 storage.session.get(key, val)
 
```

## API

#### set(key, val)

存储storage，key为键，val为值

#### get(key, def)

根据key去获取storage，def为默认值, 如果找不到会返回def

#### remove(key)

根据key去删除storage

#### has(key)

根据key去判断storage是否存在

#### clear()
删除所有storage

#### getAll()
获取所有storage

#### forEach(callback)
循环所有的storage，callback为回调函数

#### session `<Object>`
sessionStorage操作，继承localStorage所有api