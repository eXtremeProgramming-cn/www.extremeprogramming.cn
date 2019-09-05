<!-- Collective Ownership
 
Collective Ownership encourages everyone to contribute new ideas to all segments of the project. Any developer can change any line of code to add functionality, fix bugs, improve designs or refactor. No one person becomes a bottle neck for changes.

This is hard to understand at first. It's almost inconceivable that an entire team can be responsible for the system's design. Not having a single chief architect that keeps some visionary flame alive seems like it couldn't possibly work.

But it is not uncommon to ask a chief architect a question and get an answer that is just plain wrong. It is not a failing of your lead programmers. Any non-trivial system can not be held in one person's mind. Other programmers are hard at work changing the system without benefit of the architect's vision. Whether you realize it or not your design is already distributed among your team. If the entire team already has some responsibility for design decisions, shouldn't they receive the authority as well?

The way this works is for each developer to create unit tests for their code as it is developed. All code that is released into the source code repository includes unit tests that run at 100%. Code that is added, bugs as they are fixed, and old functionality as it is changed will be	covered by automated testing. Now you can rely on the test suite to watch dog your entire code repository. Before any code is released it must pass the entire test suite at 100%.

Once this is in place anyone can make a change to any method of any class and release it to the code repository as needed. When combined with frequent integration developers rarely even notice a class has been extended or repaired.

In practice collective ownership is actually more reliable than putting a single person in charge of watching specific classes. Especially since a person may leave the project at any time.

-->

# 集体所有权

集体所有权鼓励每个人为项目的所有部分贡献新的想法。 任何开发人员都可以更改任何代码行来添加功能，修复错误，改进设计或重构。 没有人会成为改进的瓶颈。

起初这很难理解。 让整个团队负责系统的设计，这几乎是不可思议的。 如果没有一个有远见卓识的首席架构师保证项目的未来，似乎就不太可能成功。

然而，向首席架构师提出一个问题并得到一个完全错误的答案，这情况也并不罕见。 我们不能责怪首席架构师或主力开发，因为任何一个不小的系统都不可能记在一个人的脑海里。 实际上团队中的每个程序员都在努力改进系统，虽然他们也许并没有首席架构师的远见。 然而无论他是否意识到，他的设计已经在整个团队中传播开去。 如果整个团队已经对设计决策负有责任，那么他们不是也应该获得授权吗？

这种方式之所以可行，是因为每个开发人员在开发代码时都为其代码创建单元测试。 发布到源代码存储库中的所有代码都包含100％覆盖运行的单元测试。 新添的代码，修复 bug 的代码以及更改旧功能的代码都将由自动化测试覆盖。 现在，你就可以依靠测试套件来监视整个代码存储库。 在发布任何代码之前，它都必须 100％ 地通过整个测试套件才行。

一旦上述测试套件做到位，任何人都可以对任何类的任何方法进行更改，并根据需要将其发布到代码存储库。 当与持续集成相结合时，开发人员甚至很少注意到类已被扩展或修复。

在实践中也证明，集体所有权确实比某个人负责特定代码的方式更可靠。 由其是因为一个人可能随时离开项目。 
