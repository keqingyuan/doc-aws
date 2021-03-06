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

借助 AWS CodeStar 的项目模板，您可以轻松开发各种应用程序，例如，网站、Web 应用程序、Web 服务和 Alexa 工具。AWS CodeStar 的项目模板提供多种兼容的编程语言（包括 Java、JavaScript、PHP、Ruby、C\# 和 Python）代码，让您可以快速上手。

## 定价

AWS CodeStar 不会额外收取任何费用。您只需为您在 CodeStar 项目中实际预置的 AWS 资源（例如，[Amazon EC2 实例](chapter11.1.md)、[AWS Lambda 执行次数](chapter11.2.md)、[Amazon Elastic Block Store 卷](chapter26.1.md)或 [Amazon S3 存储桶](chapter26.2.md)）付费。您只需按您的实际用量付费；既没有最低费用，也无需预付费。  
详情参考[定价](https://aws.amazon.com/cn/codestar/pricing/?nc=sn&loc=3)

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
![CodeStar控制面板](/assets/2019-02-17_124608.png)

### 控制面板

看上图左侧的菜单有仪表盘、源码、构建、部署、管道、团队、插件、项目8个项目。

#### 仪表盘

仪表盘中前两个贴图（点击Close可以关闭），第一个贴图里展现项目的状态，以及关联的IDE工具。  
![CodeStar控制面板-仪表盘](/assets/2019-02-17_121934.png)  
CodeStar不仅支持自家的 [AWS Cloud9](chapter4.3.md)，同时支持Eclipse、IntelliJ、Visual Studio等流行的第三方IDE，第三方的IDE都是以插件为媒介的方式支持，插件安装方式都有详细的说明文档（见[AWS Cloud9](chapter4.3.md) 体验Visual Studio Code），下图是AWS能够支持的IDE。  
![ide](/assets/2019-02-17_131028.png)  
仪表盘其它的贴图就是其它服务的入口，例如应用监控（[AWS CloudWatch](chapter18.1.md)）、[CodePipeline](chapter4.7.md)、托管工具，通过`Add tile`添加其它的服务入口，例如：Jira、持续部署等服务。

### 源码

点击Code菜单会跳转到 [AWS CodeCommit](chapter4.5.md) 或者 GitHub。

### 构建

按下Build菜单，会跳转到 [AWS CodeBuild](chapter4.4.md) 服务。左边的菜单栏按照[源码](chapter4.5.md)、[构建](chapter4.4.md)、[部署](chapter4.6.md)、[Pipeline](chapter4.7.md)展开，每一个菜单都有一个各自的说明操`Getting started`。  
![CodeStar控制面板-构建](/assets/2019-02-17_152908.png)  
**源码**

点击源码就是 [AWS CodeCommit](chapter4.5.md) 服务。如果你使用AWS CodeCommit来托管你的源码在这里你可以看到你的源码库的信息。  
![aws codecommit](/assets/2019-02-17_155625.png)  
**构建**

构建是 [AWS CodeBuild](chapter4.4.md) 服务。这里可以通过应用列表看到我们创建的应用信息，同时也可以看到某个应用的详细信息和构建历史。

  
**部署**

部署是 [AWS CodeDeploy](chapter4.6.md) 服务。在这里对看到应用我们已经有一个没有部署信息的应用，笔者要给这个应用创建部署。  
![deploy](/assets/2019-02-17_160127.png)  
点击应用名称以后，看到下图的界面。可以看到有部署组的概念，详情见 [AWS CodeDeploy](chapter4.6.md) 部署组，部署组一般用环境或者配置来分组。  
![deploy-group](/assets/2019-02-17_162851.png)  
点击一个部署组名称，进入到部署组的详情界面，可以获知这个部署组的出发次数、警告、部署组的部署历史，创建一个部署也在这里。  
![deploy-configure](/assets/2019-02-17_163432.png)  
点击`Create deployment`按钮，展现下图的界面，[AWS CodeDeploy](chapter4.6.md) 有部署配置和回滚策略相比较PSET而言这是一个亮点。  
![create-deployment](/assets/2019-02-17_163724.png)  
_**部署配置：**_是一组规则，用于确定部署应用程序的速度以及部署的成功或失败条件。  
_**回滚策略：**_如果开启回滚策略，部署失败时或者遇满足警报阈值时回滚

**Pipeline**  
Pipeline是 [AWS CodePipeline](chapter4.7.md) 服务。点击`Pipelines`菜单后如下图所示，已经有一个预制的Pipeline，截至目前位置，读者可能已经发现AWS在每一个惨淡下面都会预置了一个项目，这都预置都是基于我们在创建项目时所选择的项目开发架构模板。  
![pipeliine](/assets/2019-02-17_165947.png)  
点击Pipeline的名字，展现下图，从源码到部署一个完整的流水线。  
![pipeline](/assets/2019-02-17_170651.png)

#### 团队

在这里，您可以轻松管理项目所有者、参与者和观察者的访问权限，而无需针对每项服务手动配置策略。AWS CodeStar 通过提供符合 AWS Identity and Access Management 最佳实践的基于角色的内置策略，为团队简化了设置项目访问权限的过程。  
![team](/assets/2019-02-17_173652.png)

#### 插件

查看你的项目使用到了那些插件，笔者的项目托管在GitHub上，所以有GitHub插件，Jira插件时项目管理需要使用。  
![extensions](/assets/2019-02-17_173911.png)

### Projects

这里你可以看到项目用到的服务资源，以及删除项目操作。  
![projects](/assets/2019-02-17_175614.png)

