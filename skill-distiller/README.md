帮小白把自己的业务场景一步步变成可用的 Skill。

从空格丶 (zephyrwang6) 9 篇 AI Skill 方法论文章蒸馏而来，用大白话引导，6 步走完就能上手。

## 5 条路线

| 路线 | 适用情况 |
|---|---|
| A · 拿最好的当模板 | 你有满意的成果样本 |
| B · 把步骤串起来 | 每次都按固定步骤做 |
| C · 翻聊天记录找规律 | 说不清但老在重复做 |
| D · 把规矩变成文件 | 脑子里有规则但没写下来 |
| E · 按你的岗位来拆 | 什么都没有，只知道职业 |

## 安装

```bash
cp -r skill-distiller ~/.hermes/skills/
```

## 使用

对 AI 说：
- "帮我做一个 Skill"
- "我想把 xxx 自动化"
- "我每次都重复做 xxx，能不能让 AI 来"
- "帮我拆一下我的岗位/工作"

## 结构

```
skill-distiller/
├── SKILL.md                         ← 主流程（6步引导）
├── CHANGELOG.md                     ← 改动记录
├── feedback-log.md                  ← 用户反馈
├── references/                      ← 路线详情 + 检查清单
│   ├── route-a-best-sample.md
│   ├── route-b-steps.md
│   ├── route-c-chat-history.md
│   ├── route-d-tacit-rules.md
│   ├── route-e-career.md
│   ├── quality-checklist.md
│   └── learning-notes.md
├── templates/                       ← 生成的 Skill 模板
│   ├── skill-template.md
│   ├── rules-template.md
│   ├── usage-log-template.md
│   └── skill-checkup.md
└── scripts/
    └── learn-and-update.md          ← 学习新资料的流程
```

## 致谢

方法论来源于 [空格丶](https://github.com/zephyrwang6) 的 9 篇公众号文章。
