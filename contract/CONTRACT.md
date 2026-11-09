# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `lesson_plan` | 待审教案 | string | 是 |
| `curriculum_standards` | 课程标准或目标依据 | string | 是 |
| `grade_and_subject` | 年级与学科 | string | 是 |
| `student_profile` | 学情摘要 | string | 否 |
| `lesson_duration` | 课时长度 | string | 是 |
| `resources` | 可用资源 | array | 是 |
| `review_focus` | 审查重点 | array | 否 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `教案审查表`：结构化条目数组，不允许空壳或占位文本。
- `目标-活动-评价矩阵`：结构化条目数组，不允许空壳或占位文本。
- `时间风险`：结构化条目数组，不允许空壳或占位文本。
- `缺失证据`：结构化条目数组，不允许空壳或占位文本。
- `修订建议`：结构化条目数组，不允许空壳或占位文本。
- `复核问题`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
