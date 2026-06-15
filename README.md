# Tico跨境外贸Team Skill插件

🚀 **专属于Tico的跨境外贸Team协作Skill插件系统**

这是一个集成了**销售、产品经理、运营、会计、法务**五大岗位的GitHub Skill插件，专门为跨境外贸业务设计。

## 📋 功能概述

### 核心岗位Skills

| 岗位 | 模块 | 主要职责 | 自动化支持 |
|------|------|--------|----------|
| **销售** | Sales Skill | 客户开发、订单管理、客户反馈 | 自动标签、客户信息录入模板 |
| **产品经理** | PM Skill | 产品规划、需求评审、版本管理 | 自动优先级设置、需求看板 |
| **运营** | Operations Skill | 物流、库存、合规、支付 | 自动警报、任务分配、流程跟踪 |
| **会计** | Finance Skill | 财务管理、成本控制、税务合规 | 自动报告生成、财务流程审批 |
| **法务** | Legal Skill | 合同管理、风险评估、法��遵从 | 合规检查清单、文档审核流 |

## 🏗️ 项目结构

```
Work-skill/
├── README.md                          # 项目总览
├── .github/
│   ├── workflows/                     # GitHub Actions自动化
│   │   ├── sales-workflow.yml         # 销售岗位工作流
│   │   ├── pm-workflow.yml            # 产品经理工作流
│   │   ├── ops-workflow.yml           # 运营岗位工作流
│   │   ├── finance-workflow.yml       # 会计岗位工作流
│   │   ├── legal-workflow.yml         # 法务岗位工作流
│   │   └── team-sync.yml              # 团队协作同步
│   └── ISSUE_TEMPLATE/                # Issue模板
│       ├── sales-customer-request.md  # 销售客户需求
│       ├── pm-feature-request.md      # PM功能需求
│       ├── ops-incident.md            # 运营事项
│       ├── finance-report.md          # 财务报告
│       └── legal-compliance.md        # 法务合规
│
├── skills/
│   ├── sales/                         # 销售岗位Skill
│   │   ├── README.md
│   │   ├── customer-management.md     # 客户管理流程
│   │   ├── order-tracking.md          # 订单跟踪
│   │   ├── templates/
│   │   │   ├── customer-profile.md    # 客户档案模板
│   │   │   └── order-form.md          # 订单表格
│   │   └── checklists/
│   │       └── customer-onboarding.md # 客户上线检查表
│   │
│   ├── pm/                            # 产品经理岗位Skill
│   │   ├── README.md
│   │   ├── roadmap-management.md      # 产品规划
│   │   ├── requirement-review.md      # 需求评审
│   │   ├── templates/
│   │   │   ├── feature-spec.md        # 功能规格书
│   │   │   └── user-story.md          # 用户故事
│   │   └── checklists/
│   │       └── release-checklist.md   # 发布检查表
│   │
│   ├── operations/                    # 运营岗位Skill
│   │   ├── README.md
│   │   ├── logistics.md               # 物流管理
│   │   ├── customs-compliance.md      # 海关合规
│   │   ├── templates/
│   │   │   ├── shipping-doc.md        # 物流单据
│   │   │   └── incident-report.md     # 事项报告
│   │   └── checklists/
│   │       ├── order-fulfillment.md   # 订单履行检查
│   │       └── customs-clearance.md   # 清关检查表
│   │
│   ├── finance/                       # 会计岗位Skill
│   │   ├── README.md
│   │   ├── accounting-standards.md    # 会计准则
│   │   ├── tax-compliance.md          # 税务合规
│   │   ├── templates/
│   │   │   ├── invoice.md             # 发票模板
│   │   │   └── expense-report.md      # 费用报告
│   │   └── checklists/
│   │       ├── monthly-close.md       # 月结检查表
│   │       └── tax-filing.md          # 税务申报检查
│   │
│   └── legal/                         # 法务岗位Skill
│       ├── README.md
│       ├── contract-management.md     # 合同管理
│       ├── compliance-framework.md    # 合规框架
│       ├── templates/
│       │   ├── contract-template.md   # 合同模板
│       │   └── risk-assessment.md     # 风险评估
│       └── checklists/
│           ├── contract-review.md     # 合同审查清单
│           └── compliance-audit.md    # 合规审计清单
│
├── dashboards/                        # 仪表板和集成
│   ├── team-dashboard.md              # 团队协作仪表板
│   ├── kpi-tracking.md                # KPI跟踪
│   └── integration-guide.md           # 集成指南
│
├── docs/
│   ├── getting-started.md             # 快速开始
│   ├── workflow-guide.md              # 工作流指南
│   ├── cross-border-regulations.md    # 跨境法规汇总
│   └── best-practices.md              # 最佳实践
│
└── config/
    ├── team-roles.json                # 团队角色配置
    ├── automation-rules.json           # 自动化规则
    └── integration-settings.json       # 集成设置
```

