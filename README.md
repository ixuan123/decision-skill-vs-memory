# decision-skill-vs-memory

> 🧠 AI 助手决策工具：判断任务该存成 **Skill**（可复用技能）还是 **Memory**（临时记忆）

## 一句话解释

帮 AI 判断每次完成任务后，经验该存哪——存成 **Skill**（可复用技能）还是 **Memory**（临时记忆）。

---

## 🤔 为什么需要这个？

AI 助手每天完成很多任务，但每次都要重新想：

> "这个经验要不要保存？存哪？"

存错了会出问题：

| 错误 | 后果 |
|------|------|
| 该存 Skill 的存成了 Memory | 下次还要重新做一遍，重复劳动 |
| 该存 Memory 的做成了 Skill | Skill 仓库越来越臃肿，全是垃圾 |

---

## 📋 决策流程

```
任务完成
   │
   ▼
下次还会遇到吗？── 不──→ 存 Memory 📝
   │
   会
   │
   ▼
别人也能用吗？── 不──→ 存 Memory 📝
   │
   能
   │
   ▼
步骤固定吗？── 不──→ 存 Memory 📝
   │
   固定
   │
   ▼
  存 Skill ✅
```

---

## 🎯 实际例子

| 任务 | 存哪 | 为什么 |
|------|------|--------|
| Chrome CDP 读抖音 | ✅ Skill | 步骤固定，下次还能用 |
| Tavily API Key | 📝 Memory | 只是配置信息 |
| "不要重启 gateway" | 📝 Memory | 规则，不重复 |
| 删除重复 skill | 📝 Memory | 一次性的操作 |
| 横纵分析法 | ✅ Skill | 方法论，可复用 |
| Windows 编码踩坑 | 📝 Memory | 教训，不重复 |

---

## 💡 核心理念

> **Skill 是"怎么做"，Memory 是"发生了什么"。**
>
> - Skill 教我下次怎么做
> - Memory 让我记住这次经历了什么

---

## 📦 安装

```bash
clawhub install decision-skill-vs-memory
```

或手动安装：

```bash
git clone https://github.com/ixuan123/decision-skill-vs-memory.git
cp -r decision-skill-vs-memory skills/
```

---

_由 [OpenClaw](https://github.com/openclaw/openclaw) 社区贡献_
