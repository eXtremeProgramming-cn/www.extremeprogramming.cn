<!-- # Unit Tests

Unit tests are one of the corner stones of Extreme Programming (XP). But unit tests XP style is a little different. First you should create or download a unit test framework to be able to create automated unit tests suites. Second you should test all classes in the system. Trivial getter and setter methods are usually omitted. You will also create your tests first, before the code.

Unit tests are released into the code repository along with the code they test. Code without tests may not be released. If a unit test is discovered to be missing it must be created at that time.

The biggest resistance to dedicating this amount of time to unit tests is a fast approaching deadline. But during the life of a project an automated test can save you a hundred times the cost to create it by finding and guarding against bugs. The harder the test is to write the more you need it because the greater your savings will be. Automated unit tests offer a pay back far greater than the cost of creation.

Another common misconception is that unit tests can be written in the last three months of  the project. Unfortunately, without the unit tests development drags on and eats up those last three months and then some. Even if the time is available good unit test suites take time to evolve. Discovering all the problems that can occur takes time. In order to have a complete unit test suite when you need it you must begin creating the tests today when you don't.

Unit tests enable collective ownership. When you create unit tests you guard your functionality from being accidentally harmed. Requiring all code to pass all unit tests before it can be released ensures all functionality always works. Individual code ownership is not required if all classes are guarded by unit tests.

Unit tests enable refactoring as well. After each small change the unit tests can verify that a change in structure did not introduce a change in functionality.

Building a single universal unit test suite for validation and regression testing enables frequent integration. It is possible to integrate any recent changes quickly then run your own latest version of the test suite. When a test fails your latest versions are incompatible with the team's latest versions. Fixing small problems every few hours takes less time than fixing huge problems just before the deadline. With automated unit tests it is possible to merge a set of changes with the latest released version and release in a short time.

Often adding new functionality will require changing the unit tests to reflect the functionality. 

While it is possible to introduce a bug in both the code and test it rarely happens in actual practice. It does occasionally happen that the test is wrong, but the code is right. This is revealed when the problem is investigated and is fixed. Creating tests independent of code, hopefully before code, sets up checks and balances and greatly improves the chances of getting it right the first time.

Unit Tests provide a safety net of regression tests and validation tests so that you can refactor and integrate effectively. As they say at the circus; never work without a net! Creating the unit test before the code helps even further by solidifying the requirements, improving developer focus, and avoid creeping elegance.

-->

# 单元测试

单元测试是极限编程的基石之一。但是与传统的单元测试相比，极限编程风格的单元测试又有点不同。首先，你应该创建或下载一个单元测试框架，以便能够创建自动化的单元测试套件。其次，你应该测试系统中的所有类、所有方法，最多省略一些简单到没有任何逻辑的getter和setter方法。你还必须在写代码之前[先写测试](test-first.md)。

单元测试与被测的代码一起提交到代码库中。未经测试的代码不能进入代码库。如果发现某个单元测试缺失，则必须马上创建它。

反对投入时间编写单元测试最常见的理由是“项目快到最后期限了”。但是在项目的生命周期中，自动化测试能有效地发现和防范错误，从而节省百倍的时间和成本。测试越难写，你就越需要它，因为它为你节省的时间成本越多。自动化单元测试所提供的回报远远大于创建它的成本。

另一个常见的误区是：集中在项目的最后阶段补写单元测试。不幸的是，没有单元测试的开发会拖延并消耗掉更多的时间，使团队实际上无法在那段时间补写单元测试。即使时间允许，补写单元测试也很困难，因为代码在编写时并没有考虑可测试性。为了在需要时拥有一个完整的单元测试套件，我们必须从一开始就创建测试，在编写代码之前先编写测试。

单元测试给[代码集体所有制](collective-ownership.md)提供了支持。有了单元测试，可以保护已有功能不受意外破坏。任何代码在提交之前都必须通过所有单元测试，从而确保所有功能始终正常工作。如果所有类都由单元测试保护，则不需要由特定的人来负责特定的代码块，任何人都可以修改任何代码。

单元测试也给[重构](refactoring.md)提供了支持。在每一个小的变更之后，单元测试都可以确保结构上的变更不会引起功能上的改变。

为验证和回归测试构建一个通用的单元测试套件，可以很好地支持[持续集成](continuous-integration.md)。持续集成可以快速集成任何最近的更改，然后运行最新版本的测试套件。当测试失败时，说明最新提交的代码出现了问题。每隔几个小时解决一个小问题比在最后期限前解决一个大问题要花更少的时间。

添加新功能时，通常需要更改单元测试，以反映新的功能需求。

虽然有可能在代码和测试中同时引入错误，但在实际情况中很少发生。确实会发生“单元测试错误但代码正确”的情况，此时对失败测试进行深入研究通常会找到问题所在。创建独立于代码的测试（最好是在写代码之前），可以建立**检查和制约**<sup>[注1](#checks_balances)</sup>，并大大提高从一开始就做对的机会。

单元测试提供了回归测试和验证测试的安全网，以便你可以有效地重构和集成。就像马戏团里常说的：没有安全网就不要表演！在代码之前创建单元测试，有助于进一步确定需求，提高开发人员的专注度，并避免过度设计。

<sub><a name="checks_balances">注1</a> 检查和制约：是指写代码之前先写测试，而在写代码时则要且仅要保证测试运行通过。这样代码就受到了检查和制约，也就是说保证了即不出现功能错误、也不过度设计。</sub>
