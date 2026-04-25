# 资产契约：quanttide 第二大脑

## 资产定义

本契约定义 quanttide 元第二大脑的资产标准。

### 资产类型

quanttide 是元第二大脑（second_brain），其资产分为两类：

- **模块资产**：子仓库/子目录形式的组成单元
- **标准资产**：标准保留文件和保留目录

### 资产标识

| 字段 | 说明 |
|------|------|
| id | 资产唯一标识，格式：`qb.<module>.<name>` |
| name | 资产名称 |
| title | 资产标题 |
| description | 资产描述 |
| owner | 资产所有者 |
| type | 资产类型 |

## 盘点范围

### 模块资产

| 标识 | 路径 |
|------|------|
| assets/quanttide-handbook | 工作手册 |
| assets/quanttide-platform | 平台 |
| assets/quanttide-profile | 工作档案 |
| assets/quanttide-specification | 工程规范 |
| domains/quanttide-data | 数据工程领域 |
| default/quanttide-founder | 创始人档案 |
| default/quanttide-tech | 科技档案 |

### 标准保留文件

| 文件 | 说明 |
|------|------|
| README.md | 项目简介 |
| CHANGELOG.md | 版本变更记录 |
| ROADMAP.md | 项目路线图 |
| CONTRIBUTING.md | 贡献指南 |
| AGENTS.md | 智能体导航 |
| LICENSE | 许可证 |

### 标准保留目录

| 目录 | 说明 |
|------|------|
| .agents/ | 智能体配置 |
| .quanttide/ | 量潮配置 |

## 动态扩展字段

| 字段 | 说明 |
|------|------|
| status | 资产状态：active/draft/archive |
| version | 当前版本 |
| last_updated | 最后更新时间 |