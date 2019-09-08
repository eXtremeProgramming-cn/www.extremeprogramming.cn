# 验收测试

验收测试源于用户故事。在迭代计划会议上，客户会选择当前迭代要开发哪些故事。在迭代进行的过程中，这些被选中的用户故事会被翻译成验收测试。客户需要指定测试场景，用来检查用户故事是否实现。用户故事可以对应一个或多个验收测试，用来确保功能正常工作。

验收测试是黑盒测试。每一个验收测试有一些期望系统输出的结果。客户负责检验测试是否通过，并且在有测试失败的时候决定哪个失败的测试优先级最高。验收测试也作为发布前的回归测试。

用户故事只有通过了所有的验收测试，才能被视为完成。也就是说，每次迭代都要创建验收测试，否则开发团队就不会有任何进展。

QA（质量保障）是极限编程很重要的一部分。在一些项目中，QA是由专门的团队来执行；另一些项目中，QA是开发团队的一部分。无论哪种情况，极限编程都要求开发和QA联系非常紧密。

验收测试应该自动化，这样就可以经常运行。验收测试的结果应该发给团队成员。团队负责在迭代中安排时间修复失败的验收测试。

“验收测试”这个名字是从“功能测试”转变而来。新的名字更好地反映了测试的目的：它保证了客户需求得到满足，因而系统验收通过了。

 
<!-- Acceptance tests are created from user stories. During an iteration the user stories selected during the iteration planning meeting will be translated into acceptance tests. The customer specifies scenarios to test when a user story has been correctly implemented. A story can have one or many acceptance tests, what ever it takes to ensure the functionality works.

Acceptance tests are black box system tests. Each acceptance test represents some expected result from the system. Customers are responsible for verifying the correctness of the acceptance tests and reviewing test scores to decide which failed tests are of highest priority. Acceptance tests are also used as regression tests prior to a production release.

A user story is not considered complete until it has passed its acceptance tests. This means that new acceptance tests must be created each iteration or the development team will report zero progress.

Quality assurance (QA) is an essential part of the XP process. On some projects QA is done by a separate group, while on others QA will be an integrated  into  the  development  team itself. In either case XP requires development to have much closer relationship with QA.

Acceptance tests should be automated so they can be run often. The acceptance test score is published to the team. It is the team's responsibility to schedule time each iteration to fix any failed tests.

The name acceptance tests was changed from functional tests. This better reflects the intent, which is to guarantee that a customers requirements have been met and the system is acceptable. -->