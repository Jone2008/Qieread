<p align="center"><img alt="Water's github stats" src="https://github-readme-stats.vercel.app/api?username=Water008&show_icons=true&hide_border=true" /></p>

1.6 因作者删库停止更新，此库也停更。仅供留以后参考研究学习用。

1.5  qqreads.js修复获取cookies问题，qqreadnode修复QQREAD_CASH环境变量问题

1.4增加本仓库自动同步功能 只需设置secrets名：  PAT   
此处PAT需要申请，教程详见：https://www.jianshu.com/p/bb82b3ad1d11

1.3同步更新ziye12脚本，修复cookie失效继续阅读任务，实测也可以Actions运行，不过还是建议云函数运行。

12.30同步ziye12更新脚本，请务必添加新Secrets，name为QQREAD_CASH,值：可设置0 1 2 10 30 50 100 ，设置0即为默认不提现
同时Workflow下的yml文件增加env：QQREAD_CASH: ${{ secrets.QQREAD_CASH }}即可自动提现，不增加默认不提现

12.09凌晨经验证均已解决1金币问题

12.07同步更新ziye12脚本，解决1金币问题，请务必更新qqreads.js和qqread.yml两个文件，原来三个secrets中的一个QQREAD_HEADER请手动更改成QQREAD_BODY，删除后重新添加，抓取cookie代码已更改必须同步更新获取。三个值重新获取后填写，更新完成后手动运行下即可

BODY数值点击阅读小程序底下菜单栏“书库”进去读几秒书退出即可获取

企鹅阅读跑跑Actions

可直接fork仓库，然后设置里面分别添加如下三个secrets，值填写对应软件抓取的数据

QQREAD_BODY       对应值可直接复制所获取的{  }所有内容(包括大括号)，多账号换行

QQREAD_TIMEURL    对应值直接复制填入，多账号换行

QQREAD_TIMEHD     对应值可直接复制所获取的{  }所有内容(包括大括号)，多账号换行

然后常规run 对应yml文件即可，再不行不行的可以star一下。
