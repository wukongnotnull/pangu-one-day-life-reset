# 来源清单与采集记录

## 蒸馏模式

- **对象**：《How to fix your entire life in 1 day》
- **类型**：D2 内容类（长文）
- **模式**：纯本地语料；不联网补作者人格或理论证据
- **作者信息**：原文仅署名 `Dan`，无法确认完整身份
- **调研日期**：2026-09-09

## 来源

| 来源 | 类型 | 可信度 | 用途 |
|---|---|---:|---|
| 用户在当前会话提供的英文全文及中文对译 | 一手文本 | 高（针对“原文说了什么”） | 核心命题、协议、表达与张力 |
| `01-source-article.md` | 一手摘录 | 高（逐句摘自用户材料） | 可追溯的提取底稿 |
| `10-baseline-tests.md` | 独立测试记录 | 高（针对基线行为） | 判断新 Skill 的必要增量 |

## 脚本执行

使用：

```text
python3 {pangu_skill_root}/scripts/run.py collect-local [路径] -o [distillation目录] --no-transcribe
```

1. 首次输入当前会话的 `.jsonl` 转录文件。脚本退出码为 0，但内部结果为 `成功 0 / 失败 1`，原因是 `不支持的格式: unknown`。这次不计为有效采集。
2. 将文章关键原句整理为受支持的 Markdown 摘录后重跑；补充控制论跨域原句后再次刷新。最终结果为 `总文件数 1 / 成功 1 / 失败 0 / 总字数 7,381`。
3. `output-root` 成功探测为 `/Users/wukong/Downloads/distill-demo/.agents/skills`。
4. `skill-root` 环境探测返回退出码 2，因为宿主未注入路径变量；实际根目录依据 Cursor discovery 提供的已加载路径解析为 `/Users/wukong/Downloads/distill-demo/.cursor/skills/pangu-distill`。

## 一手占比与质量

- 可用来源数：1 份用户提供的原文。
- 一手文本占比：100%。
- 对“作者理论是否科学成立”的外部验证：0%。
- 因来源少于 10，最终只保留 3 个通过三重验证的核心模型；“挖掘—中断—压缩”因缺少跨域复现降级为操作协议，并扩大诚实边界。

## 缺口

- 无原始发布 URL、发布日期、平台和作者全名。
- 未核验 Adler、Maltz、Naval、Csikszentmihalyi 引语及心智阶段理论。
- 无样本、效果数据、失败率、长期追踪或临床安全说明。
- 摘录未保留完整双语全文；只保留进入框架的关键英文原句。
