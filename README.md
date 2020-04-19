# CMS - 轻量级内容管理系统

CMS 使用 Node.js + MongoDB 开发，拥有灵活的内容模型以及完善的权限角色机制。

## 安装之前

```
db.createUser({
  user: "admin",
  pwd: "123456",
  roles: [
    {
      role: "root", db: "admin"
    }
  ]
})
```

## 安装

```bash
$ npm install --production
$ npm start
```

完成后访问 http://localhost:3000/admin/install 进入安装程序

**环境要求：**

1. [Node.js](https://www.nodejs.org) v4.4.3 及以上
2. [Mongodb](https://www.mongodb.org) v3.0.6 及以上

## 重新安装
1. 清空数据库
2. 删除 /install.lock
3. 访问 http://localhost:3000/admin/install 进入安装程序

## License
CMS is MIT licensed, as found in the LICENSE file.
