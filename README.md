# viral-copy-factory

租房爆款文案工厂 — 完整的租房内容创作流水线。

## 功能

- 房源画像分析（目标人群、内容风格、核心卖点）
- 从飞书爆款报告获取结构密码（标题模板、钩子、标签策略）
- AI 生成即美化的小红书/抖音内容
- 去重评分（7维度/6维度，含10分去重维度）
- 评分不达标自动重试优化（最多3次）

## 使用

```bash
python -X utf8 scripts/run_pipeline.py generate --platform xhs --property-index 0
python -X utf8 scripts/run_pipeline.py batch --platform xhs --count 5
python -X utf8 scripts/run_pipeline.py history
```

## 配套 Skill

- `viral-element-analyzer`: 采集趋势数据 → 提取爆款结构 → 更新飞书报告
- `viral-copy-factory`（本仓库）: 读取飞书报告 → 生成文案 → 评分优化
