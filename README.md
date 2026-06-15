# Tico 新能源产品跨境外贸 Facebook投流 Team Skill插件

🚀 **专属于Tico的新能源跨境电商Facebook投流Team协作Skill插件系统**

本系统集成了**销售、产品经理、运营、会计、法务**五大岗位，专门为新能源产品（太阳能板、太阳能路灯、逆变器、便携式户外灯）在东亚及其他新兴市场的Facebook投流业务而设计。

## 🎯 核心定位

- **行业**: 新能源产品
- **主要产品**: 太阳能板、太阳能路灯、逆变器、便携式户外灯
- **主要市场**: 东亚（越南、菲律宾、马来西亚、新加坡）+ 西非 + 中东
- **营销渠道**: Facebook投流
- **目标客群**: B2B采购商、分销商、零售商、工程项目方

## 📊 功能概览

### 核心岗位Skills

| 岗位 | 模块 | 主要职责 | 自动化支持 | 地区适配 |
|------|------|--------|---------|--------|
| **销售** | Sales Skill | 客户开发、商机转化、FB投流分析 | 自动标签、CRM更新、投流ROI跟踪 | 越南、菲律宾、马来西亚、新加坡、西非、中东 |
| **产品经理** | PM Skill | 产品定价、市场分析、供应链管理 | 需求评审、产品合规检查 | 各市场产品适配 |
| **运营** | Operations Skill | 订单履行、物流、海关清关、库存 | 自动警报、任务分配、流程跟踪 | 多地区物流路由 |
| **会计** | Finance Skill | 财务管理、汇率管理、税务合规 | 自动报告生成、财务审批流 | 多国税务、汇兑损益 |
| **法务** | Legal Skill | 合同管理、出口合规、风险评估 | 合规检查、文档审核 | 多国贸易法规 |

## 🌍 支持的目标市场

### 🔴 优先市场（东亚）

#### 越南 (Vietnam)
- **人口**: 9700万
- **优势**: 低成本、基础设施发展快、太阳能渗透率提升
- **税率**: 10% VAT, 关税 0-20%
- **支付方式**: 银行转账、支付宝、WeChat Pay
- **语言**: 越南语、英语
- **FB用户**: 1.15亿+（广告成本低）

#### 菲律宾 (Philippines)
- **人口**: 1.2亿
- **优势**: 高FB渗透率、岛屿众多需要独立电源、英语普及
- **税率**: 12% VAT, 关税 0-30%
- **支付方式**: GCash、PayMaya、银行转账
- **语言**: 英语、菲律宾语
- **FB用户**: 1.09亿+（Facebook文化强）

#### 马来西亚 (Malaysia)
- **人口**: 3400万
- **优势**: 经济相对发达、可再生能源政策鼓励、英语使用广泛
- **税率**: 6% SST, 关税 0-20%
- **支付方式**: 银行转账、FPX、在线支付
- **语言**: 英语、马来语
- **FB用户**: 2300万+（商业化程度高）

#### 新加坡 (Singapore)
- **人口**: 570万
- **优势**: 高收入、政府重视绿能、物流枢纽
- **税率**: 8% GST, 关税 0（大多数产品）
- **支付方式**: 银行转账、信用卡、PayLah!
- **语言**: 英语、华语、马来语、泰米尔语
- **FB用户**: 450万+（高购买力）

### 🟠 次级市场（西非）

- **尼日利亚 (Nigeria)**: 人口1.7亿，太阳能需求巨大，FB投流成本低
- **加纳 (Ghana)**: 人口3300万，政治稳定，太阳能市场增长快
- **肯尼亚 (Kenya)**: 人口5300万，东非枢纽，绿能意识强
- **南非 (South Africa)**: 人口6000万，经济发达，技术认可度高

### 🟡 中东市场

- **阿联酋 (UAE)**: 迪拜太阳能需求，高购买力
- **沙特 (Saudi Arabia)**: Vision 2030绿能计划，巨大市场
- **阿曼 (Oman)**: 能源转型需求
- **卡塔尔 (Qatar)**: 高端市场、可靠性要求

## 🛠 项目结构

