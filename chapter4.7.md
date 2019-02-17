# AWS CodePipeline
AWS CodePipeline 是一种完全托管的持续集成与持续交付服务，可以帮助您实现发布管道的自动化，从而实现快速而可靠的应用程序和基础设施更新。代码一旦发生更改，CodePipeline 都会根据您定义的发布模型自动构建、测试和部署您的发布流程。这使您能够快速而可靠地提供各种功能和更新。您可以将 AWS CodePipeline 与 GitHub 等第三方服务或您自己的自定义插件轻松集成。
#### 工作流程建模
管道定义了您的发布工作流程，并描述了新代码更改在发布过程中的进展情况。管道包括一系列阶段（例如，构建、测试和部署），可充当您工作流程中的逻辑分区。每个阶段由一系列操作组成，如构建代码或部署到测试环境等任务。AWS CodePipeline 为您提供了一个图形用户界面，用于创建，配置和管理您的管道及其各个阶段和操作，使您可以轻松地对发布工作流程进行可视化和建模。

#### 并行执行
您可以使用 CodePipeline 对构建、测试和部署操作进行建模，以便并行运行，从而提高工作流程的速度。

#### AWS integrations
AWS CodePipeline 可以直接从 AWS CodeCommit、GitHub、Amazon ECR 或 Amazon S3 为您的管道提取源代码。它可在 AWS CodeBuild 中运行构建和单元测试。CodePipeline 可使用 AWS CodeDeploy、AWS Elastic Beanstalk、Amazon Elastic Container Service (Amazon ECS) 或 AWS Fargate 部署您的更改。

您还可以对 AWS CloudFormation 操作进行建模，从而在发布流程中预置、更新或删除 AWS 资源。如此一来，您还能持续交付使用 AWS Lambda、Amazon API Gateway、Amazon DynamoDB 和 AWS Serverless Application Model (AWS SAM) 构建的无服务器应用程序。

您也可以使用 CodePipeline 与 AWS Lambda 的集成，在管道的任意阶段触发由代码定义的自定义函数。例如，您可以触发一个测试您的 Web 应用程序是否成功部署的 Lambda 函数。

借助 CodePipeline，您可以配置一个将这些服务与第三方开发人员工具和自定义系统联系在一起的管道。
#### 预构建插件
借助 AWS CodePipeline，您只单击一下即可将第三方开发人员工具（如 GitHub 或 Jenkins）集成到发布过程的任何阶段。您可以使用第三方工具进行源代码控制、构建、测试或部署。有关集成的更多信息，请参阅此处。
#### 自定义插件
AWS CodePipeline 让您可以集成自己的自定义系统。通过将 CodePipeline 开源代理与您的服务器集成，您可以注册一个自定义操作，以便将服务器连接到您的管道。您也可以使用 CodePipeline Jenkins 插件将现有的构建服务器轻松注册为自定义操作。
#### 声明式模板
借助 AWS CodePipeline，您可以通过指定您发布工作流程及其阶段和操作的声明性 JSON 文档来定义管道结构。这些文档使您能够更新现有管道，以及提供用于创建新管道的起始模板。
#### 访问控制
AWS CodePipeline 使用 AWS IAM 来管理谁可以更改您的发布工作流程，以及谁可以控制它。您可以通过 IAM 用户、IAM 角色和 SAML 集成目录授予用户访问权限。
## 优势
#### 快速交付
AWS CodePipeline 可帮助您实现软件发布流程的自动化，从而使您能够向用户快速发布新功能。凭借 CodePipeline，您可以快速迭代反馈并将新功能更快地交付给客户。

自动化构建、测试和发布过程可使您轻松测试每次代码更改并捕获易于修复的小型漏洞。您可以针对每一项更改运行调试和发布流程，从而保证应用程序或基础设施代码的质量。
#### 可配置工作流
借助 AWS CodePipeline，您可以使用控制台界面、AWS CLI、AWS CloudFormation 或 AWS SDK 为软件发布流程的每个不同阶段建模。您可以轻松指定要运行的测试，并自定义部署应用程序及其依赖项的步骤。
#### 快速入门
凭借 AWS CodePipeline，您可以立即开始对软件发布流程进行建模。无需预置或设置服务器。CodePipeline 是一种完全托管型持续交付服务，可连接到您的现有工具和系统。
#### 易于集成
AWS CodePipeline 可以轻松扩展以适应您的特定需求。您可以在发布流程的任何阶段使用我们的预建插件或您自己的自定义插件。例如，您可以从 GitHub 拉取您的源代码，使用本地 Jenkins 构建服务器，使用第三方服务运行负载测试，或将部署信息传递到您的自定义操作控制面板。
