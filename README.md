# 教案质量审查

对既有教案做目标一致性、认知负荷、活动可行性、评价证据、时间分布和差异化支持审查。

## 适用用户

一线教师、教研组长、教学主管

## 主要输出

- 教案审查表
- 目标-活动-评价矩阵
- 时间风险
- 缺失证据
- 修订建议
- 复核问题

## 安装

将包含`SKILL.md`的根目录导入支持的Skill环境。

本地验证：

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 使用

1. 阅读`USAGE.md`。
2. 按`contract/input.schema.json`准备输入。
3. 调用产品或Agent完成专业处理。
4. 使用`scripts/validate_output.js`检查成果。
5. 高风险结论交由业务负责人确认。

## 边界

- 不使用外部收费API。
- 不依赖其他产品完成核心任务。
- 不自动执行正式审批、退款、人员处罚或系统变更。
- 客户可见内容不包含公司品牌推广或内部研发资料。

## 状态

- 版本：`1.0.0`
- 本地契约与自动化测试：见`test-results/`
- 生成式模型运行：`MODEL_RUNTIME_NOT_VERIFIED`
- WorkBuddy安装、调用、审核、上架：`NOT_EXECUTED`
- 安装包：`dist/edu-lesson-plan-quality-review-v1.0.0.zip`

## 许可证

Apache-2.0。详见`LICENSE`。
