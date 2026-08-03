# 天坛家具公文格式 — Claude Code Skill

为 [Claude Code](https://claude.ai/code) 定制的 Word 文档生成技能，按照天坛家具公文格式标准创建正式 `.docx` 文件。

内置**两套模板**，共享同一套正文格式规范，根据用户请求自动切换。

## 模板

| 触发词 | 模板 | 特点 |
|--------|------|------|
| "冬奥"、"奥运" | 冬奥品牌模板 | 页眉页脚带冬奥 logo 和品牌底图 |
| 默认 | 通用模板 | 标准公文格式，无品牌元素 |

## 安装

```bash
git clone https://github.com/pescadosalado/tiantan-general-word-format.git ~/.claude/skills/tiantan-word-format
```

重启 Claude Code 即可自动识别。

## 使用

```bash
# 通用模板
"用通用word格式输出一份xxx汇报"

# 冬奥品牌模板
"用冬奥word模版输出一份xxx汇报，需要2个附件"
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
| 成文日期 | 仿宋\_GB2312 | 三号 16pt | 以发文单位名为基准居中 |
| 联系人 | 仿宋\_GB2312 | 三号 16pt | 首行左空2字符，续行顶格 |

- 固定行距：**28pt**，首行缩进 2 字符

## 目录结构

```
├── SKILL.md                          # 技能定义
├── README.md
├── LICENSE
└── assets/
    ├── reference.docx                 # 通用格式参考模板
    ├── reference-winter-olympics.docx  # 冬奥品牌参考模板
    ├── FZXBSJW.TTF                    # 方正小标宋简体
    ├── simfang-仿宋GB.ttf              # 仿宋_GB2312
    └── 楷体_GB2312.ttf                 # 楷体_GB2312
```

## 许可

MIT
