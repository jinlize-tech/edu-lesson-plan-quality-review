# 使用说明

## 适用任务

教师提交的教案有小组讨论，但没有说明分组、产出和评价标准。

## 准备输入

教案、课程标准或教学目标、年级学情、课时、资源条件、班型、评价要求、希望重点审查的维度。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 确认标准
2. 解析目标与活动
3. 检查对齐和认知负荷
4. 计算时间与材料需求
5. 检查评价证据
6. 输出问题与修订示例

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

业务负责人复核输入事实、关键假设和最终成果适用范围后，成果才可进入正式业务使用。