```
Work-skill/
├── README.md                               # 项目总览
├── .github/
│   ├── workflows/
│   │   ├── sales-workflow.yml             # 销售岗位工作流
│   │   ├── pm-workflow.yml                # PM岗位工作流
│   │   ├── ops-workflow.yml               # 运营岗位工作流
│   │   ├── finance-workflow.yml           # 会计岗位工作流
│   │   ├── legal-workflow.yml             # 法务岗位工作流
│   │   └── fb-campaign-sync.yml           # Facebook投流同步
│   └── ISSUE_TEMPLATE/
│       ├── sales-fb-campaign.md           # 销售FB投流活动
│       ├── sales-customer-lead.md         # 销售客户线索
│       ├── pm-market-analysis.md          # PM市场分析
│       ├── pm-product-compliance.md       # PM产品合规
│       ├── ops-order.md                   # 运营订单
│       ├── ops-shipping.md                # 运营物流
│       ├── finance-report.md              # 会计报告
│       ├── finance-exchange.md            # 汇率管理
│       ├── legal-contract.md              # 法务合同
│       └── legal-export-compliance.md     # 出口合规
│
├── skills/
│   ├── sales/                              # 销售Skill
│   │   ├── README.md
│   │   ├── fb-advertising-strategy.md     # FB广告策略
│   │   ├── fb-audience-targeting.md       # 受众定位
│   │   ├── market-analysis/
│   │   │   ├── vietnam.md                 # 越南市场
│   │   │   ├── philippines.md             # 菲律宾市场
│   │   │   ├── malaysia.md                # 马来西亚市场
│   │   │   ├── singapore.md               # 新加坡市场
│   │   │   ├── west-africa.md             # 西非市场
│   │   │   └── middle-east.md             # 中东市场
│   │   ├── customer-management.md         # 客户管理
│   │   ├── sales-pipeline.md              # 销售漏斗
│   │   ├── templates/
│   │   │   ├── fb-ad-copy.md              # FB文案模板
│   │   │   ├── customer-profile.md        # 客户档案
│   │   │   └── quotation.md               # 报价单
│   │   └── checklists/
│   │       ├── fb-campaign-launch.md      # 活动上线检查
│   │       └── lead-qualification.md      # 线索资格确认
│   │
│   ├── pm/                                 # PM Skill
│   │   ├── README.md
│   │   ├── product-strategy.md            # 产品策略
│   │   ├── market-segmentation.md         # 市场分析
│   │   ├── pricing-strategy/
│   │   │   ├── vietnam-pricing.md
│   │   │   ├── philippines-pricing.md
│   │   │   ├── malaysia-pricing.md
│   │   │   ├── singapore-pricing.md
│   │   │   ├── west-africa-pricing.md
│   │   │   └── middle-east-pricing.md
│   │   ├── product-compliance/
│   │   │   ├── solar-panel-standards.md   # 太阳能板标准
│   │   │   ├── solar-street-light.md      # 太阳能路灯标准
│   │   │   ├── inverter-specs.md          # 逆变器规格
│   │   │   └── portable-light-specs.md    # 便携式户外灯规格
│   │   ├── templates/
│   │   │   ├── product-spec.md            # 产品规格
│   │   │   └── compliance-checklist.md    # 合规检查清单
│   │   └── market-research/
│   │       ├── competitor-analysis.md     # 竞品分析
│   │       └── demand-forecast.md         # 需求预测
│   │
│   ├── operations/                         # 运营Skill
│   │   ├── README.md
│   │   ├── order-fulfillment.md           # 订单履行
│   │   ├── logistics-routing/
│   │   │   ├── vietnam-routes.md
│   │   │   ├── philippines-routes.md
│   │   │   ├── malaysia-routes.md
│   │   │   ├── singapore-routes.md
│   │   │   ├── west-africa-routes.md
│   │   │   └── middle-east-routes.md
│   │   ├── customs-clearance.md           # 清关流程
│   │   ├── inventory-management.md        # 库存管理
│   │   ├── templates/
│   │   │   ├── shipping-doc.md            # 物流单据
│   │   │   ├── customs-form.md            # 清关表单
│   │   │   └── incident-report.md         # 事项报告
│   │   └── checklists/
│   │       ├── order-fulfillment.md       # 订单检查
│   │       └── customs-compliance.md      # 清关检查
│   │
│   ├── finance/                            # 会计Skill
│   │   ├── README.md
│   │   ├── accounting-standards.md        # 会计准则
│   │   ├── exchange-rate-management.md    # 汇率管理
│   │   ├── tax-compliance/
│   │   │   ├── vietnam-tax.md
│   │   │   ├── philippines-tax.md
│   │   │   ├── malaysia-tax.md
│   │   │   ├── singapore-tax.md
│   │   │   ├── west-africa-tax.md
│   │   │   └── middle-east-tax.md
│   │   ├── templates/
│   │   │   ├── invoice.md                 # 发票
│   │   │   ├── expense-report.md          # 费用报告
│   │   │   └── currency-conversion.md     # 汇兑记录
│   │   └── checklists/
│   │       ├── monthly-close.md           # 月度结账
│   │       └── tax-filing.md              # 税务申报
│   │
│   └── legal/                              # 法务Skill
│       ├── README.md
│       ├── contract-management.md         # 合同管理
│       ├── export-regulations/
│       │   ├── vietnam-export.md
│       │   ├── philippines-export.md
│       │   ├── malaysia-export.md
│       │   ├── singapore-export.md
│       │   ├── west-africa-export.md
│       │   └── middle-east-export.md
│       ├── product-certification/
│       │   ├── solar-panel-cert.md        # 太阳能板认证
│       │   ├── solar-street-light-cert.md # 路灯认证
│       │   ├── inverter-cert.md           # 逆变器认证
│       │   └── portable-light-cert.md     # 便携灯认证
│       ├── templates/
│       │   ├── export-contract.md         # 出口合同
│       │   ├── compliance-report.md       # 合规报告
│       │   └── risk-assessment.md         # 风险评估
│       └── checklists/
│           ├── contract-review.md         # 合同审查
│           └── export-checklist.md        # 出口检查
│
├── dashboards/
│   ├── fb-campaign-dashboard.md            # FB投流仪表板
│   ├── sales-pipeline-dashboard.md         # 销售漏斗仪表板
│   ├── regional-analysis.md                # 地区分析
│   ├── product-performance.md              # 产品表现
│   └── kpi-tracking.md                     # KPI跟踪
│
├── docs/
│   ├── getting-started.md                  # 快速开始
│   ├── workflow-guide.md                   # 工作流指南
│   ├── fb-marketing-guide.md               # FB投流指南
│   ├── regional-market-guide.md            # 区域市场指南
│   ├── product-guide.md                    # 产品指南
│   ├── customs-regulations.md              # 海关法规汇总
│   ├── tax-guide.md                        # 税务指南
│   └── best-practices.md                   # 最佳实践
│
├── config/
│   ├── team-roles.json                     # 团队角色配置
│   ├── market-config.json                  # 市场配置
│   ├── product-config.json                 # 产品配置
│   ├── automation-rules.json                # 自动化规则
│   └── integration-settings.json            # 集成设置
│
└── templates/
    ├── fb-ad-templates.md                  # FB广告模板
    ├── email-templates.md                  # 邮件模板
    └── document-templates/                 # 文档模板
        ├── invoice-template.xlsx
        ├── contract-template.docx
        └── quotation-template.xlsx
```

