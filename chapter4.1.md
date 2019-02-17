# CodeStar
AWS CodeStar 提供了您在 AWS 上快速开发、构建和部署应用程序所需的工具。借助 AWS CodeStar，您可以使用各种项目模板开始在 Amazon EC2、AWS Lambda 和 AWS Elastic Beanstalk 上开发应用程序。AWS CodeStar 项目支持多种常用编程语言，包括 Java、JavaScript、PHP、Ruby 和 Python。AWS CodeStar 提供了一种预配置的持续交付工具链，用于在 AWS 上开发、构建、测试和部署项目，让您可以加快应用程序的交付速度。通过针对不同角色（包括所有者、参与者和观察者）的内置安全策略，您可以轻松保证项目的安全访问。AWS CodeStar 中的项目控制面板让您可以轻松集中监控应用程序活动和管理日常开发任务（例如近期的代码提交、构建和部署）。AWS CodeStar 集成了 Atlassian JIRA 这种第三方问题跟踪和项目管理工具，因此您可以在 AWS CodeStar 控制面板中创建和管理 JIRA 问题。

## 优势
#### 在几分钟内开始在 AWS 上进行开发
借助 AWS CodeStar，您可以轻松建立完整的开发和持续交付工具链，来编写、构建、测试和部署您的应用程序代码。启动项目时，您可以从多种 AWS CodeStar 模板中选择适用于 Amazon EC2、AWS Lambda 和 AWS Elastic Beanstalk 的模板。您可以将 AWS CodeCommit 或 GitHub 用作项目的源代码控制。您还可以使用包括 AWS Cloud9、Microsoft Visual Studio 或 Eclipse 在内的几个选项之一编辑源代码。选择好后，底层 AWS 产品会在几分钟内完成预置，让您可以快速开始编码和部署您的应用程序。
#### 集中管理软件交付
AWS CodeStar 提供统一的用户界面，让您可以轻松协调您的日常开发活动，而不必在各种服务控制台之间来回切换。通过 AWS CodeStar 的项目控制面板，您可以集中监控应用程序活动，跟踪软件开发过程各阶段的进度，包括代码的提交、构建、测试和部署。AWS CodeStar 集成了第三方问题跟踪和项目管理工具 Atlassian JIRA Software，让您可以直接在 AWS CodeStar 控制面板中轻松管理 JIRA 问题。
#### 实现安全的团队协作
借助 AWS CodeStar，您可以和您的团队开展安全的项目协作。您可以轻松管理项目所有者、参与者和观察者的访问权限，而无需针对每项服务手动配置策略。AWS CodeStar 通过提供符合 AWS Identity and Access Management 最佳实践的基于角色的内置策略，为团队简化了设置项目访问权限的过程。
#### 有多种项目模板可选
借助 AWS CodeStar 的项目模板，您可以轻松开发各种应用程序，例如，网站、Web 应用程序、Web 服务和 Alexa 工具。AWS CodeStar 的项目模板提供多种兼容的编程语言（包括 Java、JavaScript、PHP、Ruby、C# 和 Python）代码，让您可以快速上手。

## 体验CodeStar
在CodeStar上快速创建应用还是很简单的，从选择项目模板到选择源码托管存储一个最基本的项目创建完成。
![创建流程](/assets/2019-02-17_122412.png)
#### 选择项目开发架构模板
直接上图，清晰明了，从图中可以清晰看出CodeStar根据应用种类、开发语言和AWS服务划分了很多应用模板。
![项目开发架构模板](/assets/2019-02-17_115738.png)
#### 源码托管存储库
选择应用模板后，需要用户选择源码托管位置，我们可以选择 [AWS CodeCommit](chapter4.5.md) 或者 GitHub 来托管源码。
![源码托管存储库](/assets/2019-02-17_120103.png)
#### ooh, 一个项目建好了
下图所示，就是利用CodeStar创建项目后的一个控制面板界面，目前仅支持英文、日文、韩文。
![CodeStar控制面板](/assets/2019-02-17_121934.png)
### 控制面板
看下图，现在我们来看看左侧的菜单有仪表盘、源码、构建、部署、管道、团队、插件、项目8个项目。
![控制面板](/assets/2019-02-17_124608.png)