## 🚀 快速开始

### 1. 克隆或Fork此仓库
```bash
git clone https://github.com/tico271160398-creator/Work-skill.git
cd Work-skill
```

### 2. 配置团队角色
编辑 `config/team-roles.json` 添加您的团队成员信息。

### 3. 启用GitHub Actions
所有工作流已在 `.github/workflows/` 中配置，自动启用。

### 4. 创建Issue
使用对应的Issue模板为不同岗位创建工作任务。

## 📊 核心工作流

### 销售岗位工作流 (Sales Skill)
```
客户反馈 → 自动标签(sales) → 分配销售主管 → 更新客户档案 → 订单生成 → 运营交接
```

### 产品经理工作流 (PM Skill)
```
需求提交 → PM评审 → 优先级排序 → 技术规格 → 发布计划 → 版本跟踪
```

### 运营工作流 (Operations Skill)
```
订单确认 → 库存检查 → 物流安排 → 清关申报 → 发货 → 客户跟踪
```

### 会计工作流 (Finance Skill)
```
费用记录 → 自动分类 → 合规检查 → 月度报告 → 税务申报 → 审计追溯
```

### 法务工作流 (Legal Skill)
```
合同收集 → 自动审查 → 风险评估 → 批准 → 归档 → 定期审计
```

## 🔗 集成功能

### 已支持的集成
- ✅ **Slack** - 实时通知和任务更新
- ✅ **GitHub Projects** - 看板式任务管理
- ✅ **GitHub Discussions** - 团队讨论和知识库
- ✅ **GitHub Webhooks** - 事件驱动自动化
- ✅ **Issue标签系统** - 自动分类和路由

### 计划中的集成
- 📋 钉钉/企业微信
- 📊 数据分析仪表板
- 💰 财务系统API
- 📦 ERP系统对接

## 📚 文档导航

| 文档 | 描述 | 链接 |
|------|------|------|
| 快速开始 | 如何快速上手本Skill系统 | [docs/getting-started.md](docs/getting-started.md) |
| 工作流指南 | 详细的工作流说明 | [docs/workflow-guide.md](docs/workflow-guide.md) |
| 法规汇总 | 跨境外贸相关法规 | [docs/cross-border-regulations.md](docs/cross-border-regulations.md) |
| 最佳实践 | 团队协作最佳实践 | [docs/best-practices.md](docs/best-practices.md) |
| 销售Skill | 销售岗位完整指南 | [skills/sales/README.md](skills/sales/README.md) |
| PM Skill | 产品经理完整指南 | [skills/pm/README.md](skills/pm/README.md) |
| 运营Skill | 运营岗位完整指南 | [skills/operations/README.md](skills/operations/README.md) |
| 财务Skill | 会计岗位完整指南 | [skills/finance/README.md](skills/finance/README.md) |
| 法务Skill | 法律岗位完整指南 | [skills/legal/README.md](skills/legal/README.md) |

## 🎯 主要特性

✨ **自动化工作流**
- 基于标签的自动分配
- 智能Issue分类
- 自动提醒和通知

📋 **标准化模板**
- Issue模板
- 文档模板
- 检查清单

🔄 **跨部门协作**
- 统一的任务管理
- 清晰的权限管理
- 实时的进度跟踪

📊 **数据驱动**
- KPI仪表板
- 性能报告
- 趋势分析

🌍 **国际化支持**
- 多语言文档
- 国家/地区特定的合规指南
- 跨时区协作工具

## 👥 团队角色权限

### 销售
- 创建客户相关Issue
- 查看订单状态
- 添加客户反馈

### 产品经理
- 创建功能需求
- 优先级排序
- 需求评审

### 运营
- 创建订单Issue
- 物流跟踪
- 事项报告

### 会计
- 创建财务报告
- 费用审批
- 税务申报

### 法务
- 合同管理
- 合规审查
- 风险评估

## 🔐 安全与合规

- ✅ 数据加密存储
- ✅ 访问权限控制
- ✅ 审计日志记录
- ✅ GDPR兼容
- ✅ 跨境数据转移合规

## 📞 支持与反馈

有问题或建议？
- 📧 Email: support@tico.com
- 💬 GitHub Discussions: [讨论区](../../discussions)
- 🐛 Bug报告: [提交Issue](../../issues/new)

## 📝 更新日志

### v1.0.0 (2026-06-15)
- ✅ 初始版本发布
- ✅ 五大岗位Skills实现
- ✅ 自动化工作流配置
- ✅ 完整文档编写

## 📄 License

MIT License - 详见 [LICENSE](LICENSE) 文件

---

**Made with ❤️ by Tico** | 专属跨境外贸Team协作工具
