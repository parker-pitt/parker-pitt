# 审核报告模板 · Review report template

<sub>可直接复制使用 · Free to copy. Review only what can be checked: logs, diffs, runtime state, test output. Never the builder's own account.</sub>

## 结论 · Verdict
`PASS` / `PASS_WITH_DISCLOSED_DEVIATION` / `HOLD — evidence required` / `FAIL`

一句话理由 · One-line reason:

## 我核对了什么 · What I checked
| 项目 Item | 方法 How | 结果 Result |
|---|---|---|
| 源码包可独立复现 Bundle reproducible | 独立克隆 + fsck · fresh clone + fsck | |
| diff 范围 Diff scope | 与任务卡范围对比 · against card scope | |
| 原失败测试 Original failing test | 修复前后各跑一次 · run before and after | |
| 全量测试 Full suite | 原文输出 · raw output | |

## 阻断项 · Blockers
每条写：现象、证据位置、要求补什么。
Each: symptom, where the evidence is, what is needed.

## 非阻断意见 · Non-blocking notes

## 给负责人的建议 · Recommendation to the owner
审核结论是建议，不是放行。
This verdict is a recommendation, not a release.
