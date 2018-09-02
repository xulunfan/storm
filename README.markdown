Storm最初由Nathan Marz和BackType的团队创建。BackType是一家社交分析公司。后来，Storm被收购，并通过Twitter开源。在短时间内，Apache Storm成为分布式实时处理系统的标准，允许您处理大量的数据，类似于Hadoop。Apache Storm是用Java和Clojure写的。它仍然是实时分析的领导者。

什么是Apache Storm？
Apache Storm是一个分布式实时大数据处理系统。Storm设计用于在容错和水平可扩展方法中处理大量数据。它是一个流数据框架，具有最高的摄取率。虽然Storm是无状态的，它通过Apache ZooKeeper管理分布式环境和集群状态。它很简单，您可以并行地对实时数据执行各种操作。
Apache Storm继续成为实时数据分析的领导者。Storm易于设置和操作，并且它保证每个消息将通过拓扑至少处理一次。

Apache Storm vs Hadoop
基本上Hadoop和Storm框架用于分析大数据。两者互补，在某些方面有所不同。Apache Storm执行除持久性之外的所有操作，而Hadoop在所有方面都很好，但滞后于实时计算。
| Storm | Hadoop |
| - | :-: |
| 实时流处理 | 批量处理|
| 无状态 | 有状态 |
| 主/从架构与基于ZooKeeper的协调。主节点称为nimbus，从属节点是主管。 | 具有/不具有基于ZooKeeper的协调的主-从结构。主节点是JobTracker，从节点是TaskTracker。 | 

使用Apache Storm的例子
Apache Storm对于实时大数据流处理非常有名。因此，大多数公司都将Storm用作其系统的一个组成部分。一些值得注意的例子如下:
Twitter - Twitter正在使用Apache Storm作为其“发布商分析产品”。 “发布商分析产品”处理Twitter平台中的每个tweets和点击。 Apache Storm与Twitter基础架构深度集成。
NaviSite - NaviSite正在使用Storm进行事件日志监控/审计系统。系统中生成的每个日志都将通过Storm。Storm将根据配置的正则表达式集检查消息，如果存在匹配，那么该特定消息将保存到数据库。
Wego - Wego是位于新加坡的旅行元搜索引擎。旅行相关数据来自世界各地的许多来源，时间不同。Storm帮助Wego搜索实时数据，解决并发问题，并为最终用户找到最佳匹配。

Apache Storm优势
下面是Apache Storm提供的好处列表：

    Storm是开源的，强大的，用户友好的。它可以用于小公司和大公司。

    Storm是容错的，灵活的，可靠的，并且支持任何编程语言。

    允许实时流处理。

    Storm是令人难以置信的快，因为它具有巨大的处理数据的力量。

    Storm可以通过线性增加资源来保持性能，即使在负载增加的情况下。它是高度可扩展的。

    Storm在几秒钟或几分钟内执行数据刷新和端到端传送响应取决于问题。它具有非常低的延迟。

    Storm有操作智能。

    Storm提供保证的数据处理，即使群集中的任何连接的节点死或消息丢失。
    
