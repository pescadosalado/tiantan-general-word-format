# 天坛家具 Word 公文模版 · Tiantan Furniture Word Templates

天坛家具公司日常使用的 Claude Code Word 模版技能，内置两套模版，共享同一套公文格式规范。

A Claude Code skill for creating formal Word documents at Tiantan Furniture. Two templates, one formatting standard.

---

## 两套模版 · Two Templates

| 触发词 Trigger | 模版 Template | 说明 Description |
|------|------|------|
| `冬奥word` | 🏔️ 冬奥品牌模版 | 页眉页脚带冬奥 logo 和品牌底图 / Winter Olympics branded header & footer |
| `通用word` | 📄 通用模版 | 标准公文格式，无品牌元素 / Standard format, no branding |

两套模版的正文、标题、落款、联系人格式**完全一致**，仅品牌元素不同。

Both templates share the **exact same** formatting rules for body text, headings, signatures, and contacts. The only difference is the branding.

---

## 安装 · Install

```bash
git clone https://github.com/pescadosalado/tiantan-general-word-format.git ~/.claude/skills/tiantan-general-word-format
```

重启 Claude Code 即可 / Restart Claude Code after installation.

---

## 使用 · Usage

### 中文

```
# 通用模版
用通用word输出一份数字化转型工作汇报

# 冬奥品牌模版（带 logo）
用冬奥word输出一份项目汇报，需要2个附件
```

### English

```
# General template
"Generate a digital transformation report using the general word format"

# Winter Olympics branded template
"Generate a project report using the winter olympics word template"
```

---

## 格式规范 · Format Spec

| 元素 Element | 字体 Font | 大小 Size |
|------|------|------|
| 主标题 Title | 方正小标宋简体 | 小二号 18pt |
| 一级标题 H1 ("一、...") | 黑体 | 三号 16pt |
| 二级标题 H2 ("（一）...") | 楷体_GB2312 | 三号 16pt |
| 三级标题 H3 ("1....") | 仿宋_GB2312 | 三号 16pt |
| 正文 Body | 仿宋_GB2312 | 三号 16pt |
| 落款 Signature | 仿宋_GB2312 | 三号 16pt |
| 联系人 Contact | 仿宋_GB2312 | 三号 16pt |

- 固定行距 Line spacing: **28pt**
- 首行缩进 First-line indent: 2 字符

---

## 目录结构 · Structure

```
├── SKILL.md                                     # 技能定义
├── README.md
├── LICENSE (MIT)
└── assets/
    ├── reference.docx                            # 通用模版
    ├── reference-winter-olympics.docx             # 冬奥模版
    ├── FZXBSJW.TTF
    ├── simfang-仿宋GB.ttf
    └── 楷体_GB2312.ttf
```

## 许可 · License

MIT
