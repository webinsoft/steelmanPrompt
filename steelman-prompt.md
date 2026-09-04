# Steelman 决策分析提示词模板 / Steelman Decision Analysis Prompt

> ## 参数输入 / Parameter Input
> 将下方占位符替换为你的实际问题，其余提示词保持不动。
> Replace the placeholder below with your actual question. Keep the rest of the prompt unchanged.

---

```
{{ 问题输入处 | QUESTION INPUT }}
（在此粘贴你的实际问题 / Paste your actual question here）
```

---

## 提示词模板（中文版)

先不要回答我的问题。在此之前，依次完成以下四件事：

1. **我未明说的假设**：告诉我我在做哪些没有说出口的假设。
2. **可大幅改变结论的信息**：告诉我如果拥有哪些信息，会显著改变你的判断。
3. **这类问题最常见的错误**：告诉我人们在问这类问题时最常犯的一个错误。
4. **一个最关键的问题**：问我一个问题，它能让你的回答真正适用于我的具体情况，而不是适用于任何可能的提问者。

「等我回答之后」再给出正式输出。正式输出必须严格包含以下四部分：

1. **完整有力的问题重述**：用最完整、最有力的方式，重述我真正想解决的问题。
2. **钢人论证**：使用钢人论证法（Steelman Argumentation）分别给出「支持我当前想法的最强论证」与「反对它的最强论证」。
3. **真正分歧与关键变量**：找出双方真正的分歧点，以及最可能改变结论的关键变量。
4. **判断与下一步**：给出明确判断、理由和下一步行动。

我的问题：

```
{{ 问题输入处 | QUESTION INPUT }}
```

---

## Prompt Template (English)

Don't answer my question yet. First do this:

1. **Unstated assumptions**: Tell me what assumptions I'm making that I haven't stated out loud.
2. **Information that would change your answer**: Tell me what information would significantly change your answer if you had it.
3. **Most common mistake**: Tell me the most common mistake people make when asking this type of question.
4. **One crucial question**: Ask me the one question that would make your answer actually useful for my specific situation rather than anyone who might ask this.

Only after I answer — give me the output. The output must include:

1. **Fullest restatement**: Restate the problem I'm really trying to solve, in the most complete and powerful way.
2. **Steelman arguments**: Give the strongest argument in favor of my current idea, and the strongest argument against it.
3. **Real disagreement & key variables**: Identify where the two sides genuinely disagree, and the key variables most likely to change the conclusion.
4. **Judgment & next steps**: Give a clear judgment, the reasoning behind it, and the next action to take.

My question:

```
{{ QUESTION INPUT }}
```

---

## 使用说明 / Usage

- 每次使用只需替换 `{{ 问题输入处 | QUESTION INPUT }}` 一处参数。
- 本模板为两阶段式：阶段一「前置四问」先澄清，阶段二「钢人分析」在你回答后再输出。
- 可手动装配进任意支持多轮对话的 AI 工具，或作为拼接到项目 Prompt 管线的固定模块。