Master Branch:  
[![Travis CI](https://travis-ci.org/apache/storm.svg?branch=master)](https://travis-ci.org/apache/storm)
[![Maven Version](https://maven-badges.herokuapp.com/maven-central/org.apache.storm/storm-core/badge.svg)](http://search.maven.org/#search|gav|1|g:"org.apache.storm"%20AND%20a:"storm-core")
 
Storm is a distributed realtime computation system. Similar to how Hadoop provides a set of general primitives for doing batch processing, Storm provides a set of general primitives for doing realtime computation. Storm is simple, can be used with any programming language, [is used by many companies](http://storm.apache.org/documentation/Powered-By.html), and is a lot of fun to use!

The [Rationale page](http://storm.apache.org/documentation/Rationale.html) explains what Storm is and why it was built. [This presentation](http://vimeo.com/40972420) is also a good introduction to the project.

Storm has a website at [storm.apache.org](http://storm.apache.org). Follow [@stormprocessor](https://twitter.com/stormprocessor) on Twitter for updates on the project.

## Documentation

Documentation and tutorials can be found on the [Storm website](http://storm.apache.org/documentation/Home.html).

Developers and contributors should also take a look at our [Developer documentation](DEVELOPER.md).
 

## Getting help

__NOTE:__ The google groups account storm-user@googlegroups.com is now officially deprecated in favor of the Apache-hosted user/dev mailing lists.

### Storm Users
Storm users should send messages and subscribe to [user@storm.apache.org](mailto:user@storm.apache.org).

You can subscribe to this list by sending an email to [user-subscribe@storm.apache.org](mailto:user-subscribe@storm.apache.org). Likewise, you can cancel a subscription by sending an email to [user-unsubscribe@storm.apache.org](mailto:user-unsubscribe@storm.apache.org).

You can also [browse the archives of the storm-user mailing list](http://mail-archives.apache.org/mod_mbox/storm-user/).

### Storm Developers
Storm developers should send messages and subscribe to [dev@storm.apache.org](mailto:dev@storm.apache.org).

You can subscribe to this list by sending an email to [dev-subscribe@storm.apache.org](mailto:dev-subscribe@storm.apache.org). Likewise, you can cancel a subscription by sending an email to [dev-unsubscribe@storm.apache.org](mailto:dev-unsubscribe@storm.apache.org).

You can also [browse the archives of the storm-dev mailing list](http://mail-archives.apache.org/mod_mbox/storm-dev/).

Storm developers who would want to track the JIRA issues should subscribe to [issues@storm.apache.org](mailto:issues@storm.apache.org).

You can subscribe to this list by sending an email to [issues-subscribe@storm.apache.org](mailto:issues-subscribe@storm.apache.org). Likewise, you can cancel a subscription by sending an email to [issues-unsubscribe@storm.apache.org](mailto:issues-unsubscribe@storm.apache.org).

You can view the archives of the mailing list [here](http://mail-archives.apache.org/mod_mbox/storm-issues/).

### Issue tracker
In case you want to raise a bug/feature or propose an idea, please use [Apache Jira](https://issues.apache.org/jira/projects/STORM)

### Which list should I send/subscribe to?
If you are using a pre-built binary distribution of Storm, then chances are you should send questions, comments, storm-related announcements, etc. to [user@storm.apache.org](mailto:user@storm.apache.org).

If you are building storm from source, developing new features, or otherwise hacking storm source code, then [dev@storm.apache.org](mailto:dev@storm.apache.org) is more appropriate.

If you are committers and/or PMCs, or contributors looking for following up and participating development of Storm, then you would want to also subscribe [issues@storm.apache.org](issues@storm.apache.org) in addition to [dev@storm.apache.org](dev@storm.apache.org).

### What will happen with storm-user@googlegroups.com?
All existing messages will remain archived there, and can be accessed/searched [here](https://groups.google.com/forum/#!forum/storm-user).

New messages sent to storm-user@googlegroups.com will either be rejected/bounced or replied to with a message to direct the email to the appropriate Apache-hosted group.

### IRC
You can also come to the #storm-user room on [freenode](http://freenode.net/). You can usually find a Storm developer there to help you out.

## License

Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.


## Project lead

* Nathan Marz ([@nathanmarz](http://twitter.com/nathanmarz))

## Committers

* James Xu ([@xumingming](https://github.com/xumingming))
* Jason Jackson ([@jason_j](http://twitter.com/jason_j))
* Andy Feng ([@anfeng](https://github.com/anfeng))
* Flip Kromer ([@mrflip](https://github.com/mrflip))
* David Lao ([@davidlao2k](https://github.com/davidlao2k))
* P. Taylor Goetz ([@ptgoetz](https://github.com/ptgoetz))
* Derek Dagit ([@d2r](https://github.com/d2r))
* Robert Evans ([@revans2](https://github.com/revans2))
* Michael G. Noll ([@miguno](https://github.com/miguno))
* Kishor Patil ([@kishorvpatil](https://github.com/kishorvpatil))
* Sriharsha Chintalapani([@harshach](https://github.com/harshach))
* Sean Zhong ([@clockfly](http://github.com/clockfly))
* Kyle Nusbaum ([@knusbaum](https://github.com/knusbaum))
* Parth Brahmbhatt ([@Parth-Brahmbhatt](https://github.com/Parth-Brahmbhatt))
* Jungtaek Lim ([@HeartSaVioR](https://github.com/HeartSaVioR))
* Aaron Dossett ([@dossett](https://github.com/dossett))
* Matthias J. Sax ([@mjsax](https://github.com/mjsax))
* Arun Mahadevan ([@arunmahadevan](https://github.com/arunmahadevan))
* Boyang Jerry Peng ([@jerrypeng](https://github.com/jerrypeng))
* Zhuo Liu ([@zhuoliu](https://github.com/zhuoliu))
* Haohui Mai ([@haohui](https://github.com/haohui))
* Sanket Chintapalli ([@redsanket](https://github.com/redsanket))
* Longda Feng ([@longda](https://github.com/longdafeng))
* John Fang ([@hustfxj](https://github.com/hustfxj))
* Abhishek Agarwal ([@abhishekagarwal87](https://github.com/abhishekagarwal87))
* Satish Duggana ([@satishd](https://github.com/satishd))
* Xin Wang ([@vesense](https://github.com/vesense))
* Hugo da Cruz Louro ([@hmcl](https://github.com/hmcl))
* Stig Rohde Døssing ([@srdo](https://github.com/srdo/))
* Roshan Naik ([@roshannaik](http://github.com/roshannaik))
* Ethan Li ([@Ethanlm](https://github.com/Ethanlm))

## Acknowledgements

YourKit is kindly supporting open source projects with its full-featured Java Profiler. YourKit, LLC is the creator of innovative and intelligent tools for profiling Java and .NET applications. Take a look at YourKit's leading software products: [YourKit Java Profiler](http://www.yourkit.com/java/profiler/index.jsp) and [YourKit .NET Profiler](http://www.yourkit.com/.net/profiler/index.jsp).
