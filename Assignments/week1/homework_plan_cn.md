# 第 1 周课后作业（中文拆解版）

> 目标：完成 6 种提示词工程技术练习，并让每个脚本中的测试通过。

## 你要交什么

根据 `Assignments/week1/README.md` 的要求，你需要：

1. 阅读每个源文件顶部任务说明。
2. 只修改标记为 `TODO` 的提示词区域（不要改模型设置）。
3. 迭代优化到测试通过。
4. 保存每种技术的最终提示词和输出。
5. 提交完整代码，并确认所有 TODO 都被处理。

## 第一周作业清单

- `Assignments/week1/k_shot_prompting.py`
- `Assignments/week1/chain_of_thought.py`
- `Assignments/week1/tool_calling.py`
- `Assignments/week1/self_consistency_prompting.py`
- `Assignments/week1/rag.py`
- `Assignments/week1/reflexion.py`

## 建议完成顺序（从易到难）

1. K-shot
2. Chain-of-thought
3. Tool calling
4. Self-consistency
5. RAG
6. Reflexion

## 实操流程（每个文件都按这个循环）

1. 打开文件，阅读顶部任务。
2. 填写 TODO 里的提示词。
3. 运行对应测试/脚本。
4. 记录失败案例。
5. 有针对性改提示词（加约束、加示例、明确输出格式）。
6. 重复直到通过。

## 统一调试建议

- 明确输出格式：比如“只输出 JSON，不要解释”。
- 提前约束边界：比如“无法确定时输出 UNKNOWN”。
- 优先给 2~5 个高质量示例，而不是很多低质量示例。
- 失败样本要反向喂给提示词（尤其是 reflexion/self-consistency）。

## 可直接复制的作业记录模板

```md
### 技术：<k-shot / cot / tool-calling / self-consistency / rag / reflexion>
- 初始提示词：
- 失败样例：
- 改进点：
- 最终提示词：
- 最终输出示例：
- 测试结果：
```

## 本地检查命令（示例）

在仓库根目录执行：

```bash
cd Assignments
poetry install
```

然后按需运行对应脚本或测试（以课程文件内说明为准）。

## 你可以这样和我协作

把你当前做的某一个文件（例如 `k_shot_prompting.py`）贴出来，我会按下面步骤和你一起完成：

1. 先给你一个可跑通的第 1 版提示词。
2. 根据报错/失败样本做第 2 版修正。
3. 直到你本地测试通过，再整理成可提交版本。

