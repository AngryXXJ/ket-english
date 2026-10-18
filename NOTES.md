# NOTES.md — 教学备忘

## 关于Hanyang
- 小学生，备考 KET（A2 Key）
- **不会找重点句**：阅读时不知道哪句是答题关键，需要专门训练「划重点」
- 单词学习要体现意思和应用，不能只背拼写
- 对太简单的文本会无聊；题目要有「跳一跳够得着」的难度

## 爸爸（用户）的偏好
- 务实直接，讨厌花架子（之前否掉了 emoji 美术和过浅的文本）
- 素材用真题原文，不要自编简化文本
- 固定流程：单词 → 阅读 → 语法 → 测试
- 阅读环节设计原则（已敲定）：剧情/目标前置学词 → 问题先行 + 正文无标记 → 孩子自己划关键句（分级提示，绝不直接亮答案）→ 就着划出的句子讲语法 → 真题原题做测试

## 技术备忘
- `KET全真模拟试题.pdf`：205 页扫描版无文字层。提取方法：`pdftoppm -jpeg -r 60 -f N -l M KET全真模拟试题.pdf /tmp/ket_p` 渲染成图再读；读图前用 `sips -Z 1900 -s format jpeg -s formatOptions 60` 压缩
- 已知页码：p3=Part1 短信息 4-6、p4-5=Part2 My House、p6=Part3 企鹅文+Q14-18、p7=Part4 温网 cloze、p8=Part5 邮件 cloze。每套 Test 约 16 页，全书约 8 套
- 预览 HTML：临时 `python3 -m http.server 7100`，用完杀掉

## 发布流程（持续生产 → Hanyang 持续访问）
- GitHub 仓库 `AngryXXJ/ket-english`（public，Pages 从 main 根目录发布）
- 线上地址：https://angryxxj.github.io/ket-english/
- 每做完一课：① 新 HTML 放 `lessons/` ② 在 `index.html` 加卡片 ③ `git add -A && git commit -m "第 N 课" && git push`
- Pages 部署约 1 分钟生效；PDF、脚本、旧 demo 已在 .gitignore 排除，不会上传
