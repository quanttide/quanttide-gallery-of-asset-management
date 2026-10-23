# 量潮第二大脑资产类别

量潮第二大脑以 GitHub 组织 quanttide 的根仓库 quanttide/quanttide 为入口，仓库是其资产的主要形态：18 类九宫格标准资产加 Context（上下文）和 Archive（归档）两种不占格资产均以仓库为载体，由根仓库统一组织，本体系下全部仓库均须按本文件命名与组织。资产类型定义见[量潮标准范畴](https://github.com/quanttide/quanttide-meta/blob/main/docs/gallery/metaphysics/category/index.md)，本文件规定各类资产的仓库命名与组织结构。

## 双轴组织

量潮第二大脑通过**领域第二大脑**与**资产第二大脑**双轴组织：

- 领域第二大脑：`quanttide-{领域短名}`（如 quanttide-crowd、quanttide-learn），领域轴上的统一载体
- 资产第二大脑：`quanttide-{资产类型}`（如 quanttide-journal、quanttide-bylaw），范畴轴上的聚合载体
- 双轴交点：`quanttide-{资产类型}-of-{领域英文名}`（领域第二大脑内按资产类型挂载的资产子仓库）

法人主体作为默认领域：主体资产以 `business-entity` 为默认领域，命名 `quanttide-{资产类型}-of-business-entity`（如 quanttide-profile-of-business-entity），对应主体轴与范畴轴的交点。

## 仓库命名

领域第二大脑命名 `quanttide-{领域短名}`，如 quanttide-agent、quanttide-crowd、quanttide-learn；资产第二大脑命名 `quanttide-{资产类型}`，如 quanttide-journal、quanttide-profile、quanttide-roadmap、quanttide-bylaw；资产子仓库通用命名 `quanttide-{资产类型}-of-{领域英文名}`，如 quanttide-journal-of-crowd-sourcing、quanttide-bylaw-of-document-engineering。

20 类标准资产的仓库命名如下。

**程序型记忆九宫格（9 类）：**

| 资产类型 | 仓库命名 | 示例 |
|:----|:----|:----|
| Bylaw 章程 | `quanttide-bylaw-of-{领域英文名}` | quanttide-bylaw-of-document-engineering |
| Specification 工程标准 | `quanttide-specification-of-{领域英文名}` | quanttide-specification-of-course-development |
| Toolkit 标准库 | `quanttide-{领域}-toolkit` | quanttide-crowd-toolkit |
| Handbook 手册 | `quanttide-handbook-of-{领域英文名}` | quanttide-handbook-of-software-engineering |
| Gallery 案例 | `quanttide-gallery-of-{领域英文名}` | quanttide-gallery-of-course-development |
| Platform 平台 | `qt{产品名}`（产品平台）或 `qtcloud-{产品名}`（云平台） | qtcrowd、qtclass；qtcloud-learn、qtcloud-course |
| Tutorial 教程 | `quanttide-tutorial-of-{领域英文名}` | quanttide-tutorial-of-course-development |
| Essay 论文 | `quanttide-essay-of-{领域英文名}` | quanttide-essay-of-course-development |
| Laboratory 实验室 | `quanttide-laboratory-of-{领域英文名}` | quanttide-laboratory-of-crowdsourcing-management |

**陈述型记忆九宫格（9 类）：**

| 资产类型 | 仓库命名 | 示例 |
|:----|:----|:----|
| Report 报告 | `quanttide-report-of-{领域英文名}` | quanttide-report-of-software-engineering |
| Library 图书馆 | `quanttide-library-of-{领域英文名}` | quanttide-library-of-meta-engineering |
| History 历史 | `quanttide-history-of-{领域英文名}` | quanttide-history-of-devops |
| Journal 日志 | `quanttide-journal-of-{领域英文名}` | quanttide-journal-of-crowd-sourcing |
| Profile 档案 | `quanttide-profile-of-{领域英文名}` | quanttide-profile-of-course-development |
| Brochure 宣传册 | `quanttide-brochure-of-{领域英文名}` | quanttide-brochure-of-course-development |
| Roadmap 路线图 | `quanttide-roadmap-of-{领域英文名}` | quanttide-roadmap-of-learning-management |
| Insight 洞察 | `quanttide-insight-of-{领域英文名}` | quanttide-insight-of-product-development |
| Intention 愿景 | `quanttide-intention-of-{领域英文名}` | quanttide-intention-of-crowd-sourcing |

**默认资产（2 类）：**

| 资产类型 | 仓库命名 | 示例 |
|:----|:----|:----|
| Context 上下文 | `quanttide-context-of-{领域英文名}` | quanttide-context-of-agent-engineering |
| Archive 归档 | `quanttide-archive-of-{领域英文名}` | quanttide-archive-of-business-entity |

## 组织结构

领域第二大脑（领域轴与范畴轴交点的载体）内部按统一结构组织：

```text
quanttide-{领域短名}/
├── apps/          # Platform 平台资产（qt{产品名} / qtcloud-{产品名}）
├── packages/      # Toolkit 标准库资产（quanttide-{领域}-toolkit）
├── examples/      # Laboratory 实验室资产（quanttide-laboratory-of-{领域英文名}）
├── data/          # 陈述型记忆与默认资产
│   ├── context/ journal/ profile/ roadmap/ insight/ intention/
│   └── report/ library/ history/ brochure/ archive/
└── docs/          # 程序型记忆资产
    ├── bylaw/ specification/ handbook/ gallery/ tutorial/ essay/
```

资产第二大脑（范畴轴聚合层）：`quanttide-{资产类型}` 容器按 `default/`（法人主体）与 `domains/`（领域）聚合对应资产子仓库，如 quanttide-journal 下挂 default/company 与 domains/{agent, data, crowd, ...}。
