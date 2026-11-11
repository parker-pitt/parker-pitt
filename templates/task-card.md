# 任务卡模板 · Task card template

<sub>可直接复制使用 · Free to copy. Fill every field; an empty field means the card is not ready.</sub>

## 1. 目标 · Goal
一句话：这张卡做完后，什么事情变成真的。
One sentence: what becomes true when this card is done.

## 2. 执行者 · Executor
你就是执行者。不要把这张卡转发给别人。
You are the executor. Do not forward this card.

## 3. 范围 · Scope
- 允许改动 · May change:
- 不许碰 · Must not touch:
- 不在本卡内 · Out of scope (needs a new card):

## 4. 基准 · Baseline
- 代码基准 SHA · Base SHA:
- 环境 · Environment:

## 5. 门禁 · Gates
| 门禁 Gate | 通过条件 Pass condition | 证据 Evidence |
|---|---|---|
| G1 构建 Build | | |
| G2 原失败测试先红后绿 Failing test red → green | | |
| G3 全量测试 Full suite | | |
| G4 收尾（停服务、清理）Wrap-up | 需要单独授权 Separate approval | |

## 6. 失败即停 · Stop on first failure
任何一步第一次失败：停下，报告命令、输出和你的判断。不要换参数重试，不要自己解释成"其实算通过"。
First failure at any step: stop and report the command, output and your reading. Do not retry with new parameters or reinterpret it as a pass.

## 7. 交付证据包 · Evidence pack
- 源码包 + 校验和 · Source bundle + checksums
- diff（只含本卡范围）· Diff, this card's scope only
- 测试输出原文 · Raw test output
- 偏差说明（没有就写"无"）· Deviations ("none" if none)

## 8. 放行 · Release
审核给出建议；Go / No-Go 由负责人决定。
Review recommends; the owner decides go / no-go.
