# xiaoli-cli-operit-plugins

存放使用 **Operit 协议**的插件脚本，供 [xiaoli-cli](https://gitee.com/shuiyu1123/xiaoli-cli) 的 `operit_bridge` 插件调用。

## 结构说明

```
xiaoli-cli-operit-plugins/
├── scripts/               # Operit 格式的 .ts 插件脚本
│   ├── 12306.ts
│   ├── google_search.ts
│   ├── browser.ts
│   └── ... (共 47 个脚本)
├── operit_bridge.py       # xiaoli-cli 桥接插件（参考实现）
└── README.md
```

## 脚本来源

本仓库中的 `scripts/` 目录包含来自 [Operit AI 项目](https://github.com/AAswordman/Operit) 社区的第三方工具脚本。

- 原项目: https://github.com/AAswordman/Operit
- 许可证: LGPL-3.0

## 使用方法

在 xiaoli-cli 中配置 `operit_bridge` 插件，将本仓库克隆或下载到 `plugins/operit/` 目录：

```bash
git clone https://gitee.com/shuiyu1123/xiaoli-cli-operit-plugins.git /path/to/xiaoli-cli/plugins/operit-ext
```

然后通过 `operit_bridge scan` 命令扫描加载即可。

## 许可证

`scripts/` 目录下的脚本遵守其原始项目的 **LGPL-3.0** 许可证。
`operit_bridge.py` 遵循 **MIT** 许可证。