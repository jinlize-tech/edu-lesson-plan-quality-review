# 教案质量审查示例

## 典型场景

教师提交的教案有小组讨论，但没有说明分组、产出和评价标准。

## 具体示例

系统指出讨论活动的任务、角色、时长和评价证据缺失，并给出可直接补入教案的改写片段。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "lesson_plan": "待审教案已核对（脱敏示例）",
  "curriculum_standards": "课程标准或目标依据已核对（脱敏示例）",
  "grade_and_subject": "年级与学科已核对（脱敏示例）",
  "student_profile": "学情摘要已核对（脱敏示例）",
  "lesson_duration": "课时长度已核对（脱敏示例）",
  "resources": [
    {}
  ],
  "review_focus": [
    {}
  ]
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出教案审查表、目标-活动-评价矩阵、修订建议等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
