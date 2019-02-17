# AWS CodeBuild
AWS CodeBuild 是一项完全托管的持续集成服务。您只需指定源代码的位置并选择构建设置，CodeBuild 就会运行构建脚本以便编译、测试和打包您的代码。没有需要预置和扩展的服务器，也没有需要安装、配置和操作的软件。
## 优势
#### 构建和测试代码
AWS CodeBuild 在预配置的构建环境中运行构建任务，此类环境中包含完成任务所需的操作系统、编程语言运行时和构建工具（例如 Apache Maven、Gradle 和 npm）。您只需指定源代码的位置并选择构建设置（例如要使用的构建环境以及要在构建过程中运行的构建命令）即可。AWS CodeBuild 会生成代码并将项目存储到 Amazon S3 存储桶中，而您也可以使用构建命令将其上传到项目存储库中。您可以使用 AWS CodePipeline、AWS 管理控制台、AWS CLI 或开发工具包来创建、管理和启动构建项目。
**预配置构建环境**
AWS CodeBuild 可以提供适用于 Java、Python、Node.js、Ruby、Go、Android、.NET Core for Linux 和 Docker 的构建环境。

**自定义构建环境**
您可以在自己的构建环境中使用 AWS CodeBuild，例如适用于 Microsoft .NET Framework 的环境。您可以将适用于您的构建任务的运行时和工具打包到 Docker 镜像中，然后将其上传到公共 Docker Hub 存储库或 Amazon EC2 Container Registry (Amazon ECR) 中。创建新构建项目时，您可以指定 Docker 镜像的位置，而 CodeBuild 会提取这一镜像，并将其用作构建项目的配置。 

#### 可配置设置
**指定构建命令**
您可以定义想要 AWS CodeBuild 执行的具体命令，例如安装构建工具包、运行单元测试和打包代码等。构建规范是一个 YAML 文件，让您能够选择要在每个构建阶段运行的命令以及选择其他设置。CodeBuild 可以使用适用于常见场景（例如使用 Apache Maven、Gradle 或 npm 的构建任务）的构建规范示例文件帮助您快速入门。

**选择计算类型**
您可以选择最能满足开发需求的计算类型。您可以从三种级别的计算容量中进行选择，每种级别都有不同的 CPU 和内存容量。这样，如果您想更快完成构建任务，就可以选择较高的 CPU 和内存计算容量；如果您的构建任务只需最低级别的 CPU 和内存容量就能完成，您可以选择较低的计算容量。  CodeBuild 支持 Linux 和 Windows 操作系统。

**选择源集成**
您可以通过多种方式使用 AWS CodeBuild 启动构建任务。例如，您可以在连接到 AWS CodeCommit、GitHub、GitHub Enterprise、Bitbucket 或 Amazon S3 之后，在 CodeBuild 中启动构建任务。您还可以使用 AWS CodePipeline 将 CodeBuild 与您的源存储库连接到一起，而 AWS CodePipeline 会在您每次提交更改时自动启动构建任务。

#### 持续集成和交付工作流程
AWS CodeBuild 采用按需计算和按使用量付费的模式，让您能够更加频繁地构建和集成代码，同时帮助您在开发过程中尽早发现错误并在其易于修复时尽早修复。您可以使用 CodeBuild 的源集成、构建命令或 Jenkins 集成功能，将其集成到现有的持续集成和持续交付 (CI/CD) 工作流程中。CodeBuild 也属于帮助您实现 CI/CD 的AWS 代码服务的一部分。您可以将 CodeBuild 插入到 AWS CodePipeline 中，而 AWS CodePipeline 会在您每次向源存储库提交更改时，在 CodeBuild 中自动构建和测试代码。您可以使用 AWS CodePipeline 向导连接您的源存储库，然后选择 CodeBuild 作为构建工具，从而创建这种 CI 工作流程。

借助 CodePipeline，您可以集成第三方负载或集成在 CodeBuild 完成构建后启动的用户界面测试工具（例如 BlazeMeter 和 Ghost Inspector），从而将持续集成工作流程轻松扩展到持续交付。然后，您可以使用与 AWS CodePipeline 集成的服务（例如 AWS CodeDeploy 和 AWS Elastic Beanstalk），将代码部署到您的实例或本地服务器。
#### 安全性和权限
您的构建项目使用特定于客户的密钥进行加密，而密钥由 AWS Key Management Service (KMS) 管理。AWS CodeBuild 与 AWS Identity and Access Management 集成，因此您可以精确控制哪些用户以及哪些 AWS 资源可以访问您的构建任务。
#### 监控
您可以使用 AWS CodeBuild 控制台、AWS CLI、开发工具包、API 或 Amazon CloudWatch 来查看有关构建任务的详细信息。AWS CodeBuild 会向您显示构建任务的开始时间、结束时间、状态和提交 ID 等信息。CodeBuild 还会将构建任务指标和日志传输到 CloudWatch。您可以使用 CloudWatch 创建自定义控制面板、设置 CloudWatch 警报、排查构建问题或查看构建日志。