## 🎯 核心业务流程

### 1️⃣ Facebook投流→线索获取→销售跟进

```
数据分析
  ↓
FB广告创建（分地区、产品）
  ↓
投流优化（A/B测试、受众细分）
  ↓
线索收集（表单、私信、评论）
  ↓
销售跟进（CRM更新、资格认证）
  ↓
报价单生成
  ↓
订单确认
  ↓
完成
```

### 2️⃣ 订单处理→物流→清关→交付

```
订单输入
  ↓
库存检查
  ↓
发货准备（打包、装运单）
  ↓
选择物流（按目的地）
  ↓
清关单据准备
  ↓
海关清关（目的地）
  ↓
物流跟踪
  ↓
客户签收
  ↓
完成
```

### 3️⃣ 财务管理→汇兑→税务申报

```
收入记录
  ↓
成本分配
  ↓
汇率转换（多币种）
  ↓
利润计算
  ↓
月度报表
  ↓
税务申报（各国）
  ↓
审计跟踪
  ↓
完成
```

### 4️⃣ 合规检查→合同审批→风险管理

```
客户身份验证
  ↓
产品合规检查
  ↓
出口法规审查
  ↓
合同起草和审查
  ↓
风险评估
  ↓
内部审批
  ↓
客户签署
  ↓
归档
  ↓
定期审计
```

## 📱 新能源产品详情

