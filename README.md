# 天坛家具通用公文格式 — Claude Code Skill

为 [Claude Code](https://claude.ai/code) 定制的 Word 文档生成技能，按照天坛家具通用公文格式标准创建正式 `.docx` 文件。

## 适用场景

- 公司内部汇报、项目汇报、专题汇报
- 会议纪要
- 请示、报告等正式公文
- 其他需要统一格式的公司材料

## 安装

```bash
# 克隆到 Claude Code skills 目录
git clone https://github.com/YOUR_USERNAME/tiantan-general-word-format.git ~/.claude/skills/tiantan-general-word-format
```

重启 Claude Code 即可自动识别。

## 使用

对话中直接说：

```
用通用word格式skill，帮我写一份关于XXX的汇报
```

或使用斜杠命令：

```
/tiantan-general-word-format 写一份数字化转型工作汇报，需要2个附件
```

## 格式规范

| 元素 | 字体 | 字号 | 对齐 |
|------|------|------|------|
| 主标题 | 方正小标宋简体 | 小二号 18pt | 居中 |
| 一级标题 | 黑体 | 三号 16pt | 两端对齐 |
| 二级标题 | 楷体\_GB2312 | 三号 16pt | 两端对齐 |
| 三级标题 | 仿宋\_GB2312 | 三号 16pt | 两端对齐 |
| 正文 | 仿宋\_GB2312 | 三号 16pt | 两端对齐 |
| 发文单位 | 仿宋\_GB2312 | 三号 16pt | 右对齐，右空2字符 |
| 成文日期 | 仿宋\_GB2312 | 三号 16pt | 右对齐，以发文单位居中 |
| 联系人 | 仿宋\_GB2312 | 三号 16pt | 首行左空2字符 |

### 段落

- 固定行距：**28pt**
- 首行缩进：2 字符
- 页面：A4，左边距 28mm，右边距 26mm，上下 25.4mm

## 目录结构

```
tiantan-general-word-format/
├── SKILL.md                # 技能定义（Claude Code 识别入口）
├── README.md
└── assets/
    ├── reference.docx       # 通用格式参考模板
    ├── FZXBSJW.TTF          # 方正小标宋简体
    ├── simfang-仿宋GB.ttf    # 仿宋_GB2312
    └── 楷体_GB2312.ttf       # 楷体_GB2312
```

## 许可

MIT
