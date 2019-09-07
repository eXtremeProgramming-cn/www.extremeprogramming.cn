# 发布计划

[comment]: <原文> (A release planning meeting is used to create a release plan, which lays out the overall project. The release plan is then used to create iteration plans for each individual iteration.)

发布计划会议用来制订[发布计划](/content/xp/release-plan.md)，以规划整个项目。发布计划稍后会用于为每个[迭代](/content/xp/iterative.md)创建迭代计划。


[comment]: <原文> (It is important for technical people to make the technical decisions and business people to make the business decisions. Release planning has a set of rules that allows everyone involved with the project to make their own decisions. The rules define a method to negotiate a schedule everyone can commit to.)

技术人员做技术决策，业务人员做业务决策，这至关重要。发布计划提供了一套规则，允许参与项目的每个人做出自己的决策。这套规则定义了一种方法，使得每个人可以协商时间表。


[comment]: <原文> (The essence of the release planning meeting is for the development team to estimate each user story in terms of ideal programming weeks. An ideal week is how long you imagine it would take to implement that story if you had absolutely nothing else to do. No dependencies, no extra work, but do include tests. The customer then decides what story is the most important or has the highest priority to be completed.)

发布计划会议的实质是让开发人员以理想开发时间来估算[用户故事](/content/xp/user-story.md)。理想开发时间，是指在没有干扰、没有依赖、没有额外工作、但必须包含测试的情况下，完成一个用户故事所花费的时间。然后，客户决定哪个用户故事最重要或者具有最高的优先级。


[comment]: <原文> (User stories are printed or written on cards. Together developers and customers move the cards around on a large table to create a set  of stories to be implemented as the first \(or next\) release. A useable, testable system that makes good business sense delivered early is desired.)

用户故事会被打印或者写到卡片上。开发人员和客户一起围绕着大桌子移动卡片，为第一次（或下一次）发布选定一组待实现的卡片。[尽早交付](/content/xp/small-release.md)可用、可测试、且具有良好商业价值的系统，才是人们所期望的。


[comment]: <原文> (You may plan by time or by scope. The project velocity is  used  to  determine  either how many stories can be implemented before a given date \(time\) or how long a set of stories will take to finish \(scope\). When planning by time multiply the number of iterations by the project velocity to determine how many user stories can be completed. When planning by scope divide the total weeks of estimated user stories by the project velocity to determine how many iterations till the release is ready.)

可以按时间或范围规划发布计划。[项目速率](/content/xp/velocity.md)可用来确定在指定日期前可完成多少用户故事（时间），或一组用户故事需要多久才能完成（范围）。按时间进行规划时，将迭代次数乘以项目速率，可确定能够完成多少用户故事。按范围进行规划时，将用户故事的总预估理想开发时间除以项目速率，即可确定完成发布需要多少次迭代。


[comment]: <原文> (Individual iterations are planned in detail just before each iteration begins and not in advance. The release planning meeting was called the planning game and the rules can be found at the Portland Pattern Repository.)

在每个迭代开始之前而不是提前计划每一个迭代。发布计划会议也被称作计划游戏，可在[Portland Pattern Repository](http://c2.com/cgi/wiki?PlanningGame)找到相关的规则。


[comment]: <原文> (When the final release plan is created and is displeasing to management it is tempting to just change the estimates for the user stories. You must not do this. The estimates are valid and will be required as-is during the iteration planning meetings. Underestimating now will cause problems later. Instead negotiate an acceptable release plan. Negotiate until the developers, customers, and managers can all agree to the release plan.)

当所有发布计划已创建完成，但管理人员却感到不满时，最容易犯的错误就是去改变用户故事的估算。你绝不应该这么做。估算应是每位参与者所认可的，并且应该在后继的[迭代规划会议](/content/xp/iteration-plan.md)中坚持相同的原则。低估将会造成问题。所以，应该协商一个可接受的发布计划，直到开发人员、客户、管理人员满意为止。


[comment]: <原文> (The base philosophy of release planning is that a project may be quantified by four variables; scope, resources, time, and quality. Scope is how much is to  be  done.  Resources  are  how  many people are available. Time is when the project or release will be done. And quality is how good the software will be and how well tested it will be.)

发布计划的基本理念是项目可以通过4个变量来限定：范围、资源、时间和质量。范围即需要完成多少内容；资源即有多少可用的人；时间即何时发布或完成项目；质量即软件的好坏以及是否经过良好的测试和验证。


[comment]: <原文> (No one can control all 4 variables.  When you change one you inadvertently cause another to change in response.  Note that lowering quality to any less than excellent has unforeseen impact on the other 3 variables that may not become obvious until your project slows to a crawl just before the deadline.)

没有人能够控制所有4个变量。改变一个变量将不可避免的导致其他变量的变化。值得注意的是，降低质量将可能导致项目在其他方面出现不可预料的影响，这些影响有可能直到项目慢如蜗牛且已到最后一刻时才会被察觉。


[comment]: <原文> (In essence there are only 3 variables that you actually want to change. Management can set 2 of those variables and the third will be set by the development team.  Also let the developers moderate the customers desire to have the project done immediately by hiring too many people at one time.)

本质上，只有三个变量可被改变。管理人员可设置其中的两个，第三个变量可由开发团队来设置。并允许开发人员遏制客户企图通过同时雇佣大量人员迅速完成项目的欲望。
