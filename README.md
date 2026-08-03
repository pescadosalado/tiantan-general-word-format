# 天坛家具 Word 公文模版 · Tiantan Furniture Word Templates

天坛家具公司日常使用的 Claude Code Word 模版技能。支持**三种文档类型** × 两套品牌模版，共享同一套公文格式规范。

A Claude Code skill for creating formal Word documents at Tiantan Furniture. Three document types × two brand templates, one formatting standard.

---

## 文档类型 · Document Types

| 触发词 Trigger | 类型 Type | 说明 Description |
|------|------|------|
| `会议纪要`、`专题会纪要`、`会议记录` | 📋 会议纪要 | 标题 + 会议信息（时间/地点/人员）+ 会议内容 / Meeting minutes with structured info fields |
| `汇报`、`报告`、`请示`、`通知` 等（默认） | 📄 通用公文 | 标题 + 正文 + 各级标题 / Standard report with heading hierarchy |

## 品牌模版 · Brand Templates

| 触发词 Trigger | 模版 Template | 说明 Description |
|------|------|------|
| `冬奥word` | 🏔️ 冬奥品牌 | 页眉页脚带冬奥 logo 和品牌底图 / Winter Olympics branded |
| `通用word` 或无关键词 | 📄 通用格式 | 标准公文格式，无品牌元素 / Standard format, no branding |

**示例 · Examples：**

```
# 通用格式 + 通用公文
用通用word输出一份数字化转型工作汇报，需要2个附件

# 通用格式 + 会议纪要
用通用word生成一份专题会议纪要

# 冬奥品牌 + 通用公文
用冬奥word输出一份项目汇报

# 冬奥品牌 + 会议纪要
用冬奥word生成一份部门专题会纪要
```

---

## 安装 · Install

```bash
git clone https://github.com/pescadosalado/tiantan-general-word-format.git ~/.claude/skills/tiantan-general-word-format
```

重启 Claude Code 即可 / Restart Claude Code after installation.

---

## 格式规范 · Format Spec

| 元素 Element | 字体 Font | 大小 Size |
|------|------|------|
| 主标题 Title | 方正小标宋简体 | 小二号 18pt |
| 一级标题 H1 ("一、...") | 黑体 | 三号 16pt |
| 二级标题 H2 ("（一）...") | 楷体_GB2312 | 三号 16pt |
| 三级标题 H3 ("1....") | 仿宋_GB2312 | 三号 16pt |
| 会议信息字段 Meeting Info | 黑体(标签) + 仿宋(内容) | 三号 16pt |
| 正文 Body | 仿宋_GB2312 | 三号 16pt |
| 落款 Signature | 仿宋_GB2312 | 三号 16pt |
| 联系人 Contact | 仿宋_GB2312 | 三号 16pt |

- 固定行距 Line spacing: **28pt**
- 首行缩进 First-line indent: 2 字符

---

## 目录结构 · Structure

```
├── SKILL.md                                       # 技能定义
├── README.md
├── LICENSE (MIT)
└── assets/
    ├── reference.docx                              # 通用公文 · 通用格式
    ├── reference-winter-olympics.docx               # 通用公文 · 冬奥品牌
    ├── reference-meeting-minutes.docx               # 会议纪要 · 通用格式
    ├── reference-meeting-minutes-winter-olympics.docx # 会议纪要 · 冬奥品牌
    ├── FZXBSJW.TTF
    ├── simfang-仿宋GB.ttf
    └── 楷体_GB2312.ttf
```

## 许可 · License

MIT

---

## 联系 · Contact

👤 **pescadosalado** · [GitHub](https://github.com/pescadosalado)

欢迎使用、提建议、交流反馈。如果这个模版对你有帮助，请点个 ⭐ Star！

Welcome to use, share feedback, and contribute. If you find this useful, a ⭐ star is much appreciated!
