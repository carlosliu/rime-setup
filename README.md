
# Rime 配置说明

[Rime](https://github.com/rime) 输入法是一款适用于 Mac OS X、Linux 和 Windows 的输入法，Rime 在不同平台下的对应名称如下：

* Mac OS X: 鼠鬚管([Squirrel](https://github.com/rime/squirrel))  
    配置目录：`~/Library/Rime/`
* Linux: 中州韻([ibus-rime](https://github.com/rime/ibus-rime))  
    配置目录：`~/.config/ibus/rime/`
* Windows: 小狼毫([Weasel](https://github.com/rime/weasel))  
    配置目录：`%APPDATA%\Rime`

Rime 的配置文件不同平台的放置在不同的目录，在配置目录中，主要使用 `yaml` 进行配置。目录中自有的配置文件不建议直接修改，因为可能会被自动复写。用户配置一般以原始配置文件名增加 .custom 二级后缀的方式，例如：Mac OSX 下的原始配置 `squirrel.yaml`，对应的用户配置就是 `squirrel.custom.yaml` 文件。

修改 `.custom` 配置后，『重新部署』Rime 输入法会将用户的配置增加或更新到对应的原始配置中。

## 安裝

```
$ git clone https://github.com/carlosliu/rime-setup
$ cd rime-setup
$ make install
```

## 卸載

```
$ cd rime-setup
$ make uninstall
```

## 同步

installation.yaml

```yaml
installation_id: "carlos.mbp"
sync_dir: "/Users/carlos/Dropbox/Apps/Rime"
```


## 参考
* [Rime 定製指南](https://github.com/rime/home/wiki/CustomizationGuide)
* [中州韵（小狼毫，鼠须管）输入法设置](http://blog.yesmryang.net/rime-setting/)
* [說明書#同步用戶資料](https://github.com/rime/home/wiki/UserGuide#同步用戶資料)
* [Author:佛振(lotem)@github](https://github.com/lotem)
* [如何从QIM迁移至Squirrel（鼠鬚管）](http://cocoabob.net/?p=919)
