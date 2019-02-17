# Amazon EBS
借助 Amazon EBS，您可以创建存储卷并将其挂载到 Amazon EC2 实例。挂载后，您便可在这些卷上创建文件系统、运行数据库，或以任何其他块储存设备使用方式使用这些卷。Amazon EBS 卷放在特定可用区内，并在其中自动复制，以保护您免受单一组件发生故障的威胁。所有 EBS 卷类型均提供快照持久性能力，旨在实现 99.999％ 的可用性。

Amazon EBS 提供一系列选项，让您可以优化工作负载的存储性能和费用。这些选项分为两大类：适用于数据库和启动卷等交易型工作负载的 SSD 型存储（性能主要取决于 IOPS），以及适用于 MapReduce 和日志处理等吞吐量密集型工作负载的 HDD 型存储（性能主要取决于吞吐量，以 MB/s 为单位）。

SSD 型卷包括适用于对延迟敏感的交易型工作负载的最高性能预配置 IOPS SSD (io1)，以及用于均衡各种交易数据的价格和性能的通用型 SSD (gp2)。HDD 型卷包括适用于频繁访问的吞吐量密集型工作负载的吞吐量优化型 HDD (st1)，以及适用于非频繁访问数据的最低成本 Cold HDD (sc1)。

弹性卷是 Amazon EBS 的一项功能，让您能够动态增加容量、调整性能并更改有效卷的类型，而无需停机，也不会影响性能。这使您可以轻松地将部署规模调整到适当大小，并适应性能变化。
## 优势
#### 可靠、安全的存储
每个 Amazon EBS 卷均在其可用区内提供冗余，保护您免受故障影响。加密功能和各种访问控制策略可以为您的数据提供强大的深度防护安全策略。
#### 稳定、低延迟的性能
Amazon EBS 通用 (SSD) 卷和 Amazon EBS 预配置 IOPS (SSD) 卷可以通过 SSD 技术实现非常低的延迟，并且 I/O 性能稳定，可以根据应用程序的需要进行扩展。
#### 备份、恢复、创新
创建 Amazon EBS 卷的时间点快照以便实现数据的长期持久性，从而保护您的数据。使用 Amazon EBS 快照创建新的 EC2 实例，大幅提升业务的灵活性。
#### 快速扩展，轻松缩减
借助 Amazon EBS，您可以优化卷的容量、性能或成本，以动态地做出调整，从而满足您的企业不断变化的需求。
#### 地理灵活性
Amazon EBS 支持跨 AWS 区域复制快照，从而实现地理扩展、数据中心迁移和灾难恢复，在保护您的业务的同时保证灵活性。
#### 性能优化
针对 Amazon EBS 优化过的实例可以为 Amazon EBS 卷提供专用的网络容量。这样可以尽可能减少 EBS 与您的实例之间的网络争用，为您的 EBS 卷提供最佳性能。
## 使用案例
#### 关系数据库
Amazon EBS 可随您的性能需要而进行扩展，无论您是在支持数百万游戏客户还是支持数十亿电子商务交易。Amazon EBS 上广泛部署了各类数据库，如 Oracle、Microsoft SQL Server、MySQL 和 PostgreSQL。
#### 企业应用程序
Amazon EBS 通过提供可靠的块存储来运行关键任务应用程序（如 Oracle、SAP、Microsoft Exchange 和 Microsoft SharePoint）来满足您的组织的多样化需要。
#### 开发和测试
Amazon EBS 使您的组织更灵敏、更快地对客户需求作出反应。只需单击几下就可以预置、复制、扩展或存档您的开发、测试和生产环境。
#### NOSQL 数据库
Amazon EBS 卷可以在运行 NoSQL 数据库时提供应用程序所需的稳定、低延迟的性能。
#### 业务连续性
通过定期跨不同地理区域备份数据和记录文件来尽可能减少数据丢失和缩短恢复时间。复制 Amazon 系统映像 (AMI) 和 EBS 快照，以在新的 AWS 区域启动应用程序。
## 定价
详情参考[定价](https://aws.amazon.com/cn/ebs/pricing/?nc=sn&loc=3)