### 1. 太阳能板 (Solar Panels)
- **规格**: 50W-400W
- **效率**: 18-22%
- **认证**: IEC 61215, CE, CQC
- **目标市场**: 工商业、家用、社区电网
- **关键卖点**: 高效率、长寿命(25年)、防水防盐

### 2. 太阳能路灯 (Solar Street Lights)
- **规格**: 20W-200W
- **电池容量**: 12-50Ah
- **亮度**: 可调 LED
- **认证**: IP65, IEC 60598, CE
- **目标市场**: 路灯升级、乡村电网、临时照明
- **关键卖点**: 节能、无需布线、智能控制

### 3. 逆变器 (Inverters)
- **功率**: 1kW-10kW
- **效率**: 95%+
- **输入**: DC (48V, 96V, 192V)
- **输出**: AC (220V/230V, 50/60Hz)
- **认证**: CE, FCC, RoHS
- **目标市场**: 家用备电、商业储能、离网电源
- **关键卖点**: 高效率、多重保护、远程监控

### 4. 便携式户外灯 (Portable Outdoor Lights)
- **类型**: 帐篷灯、手电筒、露营灯
- **功率**: 5W-50W
- **电池容量**: 2000-20000mAh
- **防水等级**: IP54-IP67
- **认证**: CE, RoHS, FCC
- **目标市场**: 露营、户外活动、应急、农村家用
- **关键卖点**: 轻便、防水、快充、太阳能充电

## 🌐 地区适配关键点

### 越南
- **货币**: 越南盾 (VND) 1:1约 $1:23,000
- **支付方式**: 支付宝、微信、银行转账
- **物流枢纽**: 胡志明市、河内
- **关税**: 10-20%
- **特别注意**: 电池进口受限，需要环保证书

### 菲律宾
- **货币**: 菲律宾比索 (PHP) 1:1约 $1:56
- **支付方式**: GCash、PayMaya、银行转账
- **物流枢纽**: 马尼拉
- **关税**: 0-30%
- **特别注意**: 岛屿众多，物流成本高；进口税较高

### 马来西亚
- **货币**: 马来西亚林吉特 (MYR) 1:1约 $1:4.5
- **支付方式**: FPX、银行转账、信用卡
- **物流枢纽**: 吉隆坡、槟城
- **关税**: 0-20%
- **特别注意**: 可再生能源政策支持，市场专业化程度高

### 新加坡
- **货币**: 新加坡元 (SGD) 1:1约 $1:1.35
- **支付方式**: PayLah!, 银行转账、信用卡
- **物流**: 区域物流中心
- **关税**: 0%（��多数产品）
- **特别注意**: 物流成本低，是转运枢纽；客户要求高

### 西非 (尼日利亚、加纳等)
- **货币**: 因国而异（如尼日利亚奈拉）
- **支付方式**: 电汇、信用证、支付宝
- **物流**: 主要港口（如拉各斯）
- **关税**: 10-50%（变动大）
- **特别注意**: 太阳能需求巨大，但客户付款能力差，需要严格授信

### 中东 (阿联酋、沙特等)
- **货币**: 因国而异（如阿联酋迪拉姆）
- **支付方式**: 信用证、电汇、支付宝
- **物流**: 迪拜为主要枢纽
- **关税**: 0-5%（相对低）
- **特别注意**: 客户购买力强，要求高质量和认证；英语使用广泛

## 🚀 主要特性

### ✨ 自动化工作流
- 基于标签的自动分配
- 智能Issue分类
- 自动提醒和通知
- 跨部门协作同步

### 📋 标准化模板
- 地区特定的Issue模板
- 产品特定的合规检查清单
- 市场分析报告模板
- 多币种财务模板

### 🔄 跨部门协作
- 统一的任务管理
- 清晰的权限划分
- 实时的进度跟踪
- 完整的审计日志

### 📊 数据驱动
- FB投流ROI分析
- 地区性能对标
- 产品销售分析
- 财务健康度评估

### 🌍 国际化支持
- 多语言文档
- 地区特定的法规指南
- 多币种财务管理
- 本地化市场分析

## 📖 文档导航

