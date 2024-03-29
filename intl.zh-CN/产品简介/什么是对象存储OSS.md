# 什么是对象存储OSS

阿里云对象存储OSS（Object Storage Service）是阿里云提供的海量、安全、低成本、高持久的云存储服务。其数据设计持久性不低于99.9999999999%（12个9），服务可用性（或业务连续性）不低于99.995%。

OSS具有与平台无关的RESTful API接口，您可以在任何应用、任何时间、任何地点存储和访问任意类型的数据。

您可以使用阿里云提供的API、SDK接口或者OSS迁移工具轻松地将海量数据移入或移出阿里云OSS。数据存储到阿里云OSS以后，您可以选择标准存储（Standard）作为移动应用、大型网站、图片分享或热点音视频的主要存储方式，也可以选择成本更低、存储期限更长的低频访问存储（Infrequent Access）、归档存储（Archive）、冷归档存储（Cold Archive）作为不经常访问数据的存储方式。

## 快速了解OSS

-   短视频

    观看以下视频，快速了解OSS。

-   常见问题

    查看[OSS常见问题](/intl.zh-CN/产品简介/常见问题.md)，了解其他用户经常咨询和关注的一些问题。

-   学习路径

    您可以通过[OSS产品学习路径图](https://www.alibabacloud.com/getting-started/learningpath/oss)快速了解OSS，学习相关的基础操作，并利用丰富的API、SDK包和便捷工具进行二次开发。


## 迁移数据到OSS

您可以使用在线迁移服务将第三方数据源，如亚马逊AWS、谷歌云、腾讯云、七牛云、华为云、百度云等数据轻松迁移至OSS。详细信息，请参见[在线迁移服务使用教程](https://help.aliyun.com/product/94157.html)。

如果您有TB或PB级别的海量数据需要上传到OSS，但本地的网络带宽不够，扩容成本高，可以使用闪电立方离线数据迁移服务。详细信息，请参见[离线迁移（闪电立方）介绍](/intl.zh-CN/产品简介/什么是离线迁移（闪电立方）.md)。

## OSS相关概念

-   存储类型（Storage Class）

    OSS提供标准、低频访问、归档、冷归档四种存储类型，全面覆盖从热到冷的各种数据存储场景。其中标准存储类型提供高持久、高可用、高性能的对象存储服务，能够支持频繁的数据访问；低频访问存储类型适合长期保存不经常访问的数据（平均每月访问频率1到2次），存储单价低于标准类型；归档存储类型适合需要长期保存（建议半年以上）的归档数据；冷归档存储适合需要超长时间存放的极冷数据。更多信息，请参见[存储类型介绍](/intl.zh-CN/开发指南/存储类型/存储类型介绍.md)。

-   存储空间（Bucket）

    存储空间是您用于存储对象（Object）的容器，所有的对象都必须隶属于某个存储空间。存储空间具有各种配置属性，包括地域、访问权限、存储类型等。您可以根据实际需求，创建不同类型的存储空间来存储不同的数据。

-   对象（Object）

    对象是OSS存储数据的基本单元，也被称为OSS的文件。对象由元信息（Object Meta）、用户数据（Data）和文件名（Key）组成。对象由存储空间内部唯一的Key来标识。对象元信息是一组键值对，表示了对象的一些属性，例如最后修改时间、大小等信息，同时您也可以在元信息中存储一些自定义的信息。

-   地域（Region）

    地域表示OSS的数据中心所在物理位置。您可以根据费用、请求来源等选择合适的地域创建Bucket。更多信息，请参见[OSS已开通的地域](/intl.zh-CN/开发指南/访问域名（Endpoint）/访问域名和数据中心.md)。

-   访问域名（Endpoint）

    Endpoint表示OSS对外服务的访问域名。OSS以HTTP RESTful API的形式对外提供服务，当访问不同地域的时候，需要不同的域名。通过内网和外网访问同一个地域所需要的域名也是不同的。更多信息，请参见[各个Region对应的Endpoint](/intl.zh-CN/开发指南/访问域名（Endpoint）/访问域名和数据中心.md)。

-   访问密钥（AccessKey）

    AccessKey简称AK，指的是访问身份验证中用到的AccessKey ID和AccessKey Secret。OSS通过使用AccessKey ID和AccessKey Secret对称加密的方法来验证某个请求的发送者身份。AccessKey ID用于标识用户；AccessKey Secret是用户用于加密签名字符串和OSS用来验证签名字符串的密钥，必须保密。关于获取AccessKey的方法，请参见[创建AccessKey]()。


## OSS管理方式

OSS提供多种灵活的上传、下载和管理方式。

-   通过控制台管理OSS

    OSS提供了Web服务页面，您可以登录[OSS控制台](https://oss.console.aliyun.com/overview)管理您的OSS资源。更多信息，请参见[控制台用户指南](/intl.zh-CN/控制台用户指南/登录OSS管理控制台/使用阿里云账号登录OSS管理控制台.md)。

-   通过API或SDK管理OSS

    OSS提供RESTful API和各种语言的SDK开发包，方便您快速进行二次开发。更多信息，请参见[OSS API参考](/intl.zh-CN/API 参考/API概览.md)和[OSS SDK参考](OSS SDK参考t22258.dita#concept_dcn_tp1_kfb)。

-   通过工具管理OSS

    OSS提供图形化管理工具ossbrowser、命令行管理工具ossutil、FTP管理工具ossftp等各种类型的管理工具。更多信息，请参见[OSS常用工具](/intl.zh-CN/常用工具/OSS常用工具汇总.md)。

-   通过云存储网关管理OSS

    云存储网关：OSS的存储空间内部是扁平的，没有文件系统的目录等概念，所有的对象都直接隶属于其对应的存储空间。如果您想要像使用本地文件夹和磁盘那样来使用OSS存储服务，可以通过配置云存储网关来实现。更多信息，请参见[云存储网关产品详情页面](https://www.alibabacloud.com/product/cloud-storage-gateway)。


## OSS定价

传统的存储服务供应商会要求您购买预定量的存储和网络传输容量，如果超出此容量，就会关闭对应的服务或者收取高昂的超容量费用；如果没有超过此容量，又需要您按照全部容量支付费用。

OSS仅按照您的实际使用容量收费，您无需预先购买存储和流量容量，随着您业务的发展，您将享受到更多的基础设施成本优势。

关于OSS的价格，请参见[OSS产品定价](https://www.alibabacloud.com/product/oss#pricing)。关于OSS的计量计费方式，请参见[计量项和计费项](/intl.zh-CN/计量计费/计量项和计费项/概述.md)。

## 阿里云存储服务

除了对象存储以外，阿里云还提供文件存储、块存储等类型的存储服务，满足您不同场景下的业务需求。详细信息，请参见[阿里云存储服务白皮书](/intl.zh-CN/白皮书/阿里云存储服务概述/介绍.md)。

有关阿里云存储服务的客户案例、解决方案等，请参见[阿里云存储产品家族](https://www.alibabacloud.com/product/storage)。

## 其他相关服务

您把数据存储到OSS以后，就可以使用阿里云提供的其他产品和服务对其进行相关操作。

以下是您会经常使用到的阿里云产品和服务：

-   图片处理：对存储在OSS上的图片进行格式转换、缩放、裁剪、旋转、添加水印等各种操作。更多信息，请参见[快速使用OSS图片处理服务](/intl.zh-CN/开发指南/数据处理/图片处理指南/图片处理操作方式.md)。
-   云服务器ECS：提供简单高效、处理能力可弹性伸缩的云端计算服务。更多信息，请参见[ECS产品详情页面](https://www.alibabacloud.com/product/ecs)。
-   内容分发网络CDN：将OSS资源缓存到各区域的边缘节点，利用边缘节点缓存的数据，提升同一个文件，被边缘节点客户大量重复下载的体验。更多信息，请参见[CDN产品详情页面](https://www.alibabacloud.com/product/cdn)。
-   E-MapReduce：构建于ECS上的大数据处理的系统解决方案，基于开源的Apache Hadoop和Apache Spark，方便您分析和处理自己的数据。更多信息，请参见[E-MapReduce产品详情页面](https://www.alibabacloud.com/product/e-mapreduce)。
-   媒体处理：将存储于OSS的音视频转码成适合在PC、TV以及移动终端上播放的格式。并基于海量数据深度学习，对音视频的内容、文字、语音、场景多模态分析，实现智能审核、内容理解、智能编辑。更多信息，请参见[媒体处理产品详情页面](https://www.alibabacloud.com/product/mts)。

