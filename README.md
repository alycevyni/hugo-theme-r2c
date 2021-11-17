# hugo-theme-r2c

一个简洁双栏布局主题，支持暗黑/明亮模式。适配移动端和 `meta` SEO 优化。

- 瀑布流相册
- 图片的 `alt` 文字展示
- 插入视频
- 灯箱效果

![light theme](https://i.imgur.com/5VXUBG5.png)

明亮模式

![dark theme](https://i.imgur.com/GznKevO.png)

暗黑模式

## 配置

`config.toml` 文件里有一些简单配置选项：

| 字段 | 描述 |
| :---- | :---- |
| sitename | 站点名 |
| description | 站点描述 |
| keywords | 站点关键字 |
| twitter | 推特完整地址 |
| weibo | 微博完整地址 |
| github | Github 完整地址 |
| cover | 默认站点的封面图 |
| icp | 备案号 |

### shortcodes 的一些使用方法：

`figure` 是横向并列的两张图片展示

```html
{{ figure img1="图片地址" img2="图片地址" title="文字描述（可选内容）" }}
```

`gallery` 是瀑布流的图片展示，图片地址之间请用 `'` 包裹并使用空格隔开

```html
{{ gallery '图片地址1' '图片地址2' '图片地址3' ... '图片地址N' }}
```

`img` 是支持灯箱效果的图片

```html
{{ img src="图片地址" alt="描述文字（可选）" }}
```

`steam` 是一种卡片展示 steam 游戏介绍的特殊排版

```html
{{ steam title="游戏名" id="游戏ID" desc="文字描述" }}
```

`video` 插入 MP4 视频，`autoplay` 自动播放（可选），`loop` 循环（可选），`muted` 静音可选。

```html
{{ video src="视频地址" autoplay loop muted }}
```
