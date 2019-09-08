<!-- Collective Ownership
 
Collective Ownership encourages everyone to contribute new ideas to all segments of the project. Any developer can change any line of code to add functionality, fix bugs, improve designs or refactor. No one person becomes a bottle neck for changes.

This is hard to understand at first. It's almost inconceivable that an entire team can be responsible for the system's design. Not having a single chief architect that keeps some visionary flame alive seems like it couldn't possibly work.

But it is not uncommon to ask a chief architect a question and get an answer that is just plain wrong. It is not a failing of your lead programmers. Any non-trivial system can not be held in one person's mind. Other programmers are hard at work changing the system without benefit of the architect's vision. Whether you realize it or not your design is already distributed among your team. If the entire team already has some responsibility for design decisions, shouldn't they receive the authority as well?

The way this works is for each developer to create unit tests for their code as it is developed. All code that is released into the source code repository includes unit tests that run at 100%. Code that is added, bugs as they are fixed, and old functionality as it is changed will be	covered by automated testing. Now you can rely on the test suite to watch dog your entire code repository. Before any code is released it must pass the entire test suite at 100%.

Once this is in place anyone can make a change to any method of any class and release it to the code repository as needed. When combined with frequent integration developers rarely even notice a class has been extended or repaired.

In practice collective ownership is actually more reliable than putting a single person in charge of watching specific classes. Especially since a person may leave the project at any time.

-->

# 集体所有制

极限编程提倡“所有人拥有所有代码”，鼓励每个人为项目的所有部分贡献新的想法。这种形式被称为“**代码集体所有制**”。任何开发人员都可以更改任何代码来添加功能、修复错误、改进设计或是重构。不会因为任何一个人缺席而无法做出修改。

起初这很难理解。“让整个团队负责系统的设计”，这听起来不可思议。很多人会认为：如果没有一个远见卓识的首席架构师保证项目的未来，似乎项目就不太可能成功。

然而，首席架构师也不是万能的。向首席架构师提出问题并得到完全错误的答案，这种情况也并不罕见。我们不能责怪首席架构师或主力开发，因为任何一个不小的系统都不可能记在一个人的脑海里。

另一方面，由于缺乏架构师的全局视野，团队中的程序员在修改系统时会遭遇困难。无论承不承认，软件设计的责任已经分散在整个团队中了。既然团队成员已经在做设计决策，为何不给他们充分的知识与赋权？

代码集体所有制之所以可行，是因为每个开发人员在开发代码时都[首先编写单元测试](test-first.md)。提交到代码库中的所有代码，都有100％的单元测试覆盖。不论是新添的功能、修复Bug的代码、还是更改旧功能的代码，都有自动化测试覆盖。依靠测试套件就可以监视整个代码库。任何代码都必须100％地通过整个测试套件，才有可能被发布使用。

有了这样一套测试套件，任何人都可以对任何类的任何方法进行更改，并将其提交到代码库。这种修改代码的方式与频繁的[持续集成](continuous-integration.md)相结合，开发人员甚至很少注意到类已被扩展或修复。

实践证明，集体所有制确实比“一个人负责一块代码”的方式更可靠。尤其考虑到任何人都有可能随时离开项目，集体所有制的优势就更加明显。 
