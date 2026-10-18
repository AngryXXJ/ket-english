# 方向调整：放弃游戏化，转向 teach 学习素材

用户试玩了两版游戏 Demo 后判断「游戏本身不精巧」，决定改走学习素材路线：把《KET全真模拟试题》的阅读真题提取出来，按「单词 → 阅读 → 语法 → 测试」固定流程做成 HTML 课件给Hanyang用。美术、游戏引擎（CodeCombat）均放弃。

## Implications
- 课件产出位置：`lessons/`，单文件 HTML，排版干净可打印，即时反馈，不用游戏化包装
- 原文转写存档在 `reference/test<N>-reading-原文.md`，做新课时直接取用，不必重读 PDF
- PDF 结构：每套 Test 约 16 页；Paper 1 阅读在开头（Part 2 三人短文、Part 3 长文、Part 4/5 cloze 都适合做课）；Test 1 已全部转写
- 阅读环节核心训练「自己划重点句」：正文无标记、问题先行、分级提示、不直接亮答案（NOTES.md 有完整设计原则）
