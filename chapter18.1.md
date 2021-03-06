# Amazon CloudWatch

Amazon CloudWatch 是一种监控和管理服务，可提供有关 AWS、混合及本地应用程序和基础设施资源的数据和切实见解。借助 CloudWatch，您可以从一个平台收集和访问以日志和指标形式提供的所有性能和运行数据。这使您能够解决监控孤立环境（服务器、网络和数据库等）中的单个系统和应用程序面临的挑战。通过 CloudWatch，您可以监控整个堆栈（应用程序、基础设施和服务），并利用警报、日志和事件数据来执行自动操作并缩短解决问题的平均时间 \(MTTR\)。这释放了重要的资源，使您可以专注于构建应用程序和创造业务价值。

CloudWatch 可为您提供切实见解，有助于您优化应用程序性能，管理资源利用率并了解整个系统的运行状况。CloudWatch 提供最多 1 秒的指标和日志数据可见性，可保留 15 个月的数据（指标）并针对指标执行计算。这使您可以执行历史分析以便优化成本，并获得实时见解以优化应用程序和基础设施资源。

## 优势

#### 从单一平台访问您的所有数据

现代应用程序具有分布式的特点（即在微服务架构上运行）并且会以指标、日志等形式生成大量数据。您需要有一种简单易用的方式，从这些孤立的数据来源（服务器、网络、数据库等）收集、访问和整理数据，从而有效地监控应用程序和基础设施资源。Amazon CloudWatch 让您可以从在 AWS 和本地服务器上运行的所有 AWS 资源、应用程序和服务收集指标和日志，帮助您打破数据孤岛，从而可以轻松获得整个系统的可见性。

#### 采集自定义和精细化的 AWS 资源指标的最简单方式

使用 Amazon CloudWatch 时，监控 AWS 资源轻而易举。CloudWatch 与 Amazon EC2、Amazon DynamoDB、Amazon S3、Amazon ECS、AWS Lambda 和 Amazon API Gateway 等 70 多种 AWS 服务原生集成，可自动发布频率为 1 分钟的详细指标和粒度高达 1 秒的自定义指标。您可以使用 AWS Systems Manager 来安装 CloudWatch 代理，或者使用 CloudWatch API 轻松收集和发布此类数据并将其存储在 CloudWatch 中。

#### 跨应用程序、基础设施和服务的可见性

在分布式堆栈中获得可见性即可关联和可视化指标和日志，从而快速确定并解决问题。使用 Amazon CloudWatch，您能够可视化 CPU 利用率和内存等关键指标。您还可以将错误等日志模式与特定指标相关联，从而快速获知具体情况，诊断问题并了解根本原因。

#### 降低总体拥有成本

Amazon CloudWatch 使您能够设置高精度警报和采取自动化操作。这意味着将会释放重要资源，集中用于增加业务价值。例如，您可以获得有关 Amazon EC2 实例的警报，并设置 Auto Scaling 来添加或删除实例。您还可以执行自动响应来检测和关闭未使用的 EC2 资源，从而减少超额计费情况并提高资源优化率。

#### 优化应用程序和运营资源

您需要统一的运营视图、实时的粒度数据和历史参考内容，以便优化性能和资源利用率。使用 Amazon CloudWatch，您可以实现粒度为 1 秒的增强监控，并将指标存储和保留长达 15 个月。您还可以利用指标数学等原生 CloudWatch 功能来计算指标数据。例如，您可以汇总整个 EC2 实例队列的使用数据，以获得运营和利用率见解。

#### 从日志中获取可行动的见解

借助 Amazon CloudWatch Logs Insights，您可以即时了解、分析和直观显示日志，从而轻松排查运营问题。使用 Logs Insights，您仅需为运行的查询付费。Logs Insights 可以根据您的日志数量和查询复杂度进行扩展，从而在几秒钟内提供答案。此外，您还可以发布基于日志的指标、创建警报，在 CloudWatch 控制面板中将日志和指标关联起来，从而获得完全的运营可见性。

## 定价

详情参考[定价](https://aws.amazon.com/cn/cloudwatch/pricing)

