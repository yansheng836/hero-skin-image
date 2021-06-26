# Hero-Skin

本项目仅仅用于备份图片。

存储：

- Gitee：<https://gitee.com/yansheng0083/hero-skin-image>
- GitHub：<https://github.com/yansheng836/hero-skin-image>

访问照片：

![103澜-1-鲨之猎刃](https://cdn.jsdelivr.net/gh/yansheng836/hero-skin-image/5wallpaper-bigskin-images/103%E6%BE%9C-1-%E9%B2%A8%E4%B9%8B%E7%8C%8E%E5%88%83.jpg)

- [https://gitee.com/yansheng0083/hero-skin-image/blob/main/5wallpaper-bigskin-images/103澜-1-鲨之猎刃.jpg](https://gitee.com/yansheng0083/hero-skin-image/blob/main/5wallpaper-bigskin-images/103澜-1-鲨之猎刃.jpg)
- [https://gitee.com/yansheng0083/hero-skin-image/raw/main/5wallpaper-bigskin-images/103澜-1-鲨之猎刃.jpg](https://gitee.com/yansheng0083/hero-skin-image/raw/main/5wallpaper-bigskin-images/103澜-1-鲨之猎刃.jpg)

- [https://github.com/yansheng836/hero-skin-image/blob/main/5wallpaper-bigskin-images/104司空震-1-雷霆之王.jpg](https://github.com/yansheng836/hero-skin-image/blob/main/5wallpaper-bigskin-images/104司空震-1-雷霆之王.jpg)
- [https://raw.githubusercontent.com/yansheng836/hero-skin-image/main/5wallpaper-bigskin-images/104司空震-1-雷霆之王.jpg](https://raw.githubusercontent.com/yansheng836/hero-skin-image/main/5wallpaper-bigskin-images/104司空震-1-雷霆之王.jpg)
- [https://cdn.jsdelivr.net/gh/yansheng836/hero-skin-image/5wallpaper-bigskin-images/104司空震-1-雷霆之王.jpg](https://cdn.jsdelivr.net/gh/yansheng836/hero-skin-image/5wallpaper-bigskin-images/104司空震-1-雷霆之王.jpg)

## 英雄、皮肤数量

|         时间          | 英雄数量 | 皮肤数量 |
| :-------------------: | :------: | :------: |
|      2019-11-14       |    96    |   366    |
| 2021年1月30日23:41:04 |    96    |   422    |
| 2021年1月30日23:51:42 |   104    |   439    |
| 2021年6月26日19:05:57 |   106    |   470    |

## 王者荣耀

官网英雄介绍主页：<https://pvp.qq.com/web201605/herolist.shtml>

爬取王者荣耀的英雄皮肤图片，详情请看对应python仓库：<https://github.com/yansheng836/hero-skin-images>。

### 统计

到目前为止，王者荣耀一共有96个英雄，366个皮肤（含伴生皮肤）。

### 存在问题

爬取的网页数据不是最新的，如直接爬取最新的英雄为93，506，云中君；但是将该网页下载后再爬取，最新,96，523，西施。

处理方法：可以将网页先下载下来，爬取本地文件。

### bug

小图有一张有问题：

```
图片链接(https://game.gtimg.cn/images/yxzj/img201606/heroimg/142/142-bigskin-5.jpg)无效！响应状态码为：404
```

直接访问也是404。

### 辅助功能

统计英雄皮肤图片数量，拼接成json数据，为hexo博客提供每日切换背景图片的效果（现在有367张图片）。

主要程序：

- `DownloadBigskinWallpaper.java`：电脑壁纸，对应json：`wzry_mobile_367.json`
- `DownloadMobileskinWallpaper.java`：手机壁纸，对应json：`wzry_wallpaper367.json`

## 英雄联盟(LOL)

官网英雄介绍主页：<http://lol.qq.com/data/info-heros.shtml>

全部数据：<https://game.gtimg.cn/images/lol/act/img/js/heroList/hero_list.js>

单个英雄数据：`'//game.gtimg.cn/images/lol/act/img/js/hero/' + heroid + '.js'`

如：<http://game.gtimg.cn/images/lol/act/img/js/hero/1.js>

