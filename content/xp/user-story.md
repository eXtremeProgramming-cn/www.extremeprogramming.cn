# 用户故事

我们以用户故事的形式描述需求，而不使用庞大的需求文档。用户故事可以在[发布计划会议](release-planning.md)上用做时间估算的单元。用户故事应该站在客户的角度编写，描述他们希望系统提供的服务。不过，用户故事不局限于描述用户界面。用户故事应该使用三段式编写，应该使用业务的语言编写，而不应带有太多技术术语。

<!-- User stories serve the same purpose as use cases but are not the same. They are used to create time estimates for the release planning meeting. They are also used instead of a large requirements document. User Stories are written by the customers as things that the system needs to do for them. They are similar to usage scenarios, except that they are not limited to describing a user interface. They are in the format of about three sentences of text written by the customer in the customers terminology without techno-syntax. -->

同时，由用户故事还能驱动出相应的[验收测试](acceptance-test.md)。一个用户故事是否完成，必须由一个或多个自动化的验收测试来验证。

<!-- User stories also drive the creation of the acceptance tests. One or more automated acceptance tests must be created to verify the user story has been correctly implemented. -->

与传统的需求规格文档相比，用户故事最大的特点在于详细程度不同。用户故事应该只包含最低程度的细节，只要足够对完成故事所需的时间做出较有信心的估算即可。等到真的要实现这个用户故事时，开发者再去跟客户当面沟通，获取更详细的故事细节。

<!-- One of the biggest misunderstandings with user stories is how they differ from traditional requirements specifications. The biggest difference is in the level of detail. User stories should only provide enough detail to make a reasonably low risk estimate of how long the story will take to implement. When the time comes to implement the story developers will go to the customer and receive a detailed description of the requirements face to face.	 -->

开发者需要估算完成用户故事大概需要的时间。在为期2~3周的迭代中，一个故事理想的完成时间应该在1~5天。超过5天的故事就太大了，需要进一步拆分成更小的故事。不到1天的故事可以与其他故事合并。

用户故事与传统需求文档的另一个区别在于对用户诉求的重视程度。在用户故事中，应该尽量避免涉及具体的技术、数据库、算法等细节，应该尽量聚焦于用户需求和业务价值，而非详尽地描述用户界面细节。
