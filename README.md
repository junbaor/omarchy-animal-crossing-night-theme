# 🌙 动物森友会-夜 · Animal Crossing Night for Omarchy

[**动物森友会**（白天版）](https://github.com/junbaor/omarchy-animal-crossing-theme)的夜间姊妹主题：月光下的深蓝小岛、萤火虫与栈桥暖灯。慢一点也没关系，晚安村。

![主题预览](preview.png)

## 壁纸

| 星夜小岛 | 月光草原 | 夜灯栈桥 |
|:---:|:---:|:---:|
| ![星夜小岛](backgrounds/1-island-night.png) | ![月光草原](backgrounds/2-meadow-night.png) | ![夜灯栈桥](backgrounds/3-pier-night.png) |

切换壁纸：`omarchy theme bg next`

## 安装

```bash
omarchy theme install https://github.com/junbaor/omarchy-animal-crossing-night-theme
```

安装后主题名为 `animal-crossing-night`。想要中文主题名的话：

```bash
mv ~/.config/omarchy/themes/animal-crossing-night ~/.config/omarchy/themes/动物森友会-夜
omarchy theme set 动物森友会-夜
```

## 配色

| 角色 | 色值 | 说明 |
|---|---|---|
| 背景 | `#1F2A33` | 月夜深蓝 |
| 强调 | `#7CC85C` | 萤光叶绿 |
| 前景 | `#E6DEC8` | 月光米 |
| 黄 | `#F2C94C` | 暖灯金（路灯/铃铛 🔔） |
| 蓝 | `#6FB6DC` | 夜海蓝 |
| 红 | `#E8756A` | 珊瑚红 |
| 紫 | `#D98BB5` | 花瓣紫 |
| 青 | `#5FBFC4` | 萤火青 |
| 棕 | `#A9846A` | 夜木棕 |

完整配色见 [colors.toml](colors.toml)，所有前景色按 WCAG 对比度（≥ 4.5:1）校准过。

## 配套主题

- ☀️ 白天版：[omarchy-animal-crossing-theme](https://github.com/junbaor/omarchy-animal-crossing-theme)

白天用奶油色小岛，晚上切到星夜萤火，`omarchy theme switcher` 一键换。

## 自定义

1. 编辑 `~/.config/omarchy/themes/<主题名>/colors.toml`
2. 运行 `omarchy theme refresh` 重新生成所有应用配置

终端、Neovim、btop、VS Code、GTK、fcitx5、菜单/通知/锁屏等配置都会从 `colors.toml` 自动生成。

## 文件结构

```
├── colors.toml        # 核心配色（其余配置由 Omarchy 模板生成）
├── backgrounds/       # 三张 2560×1440 原创夜景壁纸
├── sources/           # 壁纸的 SVG 源文件，欢迎改色再创作
├── preview.png        # 主题选择器预览图
├── icons.theme        # 图标包（Yaru-olive-dark）
├── keyboard.rgb       # 键盘背光颜色
├── unlock.png         # Plymouth 开机画面 logo（萤光绿）
└── preview-unlock.png # 开机画面预览
```

想让开机画面也变成星夜：菜单 → 样式 → Unlock，或运行
`sudo omarchy-plymouth-set-by-theme animal-crossing-night`

## 相关链接

- [Omarchy](https://omarchy.org/) · [主题文档](https://github.com/basecamp/omarchy)
- 壁纸为原创矢量插画（SVG 源码在 `sources/`），可自由修改使用

## License

[MIT](LICENSE)
