# Clear Thinking

A Codex skill for making clearer, more deliberate, and more risk-aware decisions.

[简体中文](README.zh-CN.md)

## Overview

Clear Thinking is a Codex skill for decision analysis, option comparison, risk control, action planning, and post-decision review. It helps you notice default reactions, define the real problem, compare meaningful alternatives, and turn a decision into bounded action.

## Core framework

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

## Installation

Copy the repository into your user-level Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R clear-thinking ~/.codex/skills/
```

Or clone it directly:

```bash
git clone https://github.com/guangfuhao/clear-thinking-skill.git ~/.codex/skills/clear-thinking
```

## Usage

Explicit invocation:

```text
$clear-thinking Compare these options and show the key assumptions, risks, low-cost experiments, and review points.
```

Natural-language invocation:

```text
I am considering leaving my job to start a business. Help me analyze the decision with Clear Thinking.
```

## Repository structure

```text
SKILL.md                              # Skill entry point and workflow
references/decision-playbook.md      # Decision cards, matrices, and review templates
agents/openai.yaml                   # Codex UI metadata and invocation policy
```

## Scope and safety

This skill improves the reasoning process; it does not make the final decision for the user. High-stakes medical, legal, financial, and career decisions should be checked with appropriate professionals. It does not perform irreversible external actions such as placing orders, signing contracts, resigning, or sending formal notices without explicit authorization.
