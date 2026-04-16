# skill-distiller

帮小白把自己的业务场景一步步变成可用的 Skill。

从空格丶 (zephyrwang6) 9 篇 AI Skill 方法论文章蒸馏而来，用大白话引导，6 步走完就能上手。

## 安装

```bash
# 方式1：从 cloud-skill 仓库复制
git clone https://github.com/Yunxj/cloud-skill.git
cp -r cloud-skill/skill-distiller ~/.hermes/skills/

# 方式2：直接下载这个 Skill
git clone -n --depth 1 --filter=blob:none https://github.com/Yunxj/cloud-skill.git \
  && cd cloud-skill \
  && git checkout HEAD -- skill-distiller \
  && cp -r skill-distiller ~/.hermes/skills/
```

## 使用方法

安装完成后，对 AI 说以下任意一句就能启动：

- "帮我做一个 Skill"
- "我想把 xxx 自动化"
- "我每次都重复做 xxx，能不能让 AI 来"
- "帮我拆一下我的岗位/工作"

### 它会带你走 6 步

| 步骤 | 做什么 | 你需要做什么 |
|---|---|---|
| 1. 聊清楚你想干嘛 | 问你 3 个问题搞清需求 | 用自己的话说就行 |
| 2. 选最适合你的路线 | 自动匹配 5 条路线之一 | 确认就行，不用自己选 |
| 3. 带着你一步步做出来 | 引导你补充输入/输出/规矩/标准 | 回答 4 个必答问题 |
| 4. 帮你检查一遍 | 按 4 大类检查清单逐项过 | 看结果，有问题的直接帮你改 |
| 5. 装好就能用 | 告诉你怎么安装和试跑 | 跟着做就行 |
| 6. 越用越好 | 内置使用记录和定期体检机制 | 说"记一笔"或"体检报告" |

### 5 条路线（自动匹配，你不需要知道怎么选）

| 路线 | 适用情况 |
|---|---|
| A · 拿最好的当模板 | 你有满意的成果样本 |
| B · 把步骤串起来 | 每次都按固定步骤做 |
| C · 翻聊天记录找规律 | 说不清但老在重复做 |
| D · 把规矩变成文件 | 脑子里有规则但没写下来 |
| E · 按你的岗位来拆 | 什么都没有，只知道职业 |

### 让它学习新东西

随时丢资料给它，说"学一下这个"就行：
- 文章链接 / PDF
- 别人的 Skill 文件
- 方法论笔记

它会自动提取有价值的内容，更新自己的引导能力。

## 结构说明

```
skill-distiller/
├── SKILL.md                         ← 主文件，AI 读取的引导流程
├── CHANGELOG.md                     ← 版本改动记录
├── feedback-log.md                  ← 用户反馈记录
├── references/                      ← 详细参考资料
│   ├── route-a-best-sample.md       ← 路线A详细引导
│   ├── route-b-steps.md             ← 路线B详细引导
│   ├── route-c-chat-history.md      ← 路线C详细引导
│   ├── route-d-tacit-rules.md       ← 路线D详细引导
│   ├── route-e-career.md            ← 路线E详细引导
│   ├── quality-checklist.md         ← 质量检查清单
│   └── learning-notes.md            ← 学习笔记
├── templates/                       ← 生成的 Skill 用到的模板
│   ├── skill-template.md            ← Skill 主文件模板
│   ├── rules-template.md            ← 规则文件模板
│   ├── usage-log-template.md        ← 使用日志模板
│   └── skill-checkup.md             ← 体检报告模板
└── scripts/
    └── learn-and-update.md          ← 学习新资料的处理流程
```

## 致谢

方法论来源于 [空格丶](https://github.com/zephyrwang6) 的 9 篇公众号文章。
