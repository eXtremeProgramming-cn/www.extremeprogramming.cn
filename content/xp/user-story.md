# 用户故事

用户故事与用例均服务于同样的目的，但有所不同。用户故事的作用是，可以在[发布计划会议](./release-plan.md)上用做时间估算的单元。同时，我们以用户故事的形式来描述需求，而非使用庞大的需求文档。用户故事应该站在[客户](http://www.extremeprogramming.org/rules/customer.html)的角度编写，描述他们希望系统提供的服务。这与使用场景类似，只不过用户故事不局限于用户接口层面的描述。一个用户故事应该使用三段式编写，应该使用业务的语言编写，而不应带有太多技术口语。

<!-- User stories serve the same purpose as use cases but are not the same. They are used to create time estimates for the release planning meeting. They are also used instead of a large requirements document. User Stories are written by the customers as things that the system needs to do for them. They are similar to usage scenarios, except that they are not limited to describing a user interface. They are in the format of about three sentences of text written by the customer in the customers terminology without techno-syntax. -->

同时，由用户故事还能驱动出相应的[验收测试](./functionaltests.md)。一个用户故事是否完成，必须有一个或多个自动化的验收测试来验证。

> User stories also drive the creation of the acceptance tests. One or more automated acceptance tests must be created to verify the user story has been correctly implemented.

用户故事最常被误解的一个地方，在于混淆了它与传统的需求规格说明之间的区别。它们最大的差异点在于详细程度不同。用户故事应该只包含最低程度的细节，只要足够对完成故事所需的时间做出较有信心的估算即可。等到真的要实现这个用户故事时，开发者再去跟客户当面沟通，获取更为详细的故事细节。

> One of the biggest misunderstandings with user stories is how they differ from traditional requirements specifications. The biggest difference is in the level of detail. User stories should only provide enough detail to make a reasonably low risk estimate of how long the story will take to implement. When the time comes to implement the story developers will go to the customer and receive a detailed description of the requirements face to face.	

开发者需要估算完成用户故事大概需要的时间。对于每个用户故事，开发者可能做出1周到3周不等的“理想开发时间”估算。所谓理想开发时间，指的是纯粹完成故事需要编码的工作量，而不考虑干扰、其他任务分配的情况，同时假设你对完成故事所需的步骤胸有成竹。如果估算超过3周，说明你需要将用户故事继续往下分解；如果估算小于1周，说明用户故事太过细节，可以与其他故事进行合并。在发布会议中，创建一个[发布计划](http://www.extremeprogramming.org/rules/commit.html)最完美的用户故事数目大概是80个，允许上下有20个左右的浮动。

> Developers estimate how long the stories might take to implement. Each story will get a 1, 2 or 3 week estimate in "ideal development time". This ideal development time is how long it would take to implement the story in code if there were no distractions, no other assignments, and you knew exactly what to do. Longer than 3 weeks means you need to break the story down further. Less than 1 week and you are at too detailed a level, combine some stories. About 80 user stories plus or minus 20 is a perfect number to create a release plan during release planning.

用户故事与需求文档的另一个区别在于对用户诉求的重视程度。在用户故事中，应该尽量避免涉及具体的技术、数据库、算法等细节，应该尽量聚焦于用户需求和业务价值，而非致力于详尽地描述用户界面细节。

> Another difference between stories and a requirements document is a focus on user needs. You should try to avoid details of specific technology, data base layout, and algorithms. You should try to keep stories focused on user needs and benefits as opposed to specifying GUI layouts.
