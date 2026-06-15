# 快速开始指南

欢迎使用Tico跨境外贸Team Skill插件！本指南将帮助您快速上手。

## 📌 前置要求

- GitHub账户 ✅
- 项目有读写权限 ✅
- 基本了解GitHub Issue和Pull Request ✅

## 🎯 初始化步骤

### 第1步：配置团队角色

编辑 `config/team-roles.json` 文件：

```json
{
  "roles": [
    {
      "id": "sales",
      "assignees": ["销售主管的GitHub用户名"]
    },
    {
      "id": "pm",
      "assignees": ["PM的GitHub用户名"]
    },
    // ... 其他角色
  ]
}
```

### 第2步：创建第一个Issue

#### 销售岗位Issue
1. 进入 **Issues** 标签
2. 点击 **New Issue**
3. 选择 **Sales Customer Request** 模板
4. 填写客户信息
5. 点击 **Submit new issue**

#### 产品经理Issue
1. 选择 **PM Feature Request** 模板
2. 描述功能需求
3. 设置优先级
4. 提交

### 第3步：理解工作流

每个岗位都有对应的GitHub Actions工作流，自动化以下操作：

- 📋 自动标签分配
- 👤 自动分配给相应岗位负责人
- 📢 发送Slack/钉钉通知
- 📊 更新Dashboard

## 📋 每个岗位的工作方式

### 🏢 销售岗位

**目标**：追踪客户和订单

**工作流**：
```
新客户 → 创建Issue → 自动分配销售主管 → 更新客户档案 → 订单生成
```

**常见操作**：
```bash
# 创建客户Issue
# 1. 使用Issue模板
# 2. 填写客户名称、国家、联系方式
# 3. Issue自动标记为 #sales
# 4. 系统自动分配给销售主管
```

### 📊 产品经理岗位

**目标**：管理产品需求和版本发布

**工作流**：
```
需求提交 → PM评审 → 优先级排序 → 技术规格编写 → 发布计划
```

**常见操作**：
```bash
# 创建功能需求
# 1. 提交Feature Request Issue
# 2. PM进行评审和优先级排序
# 3. 添加到项目看板
# 4. 跟踪开发进度
```

### 🚚 运营岗位

**目标**：确保订单流畅和合规

**工作流**：
```
订单确认 → 库存检查 → 物流安排 → 清关 → 发货 → 跟踪
```

**常见操作**：
```bash
# 创建订单Issue
# 1. 使用Operations Incident模板
# 2. 记录订单号、目的地、商品
# 3. 系统自动分配给运营主管
# 4. 追踪物流状态
```

### 💼 会计岗位

**目标**：管理财务和税务

**工作流**：
```
费用记录 → 自动分类 → 月度报告 → 税务申报 → 审计
```

**常见操作**：
```bash
# 创建财务报告
# 1. 提交Finance Report Issue
# 2. 填写月份和财务数据
# 3. 系统自动进行合规检查
# 4. 生成税务申报表
```

### ⚖️ 法务岗位

**目标**：管理合同和合规

**工作流**：
```
合同收集 → 自动审查 → 风险评估 → 批准 → 归档 → 审计
```

**常见操作**：
```bash
# 创建合规Issue
# 1. 提交Legal Compliance Issue
# 2. 上传合同或文件
# 3. 系统进行初步审查
# 4. 法务评估风险等级
```

## 🔄 跨部门协作流程

### 场景1：销售获得客户订单

```
销售 创建 "New Customer" Issue
        ↓
系统自动:
  • 添加 #sales 标签
  • 分配给销售主管
  • 通知PM(产品咨询)
        ↓
销售 填写客户档案
        ↓
PM 确认产品可用性
        ↓
销售 生成订单
        ↓
系统自动:
  • 添加 #operations 标签
  • 创建订单Issue给运营
        ↓
运营 启动物流流程
        ↓
法务 检查合规性(自动)
        ↓
会计 记录订单收入
        ↓
完成！
```

### 场景2：PM发起新功能开发

```
PM 创建 "Feature Request" Issue
        ↓
系统自动:
  • 添加 #product-management 标签
  • 添加到Product看板
        ↓
PM 进行需求评审
        ↓
PM 编写技术规格
        ↓
系统自动:
  • 通知相关团队
  • 更新Dashboard
        ↓
开发 开始实现
        ↓
完成！
```

## 📊 使用GitHub Projects看板

### 创建Project看板

1. 进入 **Projects** 标签
2. 点击 **New project**
3. 选择 **Table** 或 **Board** 视图
4. 添加不同岗位的看板

### 看板列（推荐）

- 📥 **待分配** - 新创建的Issue
- 🔄 **进行中** - 正在处理
- 👀 **待审批** - 等待审核
- ✅ **已完成** - 完成的任务

## 🔐 权限管理

### 推荐权限设置

**Repository Settings → Collaborators**

```
销售主管: Maintain
PM: Maintain
运营主管: Maintain
会计主管: Write
法务主管: Write
其他员工: Triage
```

## 🔔 通知设置

### 启用GitHub通知

1. 进入 **Settings → Notifications**
2. 选择 "Participating and @mentions"
3. 启用 "Email notifications"

### 集成Slack通知

1. 安装 [GitHub Slack App](https://github.com/apps/slack-github)
2. 选择频道和事件
3. 配置 `config/integrations-settings.json`

## 📚 后续步骤

1. ✅ 读完本指南
2. ✅ 配置 `config/team-roles.json`
3. ✅ 创建第一个Issue
4. ✅ 查看 [工作流指南](workflow-guide.md)
5. ✅ 阅读 [跨境法规汇总](cross-border-regulations.md)
6. ✅ 参考 [最佳实践](best-practices.md)

## ❓ 常见问题

### Q: 如何修改Issue模板？
A: 编辑 `.github/ISSUE_TEMPLATE/` 目录下的文件。

### Q: 如何添加新的团队成员？
A: 编辑 `config/team-roles.json` 并添加到 `assignees` 数组。

### Q: 工作流不工作怎么办？
A: 检查 `.github/workflows/` 中的YAML文件和GitHub Actions日志。

### Q: 如何与外部工具集成？
A: 查看 `dashboards/integration-guide.md`。

## 📞 获取帮助

- 📖 查看完整文档: [docs/](../docs)
- 💬 GitHub Discussions: [提问](../../discussions)
- 🐛 报告问题: [提交Issue](../../issues)
- 📧 Email: support@tico.com

---

**现在您已准备好使用Tico Team Skill了！祝您使用愉快！** 🎉
