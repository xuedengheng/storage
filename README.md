# storage-controller
一个本地存储工具，通过相同的api去支持`localStorage`和`sessionStorage`

<a href="https://circleci.com/gh/tuateam/tua-storage/tree/master"><img src="https://img.shields.io/circleci/project/tuateam/tua-storage/master.svg" alt="Build Status"></a>
<a href="https://codecov.io/gh/xuedengheng/storage"><img src="https://codecov.io/gh/xuedengheng/storage/branch/master/graph/badge.svg" alt="Coverage Status"></a>
<a href="https://www.npmjs.com/package/storage-controller"><img src="https://img.shields.io/npm/v/storage-controller.svg" alt="Version"></a>
<a href="https://www.npmjs.com/package/storage-controller"><img src="https://img.shields.io/npm/l/storage-controller.svg" alt="License"></a>
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