| 文档 | 描述 | 链接 |
|------|------|------|
| 快速开始 | 如何快速上手本Skill系统 | [docs/getting-started.md](docs/getting-started.md) |
| 工作流指南 | 详细的工作流说明 | [docs/workflow-guide.md](docs/workflow-guide.md) |
| FB投流指南 | Facebook广告策略与执行 | [docs/fb-marketing-guide.md](docs/fb-marketing-guide.md) |
| 区域市场指南 | 各地区市场深度分析 | [docs/regional-market-guide.md](docs/regional-market-guide.md) |
| 产品指南 | 四大产品详细说明 | [docs/product-guide.md](docs/product-guide.md) |
| 海关法规 | 各地区进出口法规汇总 | [docs/customs-regulations.md](docs/customs-regulations.md) |
| 税务指南 | 各国税务申报指南 | [docs/tax-guide.md](docs/tax-guide.md) |
| 最佳实践 | 团队协作最佳实践 | [docs/best-practices.md](docs/best-practices.md) |
| 销售Skill | 销售岗位完整指南 | [skills/sales/README.md](skills/sales/README.md) |
| PM Skill | 产品经理完整指南 | [skills/pm/README.md](skills/pm/README.md) |
| 运营Skill | 运营岗位完整指南 | [skills/operations/README.md](skills/operations/README.md) |
| 财务Skill | 会计岗位完整指南 | [skills/finance/README.md](skills/finance/README.md) |
| 法务Skill | 法律岗位完整指南 | [skills/legal/README.md](skills/legal/README.md) |

## 🎓 使用场景

### 场景1: 新产品进入新市场
```
1. PM创建「市场分析」Issue
2. 销售补充「地区特定的市场洞察」
3. 法务检查「出口合规」
4. 财务计算「定价策略」
5. 运营规划「物流路由」
6. 销售准备「FB投流活动」
7. 自动生成「地区适配报告」
8. 启动Facebook投流
```

### 场景2: Facebook投流活动执行
```
1. 销售创建「FB投流活动」Issue
2. 自动标签 #sales #fb-campaign
3. 自动分配给销售主管
4. 销售设置「受众定位」和「文案素材」
5. PM验证「产品信息准确性」
6. 法务检查「广告内容合规性」
7. 销售启动投流
8. 运营/销售跟踪「线索转化」
9. 财务记录「广告成本」
10. 定期生成「ROI分析报告」
```

### 场景3: 大订单处理
```
1. 销售创建「客户线索」Issue
2. 销售跟进和报价
3. 法务审查「合同条款」
4. 客户签约
5. 运营创建「订单」Issue
6. 检查库存和生产进度
7. 准备「物流单据」和「清关表单」
8. 选择物流供应商（按目的地）
9. 财务记录收入和成本
10. 定期沟通物流进度
11. 清关完成后交付
12. 归档所有文档
```

### 场景4: 月度财务结账
```
1. 会计创建「月度财务报告」Issue
2. 收集所有「发票」和「费用报告」
3. 汇率转换（多币种）
4. 法务检查「税务合规」
5. 生成「月度财务报表」
6. 运营补充「物流成本确认」
7. 销售补充「成本分摊」
8. 准备「税务申报表」
9. 提交税务部门
10. 完成审计日志
```

## 🔐 安全与合规

- ✅ 客户数据加密存储
- ✅ 访问权限细粒度控制
- ✅ 审计日志完整记录
- ✅ GDPR合规（欧洲市场）
- ✅ 出口管制合规
- ✅ 各国税务合规
- ✅ 产品认证追踪

## 💬 支持与反馈

- 📖 查看完整文档: [docs/](docs/)
- 💬 GitHub Discussions: [讨论区](../../discussions)
- 🐛 报告问题: [提交Issue](../../issues)
- 📧 Email: support@tico.com
- 💼 商业合作: business@tico.com

## 📈 更新日志

### v2.0.0 (2026-06-15)
- ✅ 完全重构为新能源 + Facebook投流版本
- ✅ 支持6个主要目标市场
- ✅ 4大产品模块（太阳能板、路灯、逆变器、便携灯）
- ✅ 完整的地区适配指南
- ✅ FB投流工作流集成
- ✅ 多币种财务管理
- ✅ 完整的出口合规框架

### v1.0.0 (2026-06-15)
- ✅ 初始版本发布
- ✅ 五大岗位Skills实现
- ✅ 自动化工作流配置
- ✅ 完整文档编写

## 📄 License

MIT License - 详见 [LICENSE](LICENSE) 文件

---

**Made with ❤️ by Tico** | 专属新能源跨境Facebook投流Team协作工具 🌍☀️
