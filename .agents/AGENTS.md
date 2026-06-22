<RULE>
# Learning Sequence Preference: Top-Down & Positive Feedback First
When proposing, evaluating, or structuring learning plans for this user, ALWAYS sequence the tasks to provide end-to-end positive feedback early.
- Introduce complex foundational engineering (e.g., Data ETL pipelines) *after* the core modeling/training loops have been successfully run with existing datasets.
- Do not force a strict chronological industrial pipeline if it delays the first "aha" moment of a working model.
- Maintain analytical depth in Pretraining (do not deprioritize it), but allow practical implementations to be compressed if hardware or time constraints require it.
</RULE>

<RULE>
# Evaluation Completeness: Fix ALL identified issues
When an evaluation report identifies Limitations, Challenges, or Check failures:
- Every issue marked CRITICAL or MAJOR must have a corresponding code change OR an explicit "won't fix" justification approved by the user.
- Do not mark a task as complete (GOAL_COMPLETE) if any CRITICAL/MAJOR issue from the evaluation remains unaddressed.
- "Structural" issues (like missing metadata/annotations) count as real issues, not just "nice to have".
</RULE>


<RULE>
# LeetCode Workflow Preference
When proposing or structuring LeetCode / Algorithm practice:
1. **Platform**: Default to using the LeetCode website for coding and execution. Do NOT over-engineer local testing environments (like local `ListNode`/`TreeNode` setups) unless explicitly requested.
2. **Local Prep**: "Local preparation" should focus on tracking progress (e.g., Markdown checklists), archiving solutions, and providing cheat sheets, not executing code.
3. **Language Progression**: If the user is anxious about language friction, recommend the "Python first (for algorithm intuition), C++ later (for systems deployment)" strategy.
</RULE>


<RULE>
# Rusty Fundamentals Protocol: JIT Review
When the user expresses that they have forgotten fundamental prerequisites (e.g., DSA, Python, Math):
1. **Never front-load massive theory**: Do not propose a linear "review everything first, practice later" syllabus. This delays positive feedback.
2. **Apply Just-in-Time (JIT) Review**: Break the theory into micro-sessions (20-30 mins) and interleave them directly before the relevant practical task.
3. **Preferred Formats**: Default to high-density, interactive, visual resources (like `hello-algo.com` for DSA) over long-form video lectures.
</RULE>

<RULE>
# Learning Module Flow Classification
When designing or restructuring learning plans with multiple modules/projects:
1. **Classify each module** as either "算法类 (algorithm-driven)" or "工程类 (engineering-driven)".
2. **Algorithm-driven** (theory-first): Topics where the mathematical formulation IS the core insight (e.g., DPO, GRPO, MoE routing, RL algorithms). Flow: 📄 论文精读 → ✏️ 公式手推 → 💻 代码实现 → ❓ DDQ
3. **Engineering-driven** (code-first): Topics where the system design IS the core insight (e.g., vLLM, data pipelines, distributed training, evaluation harness). Flow: 💻 代码跑通 → 🔍 源码精读 → 📄 论文查漏 → ❓ DDQ
4. **Label each module** with its type and flow in the roadmap document.
5. **When DDQs span multiple modules** (progressive learning), mark the depth level (🔵 Awareness → 🟡 Working → 🔴 Expert) and cross-reference rather than duplicating questions.
</RULE>
