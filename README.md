# hero-skin-image

本项目仅仅用于备份王者荣耀的皮肤图片。

爬虫详见：

- Gitee：<https://gitee.com/yansheng0083/hero-skin>
- GitHub：<https://github.com/yansheng836/hero-skin>

## 存在问题

### 2025年2月8日 停用Gitee仓库

因为仓库太大了，而个人版Gitee有总仓库1GB大小限制，故不再存储到Gitee。

### 2025年2月8日 更新html，发现有英雄被删除

发现有英雄被删除：成吉思汗，导致后面的英雄顺序发生了变化，重复下载了。

补全：手动在“杨戬”后面加上了。

```html
<li><a href="https://pvp.qq.com/web201605/herodetail/chengjisihan.shtml" target="_blank"><img src="./英雄资料列表页-英雄介绍-王者荣耀官方网站-腾讯游戏_files/177.jpg" width="91" height="91" alt="成吉思汗">成吉思汗</a></li>
```

## 王者荣耀

官网英雄介绍主页：<https://pvp.qq.com/web201605/herolist.shtml>

![1624789982833](assets/1624789982833.png)

### 统计

ps:~~2023年4月30日00:18:05 发现好像英雄数据一直都不变，不知道是不是JSON变了，后面再排查下。~~

~~2023年04月30日01:00:28：更新主页信息（即重新下载HTML文件），使新英雄生效。~~

2026年2月27日21:25:50，使用新版 [hero-skin-1.0.4-wzry.jar](./hero-skin-1.0.4-wzry.jar) 重新下载所有壁纸（新版英雄名不再排序）。

|          时间          | 英雄数量 | 皮肤数量 | 1phone | 2phone | 3phone | 4wallpaper | 5wallpaper |
| :--------------------: | :------: | :------: | :----: | :----: | :----: | :--------: | :--------: |
|     2019年11月14日     |    96    |   366    |        |        |        |            |            |
| 2021年01月30日23:41:04 |    96    |   422    |        |        |        |            |            |
| 2021年01月30日23:51:42 |   104    |   439    |        |        |        |            |            |
| 2021年06月26日19:05:57 |   106    |   470    |        |        |        |            |            |
| 2021年10月21日08:12:19 |   106    |   490    |        |        |        |            |            |
| 2022年03月26日16:15:39 |   106    |   519    |        |        |        |            |            |
| 2023年04月30日00:15:18 |   106    |   600    |        |        |        |            |            |
| 2023年04月30日01:00:14 |   114    |   617    |        |        |        |            |            |
| 2023年07月09日02:00:04 |   115    |   632    |        |        |        |            |            |
| 2024年09月27日02:27:12 |   123    |   752    |  752   |  747   |  748   |    750     |    752     |
| 2025年12月14日18:23:38 |   124    |   861    |  861   |  854   |  855   |    860     |    861     |
| 2026年2月27日21:23:30  |   134    |   892    |  892   |  892   |  892   |    892     |    892     |

### 存储

- Gitee：<https://gitee.com/yansheng0083/hero-skin-image>
- GitHub：<https://github.com/yansheng836/hero-skin-image>

### 访问照片的方式

![澜-1-鲨之猎刃](https://raw.githubusercontent.com/yansheng836/hero-skin-image/main/5wallpaper-bigskin-images/司空震-1-雷霆之王.jpg)

- WEB版：<https://github.com/yansheng836/hero-skin-image/blob/main/5wallpaper-bigskin-images/司空震-1-雷霆之王.jpg>
- 原图版：<https://raw.githubusercontent.com/yansheng836/hero-skin-image/main/5wallpaper-bigskin-images/司空震-1-雷霆之王.jpg>
- CDN版：<https://cdn.jsdelivr.net/gh/yansheng836/hero-skin-image/5wallpaper-bigskin-images/司空震-1-雷霆之王.jpg>

