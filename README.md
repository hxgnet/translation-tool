# 星联语翻译系统

纯前端实现的「中文 / 拼音 ↔ 星联语」双向转换工具，单文件 `index.html`，无需任何后端与依赖，打开即用。

## 功能

- **翻译转换**：输入中文或带声调/数字声调的拼音，自动转换为星联语；也支持星联语反查拼音
- **训练模式**：看星联猜拼音、看拼音写星联、转换过程训练，并统计正确率
- **星联词典**：声母 / 韵母 / 组合音节分类表格，支持搜索与定位
- **使用教程**：内置转换规则说明
- **本地历史与自动保存**：翻译记录保存在浏览器 localStorage，刷新不丢失

## 使用方法

直接用浏览器打开 `index.html`：

```bash
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

也可以把仓库发布到 GitHub Pages：`Settings → Pages → Branch: main / root`，然后访问
`https://hxgnet.github.io/translation-tool/`。

### 输入示例

| 输入 | 说明 |
| --- | --- |
| `你好世界` | 中文直接输入 |
| `nǐ hǎo` / `ni3 hao3` | 带声调或数字声调拼音 |
| `einu aeoho` | 星联语，反向还原拼音 |

快捷键：`Ctrl + Enter` 触发翻译。

## 项目结构

```
translation-tool/
├── index.html   # 全部界面、样式与转换逻辑（自包含，无外部依赖）
└── README.md
```

## 说明

- 转换规则、词典数据全部内置于 `index.html`，不访问任何网络接口，不收集用户数据
- 版权归原作者所有：制作者 argza ionmo iainxix、虎孝服务、G网工作室
