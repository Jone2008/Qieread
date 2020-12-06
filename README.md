12.07同步更新ziye12脚本，解决1金币问题，请务必更新qqreads.js和qqread.yml两个文件，原来三个secrets中的一个QQREAD_HEADER请手动更改成QQREAD_BODY，删除后重新添加，值可用原来的，或者三个值重新获取，更新完成后手动运行下即可



企鹅阅读跑跑Actions

可直接fork仓库，然后设置里面分别添加如下三个secrets，值填写对应软件抓取的数据

QQREAD_BODY       对应值可直接复制所获取的{  }所有内容(包括大括号)，多账号换行

QQREAD_TIMEURL    对应值直接复制填入，多账号换行

QQREAD_TIMEHD     对应值可直接复制所获取的{  }所有内容(包括大括号)，多账号换行

然后常规run 对应yml文件即可，再不行不行的可以star一下。
