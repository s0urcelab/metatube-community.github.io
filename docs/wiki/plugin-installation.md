# Plugin installation (插件安装)

## 安装之前

请先确保当前的Jellyfin/Emby为**最新的**稳定版本，因为作者开发精力有限且Jellyfin/Emby的测试版本存在诸多不稳定性，所以本插件现在不会日后也不会提前支持这两个平台的beta版本。

在Jellyfin/Emby的beta测试版本中出现的插件无法识别，插件无法使用等问题，请勿在Issue中提问，亦不做任何解答，望谅解。

## Jellyfin

1. 进入 Jellyfin 控制台 > 插件 > 存储库，点击添加
2. 输入存储库名称：`MetaTube`
3. 输入存储库URL：[`https://raw.githubusercontent.com/metatube-community/jellyfin-plugin-metatube/dist/manifest.json`](https://raw.githubusercontent.com/metatube-community/jellyfin-plugin-metatube/dist/manifest.json)
4. 在插件目录下找到 MetaTube，点击安装
5. 重启Jellyfin

_适用于中国大陆的存储库URL：[`https://cdn.jsdelivr.net/gh/metatube-community/jellyfin-plugin-metatube@dist/manifest.json`](https://cdn.jsdelivr.net/gh/metatube-community/jellyfin-plugin-metatube@dist/manifest.json)（可能有缓存）_

## Emby

1. 从 [Releases](https://github.com/metatube-community/jellyfin-plugin-metatube/releases) 下载 MetaTube 最新插件
2. 解压出 MetaTube.dll 文件
3. 将 dll 文件复制到 Emby 插件目录
4. 重启 Emby 服务

PS：Emby 后续插件更新由计划任务在后台自动完成。

## 目录

常见的Emby插件目录如下：

- 群晖
  > /volume1/Emby/plugins
- Windows
  > emby\programdata\plugins
- Docker
  > <配置文件夹>/plugins
- Linux（供参考）
  > /var/lib/emby-server/plugins/
