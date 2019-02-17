# AWS X-Ray
借助 AWS X-Ray，开发人员能够轻松分析其生产行为及具有端到端跟踪功能的分布式应用程序。您可以使用 X-Ray 确定性能瓶颈、边缘情况错误以及其他难于检测的问题。X-Ray 支持各种类型或大小的开发或生产应用程序，从简单的异步事件调用和三层 Web 应用程序到使用微服务架构构建的复杂的分布式应用程序。这让开发人员能够快速找到并解决其应用程序中出现的问题，并改善最终用户对其应用程序的体验。
## 优势
#### 设置简单
AWS X-Ray 可以与在 Amazon Elastic Compute Cloud (EC2)、Amazon EC2 Container Service (Amazon ECS)、AWS Lambda 和 AWS Elastic Beanstalk 上运行的应用程序配合使用。X-Ray 的入门很简单。您只需将 X-Ray 软件开发工具包与您的应用程序集成并安装 X-Ray 代理即可。使用 AWS Elastic Beanstalk 时，您只需将 X-Ray 软件开发工具包与您的应用程序集成，因为 Elastic Beanstalk 上预安装了 X-Ray 代理。
#### 端到端跟踪
AWS X-Ray 提供一个对应用程序所作请求的端到端、跨服务视图。它为您提供一个流经应用程序且以应用程序为中心的请求视图，具体方法是将从应用程序中各个服务收集的数据整合到一个称为“轨迹”的单元。您可以使用该轨迹跟踪单个请求流经应用程序中每个服务或层的路径，以便查明问题所在。

#### AWS 服务和数据库集成

AWS X-Ray 支持在 Amazon Elastic Compute Cloud (Amazon EC2)、Amazon EC2 Container Service (Amazon ECS)、AWS Lambda 和 AWS Elastic Beanstalk 上运行的应用程序。X-Ray 软件开发工具包可以捕获有关对 MySQL 和 PostgreSQL 数据库 （自托管、Amazon RDS、Amazon Aurora）及 Amazon DynamoDB 所作请求的元数据。它还可以捕获有关对 Amazon Simple Queue Service 和 Amazon Simple Notification Service 所作请求的元数据。

支持多种语言

AWS X-Ray 可跟踪以 Node.js、Java 和 .NET 编写的应用程序。

请求采样

您可以设置最适合您的生产应用程序或开发应用程序的轨迹采样率。X-Ray 会持续跟踪对您的应用程序作出的请求并存储您的分析请求采样。这会为您提供能够使您的分析有意义的适量数据，同时避免因存储和管理过多数据而产生额外开销。
#### 服务地图
AWS X-Ray 会创建一个可供应用程序使用的服务地图，其中包含轨迹数据，您可以使用此类数据深入调查具体服务或问题。此服务地图提供了应用程序中的服务与各个服务的整合数据之间的连接视图，其中包括平均延迟和故障率。您可以创建依赖关系树、执行跨可用区或跨区域调用检测等。
![service-map](/assets/X-Ray_Screenshot1.b5f74e2132e72c0d180bb2199d20238742753b2f.jpg)
![trace](/assets/X-Ray_Screenshot2.75f8f7dfe80e70b94f401291d1ae3cb0fc9b4ba3.png)
#### 检测服务器端延迟和客户端延迟
借助 AWS X-Ray，您可以直接从服务地图直观地检测出节点和边缘的延迟分布情况。您可以快速隔离异常、以图表形式表示模式和趋势、深入了解轨迹数据，并按内置的键和自定义注释进行筛选，以更清楚地了解影响您的应用程序和最终用户的性能问题。
#### 数据注释和筛选
借助 AWS X-Ray，可以向应用程序中特定组件或服务释放出的数据添加注释。您可以使用此方法添加特定于业务的元数据，以便帮助您更好地诊断问题。您还可以按注释值、平均延迟、HTTP 响应状态、时间戳、使用的数据库表等属性查看和筛选轨迹数据。