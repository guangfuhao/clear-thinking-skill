# Clear Thinking

A Codex skill for making clearer, more deliberate, and more risk-aware decisions.

## 中文

### 概述

“清晰思考”是一套用于决策分析、方案比较、风险控制、行动规划和复盘的 Codex skill。它帮助你识别默认反应，重新定义真正的问题，比较不同选项，并把决定转化为有边界的行动。

### 核心框架

1. **识别默认反应**：情绪、自负、合群和惯性。
2. **采用强者思维**：自我问责、自我认知、自我控制，以及不等于自负的自信。
3. **设定高标准**：明确成功标准、价值排序和不可接受的结果。
4. **执行决策流程**：
   - 定义问题与根因
   - 至少提出三个实质不同的方案
   - 根据标准、证据和专家意见评估
   - 结合可逆性与信息边际价值决定行动时机
   - 设置安全边际、止损条件和回退路径
   - 记录决策并复盘过程
5. **先子弹后炮弹**：先用低成本、可逆的实验验证关键假设，再投入不可逆资源。

低后果、可逆的事项可以使用轻量模式；复杂、重要或不可逆的事项可以使用完整决策工作台。

### 安装

将仓库目录复制到 Codex 的用户级 skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R clear-thinking ~/.codex/skills/
```

也可以直接克隆：

```bash
git clone https://github.com/guangfuhao/clear-thinking.git ~/.codex/skills/clear-thinking
```

### 使用

显式调用：

```text
$clear-thinking 帮我比较这三个方案，列出关键假设、风险、低成本试验和复盘节点。
```

自然语言调用：

```text
我在考虑是否辞职创业，请用清晰思考框架帮我分析。
```

### 文件结构

```text
SKILL.md                              # 技能入口与工作流程
references/decision-playbook.md      # 决策卡、评估矩阵和复盘日志模板
agents/openai.yaml                   # Codex 界面元数据与调用策略
```

### 使用边界

这个 skill 用于改善思考过程，不替用户做最终决定。对医疗、法律、投资和重大职业变动等高风险问题，应补充合适的专业核验。未经明确授权，不执行下单、签约、辞职或发送正式通知等外部不可逆行动。

## English

### Overview

Clear Thinking is a Codex skill for decision analysis, option comparison, risk control, action planning, and post-decision review. It helps you notice default reactions, define the real problem, compare meaningful alternatives, and turn a decision into bounded action.

### Core framework

1. **Detect default reactions**: emotion, ego, conformity, and inertia.
2. **Adopt a stronger posture**: self-accountability, self-awareness, self-control, and confidence without ego.
3. **Set high standards**: define success, priorities, and unacceptable outcomes.
4. **Run the decision process**:
   - Define the problem and its root cause
   - Generate at least three materially different options
   - Evaluate them against explicit standards and reliable expertise
   - Decide when to act using reversibility and the marginal value of information
   - Add safety margins, stop conditions, and fallback paths
   - Record the decision and review the process
5. **Use bullets before cannon**: validate key assumptions with a small, reversible experiment before committing irreversible resources.

Use the lightweight mode for low-consequence, reversible choices. Use the full decision worksheet for complex, consequential, or irreversible choices.

### Installation

Copy the repository into your user-level Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R clear-thinking ~/.codex/skills/
```

Or clone it directly:

```bash
git clone https://github.com/guangfuhao/clear-thinking.git ~/.codex/skills/clear-thinking
```

### Usage

Explicit invocation:

```text
$clear-thinking Compare these options and show the key assumptions, risks, low-cost experiments, and review points.
```

Natural-language invocation:

```text
I am considering leaving my job to start a business. Help me analyze the decision with Clear Thinking.
```

### Repository structure

```text
SKILL.md                              # Skill entry point and workflow
references/decision-playbook.md      # Decision cards, matrices, and review templates
agents/openai.yaml                   # Codex UI metadata and invocation policy
```

### Scope and safety

This skill improves the reasoning process; it does not make the final decision for the user. High-stakes medical, legal, financial, and career decisions should be checked with appropriate professionals. It does not perform irreversible external actions such as placing orders, signing contracts, resigning, or sending formal notices without explicit authorization.
