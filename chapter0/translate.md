# Preface Or (只翻译目录结构)


## 浏览这本书

本书有两个主要部分，每个部分有四个章节，每个章节后面都有一个相对独立的章节。

书的第一个部分是*The Beam Model*,重点介绍最初为*Google Cloud Dataflow*开发的批处理流数据模型(现在被捐赠给Apache软件基金会),这个模型的大部分内容在现行业中的系统仍然能够看到它的影子。
第一部分*The Beam Model*包含了四个章节。

第一章节*Streaming 101*, 涵盖了流处理的基础知识，建立了一些术语，讨论了流系统的功能，区分两个重要的时间域（处理时间和事件时间），最后介绍了一些常见的数据处理模式。


第二章节*The What, Where, When, and How of Data Processing*,详细介绍了乱序数据流处理的核心概念，每个概念都在一个具体的运行示例的上下文中进行了分析,并且带有动画图来突出时间维度。

第三章节*Watermarks*,深入研究时间进度指标(temporal progress metrics)，指出它们如何被创建并在管道(pipelines)中传播的。章节的最后会通过两个真实的*Watermarks*案例结尾

第四章节*Advanced Windowing*,和第二章衔接，深入探讨一些高级的窗口化和触发概念，例如处理时间窗口，会话和连续触发器。

在第一部分和第二部分之间，我们插入了一章很重要的内容--第五章节*Exactly-Once and Side Effects*,这一章节列举了提供端到端的精确一次处理语义的挑战，并且详细介绍了三种不同实现Apache Flink，Apache Spark和Google Cloud 数据流。

接下来开始就是第二部分*Streams and Tables*,它深入研究底层数据中“流和表”,内容被分解成四个模块

第六章节*Streams and Tables*,介绍了流和表的基本概念，通过流和表的角度分析了经典的MapReduce方法，然后构建了一种流和表的理论,该理论足够涵盖*The Beam Model*的内容。

第七章节*The Practicalities of Persistent State*,

第八章节*Streaming SQL*,探讨了关系代数和SQL上下文中流的含义，对比了Beam模型和经典SQL（当今存在的）中固有的流和表偏差，并提出了在SQL中纳入健壮流语义的一组可行途径。

第九章节*Streaming Joins*,这章研究了各种不同的streaming join类型，分析了它们在流传输上下文中的行为。最后，详细介绍了一个有用的但缺乏支持的流连接用例：时间有效性窗口。

最后，用第十章节*The Evolution of Large-Scale Data Processing*,结束本书,该章节回顾了数据处理系统MapReduce沿袭的重要历史，考察了将流传输系统发展到今天的一些重要贡献。

